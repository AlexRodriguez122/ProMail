---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Register-Rule

## SYNOPSIS
Registra una regla de gestión para los mensajes de correo entrantes.

## SYNTAX

### WithArray
```
Register-Rule -Name <String> -AuthorizedSender <String[]> -Subject <String[]> -AttachmentsName <String[]>
 -PluginName <String> [-ResponseTemplatePath <String>]
```

### WithPath
```
Register-Rule -Name <String> -AuthorizedSenderPath <String> -Subject <String[]> -AttachmentsName <String[]>
 -PluginName <String> [-ResponseTemplatePath <String>]
```

## DESCRIPTION
Registra una regla de gestión para los mensajes de correo entrantes. 
Recibe como parámetros los elementos que conformarán la nueva regla.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Register-Rule -Name Prueba -AuthorizedSender Correo@Correo.com -Subject 'Prueba1' -AttachmentName 'Prueba1.txt' -Plugin 'NombrePlugin'
```

## PARAMETERS

### -Name
Nombre con el cual sera guardada la regla.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthorizedSender
Arreglo con las cuentas de correo que serán registradas como remitentes autorizados.

```yaml
Type: String[]
Parameter Sets: WithArray
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AuthorizedSenderPath
Ruta del archivo que contiene las cuentas de correo que serán registradas como remitentes autorizados.

```yaml
Type: String
Parameter Sets: WithPath
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Subject
Arreglo con los asuntos admitidos por esta regla.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AttachmentsName
Arreglo con los nombres admitidos para los archivos adjunto de los correos entrantes.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PluginName
Nombre del plugin que se va a invocar para procesar los archivos adjuntos descargados.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResponseTemplatePath
Plantilla html de respuesta para los correos.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Ninguna

## OUTPUTS

### Registro nuevo de una regla de gestión en la base de datos.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Get-Rule](Get-Rule.md)

[Update-RuleTemplate](Update-RuleTemplate.md)

