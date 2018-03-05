---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Add-AuthorizedSender

## SYNOPSIS
Registra remitentes autorizados vinculándolos a una regla de gestión.

## SYNTAX

### FromHost (Default)
```
Add-AuthorizedSender -IdRule <Int32>
```

### WithArray
```
Add-AuthorizedSender -IdRule <Int32> -EmailAuthorized <String[]>
```

### WithPath
```
Add-AuthorizedSender -IdRule <Int32> -EmailAuthorizedPath <String>
```

## DESCRIPTION
Registra remitentes autorizados vinculándolos a reglas previamente creadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-AuthorizedSender -IdRule 72 -EmailAuthorized porcelanas@InduCeram.com
```

### -------------------------- EXAMPLE 2 --------------------------
```
Add-AuthorizedSender -IdRule 144 -EmailAuthorizedPath 'C:\Ruta\Autorizados.txt'
```

## PARAMETERS

### -IdRule
Identificador de la regla a la cual se desea vincular los remitentes autorizados.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: 0
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EmailAuthorized
Direcciones de correo electrónico, separadas por comas, que serán registradas como remitentes
autorizados para la regla cuyo identificador se define en el parámetro IdRule.

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

### -EmailAuthorizedPath
{{Fill EmailAuthorizedPath Description}}

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

## INPUTS

## OUTPUTS

### System.Int32

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Add-AuthorizedSender](Add-AuthorizedSender.md)

[Remove-AuthorizedSender](Remove-AuthorizedSender.md)


