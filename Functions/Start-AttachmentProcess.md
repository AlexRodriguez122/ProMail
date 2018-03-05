---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Start-AttachmentProcess

## SYNOPSIS
Inicia el procesamiento de un archivo adjunto.

## SYNTAX

```
Start-AttachmentProcess [-JobName] <String> [-AttachmentPath] <String> [-ReceivedMsg] <PSObject>
 [-ObjectRule] <PSObject> [-Credential] <PSCredential> [-Attachment] <String>
```

## DESCRIPTION
Inicia el procesamiento de un archivo adjunto que superó las verificaciones de la regla.
El archivo adjunto recibido será pasado a un proceso externo para que se encargue de analizar su contenido y 
llevar acabo el proceso requerido.
Está función, luego de iniciar el proceso, esperará el resultado del mismo.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Start-AttachmentProcess -JobName 'Ejemplo1' -AttachmentPath 'C:\Adjuntos\Bloqueos_febrero_317.txt' -ReceivedMsg $EmailMsg -PluginName 'Bloquear-Bonos' -Credential = $Credential
```

## PARAMETERS

### -JobName
Nombre del proces

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -AttachmentPath
Ubicación del archivo adjunto luego de ser descargado, esta ruta le indica al proceso externo donde 
encontrar el archivo requerido.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReceivedMsg
El mensaje recibido que superó las validaciones y permitió que se iniciara el proceso externo. 
De este mensaje son requeridos la dirección del remitente y el asunto.

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectRule
{{Fill ObjectRule Description}}

```yaml
Type: PSObject
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Credencial con la que se conectara para el envio de correo.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Attachment
{{Fill Attachment Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Ninguna

## OUTPUTS

### Un mensaje de correo en respuesta a cada mensaje recibido de un remitente no bloqueado. Cuando aplica, el mensaje de
respuesta invluye el resultado del proceso y el archivo adjunto requerido.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[[Start-AttachmentProcess](Start-AttachmentProcess.md)]()

