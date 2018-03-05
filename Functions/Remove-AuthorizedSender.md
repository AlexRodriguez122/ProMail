---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Remove-AuthorizedSender

## SYNOPSIS
Elimina registros de remitentes autorizados.

## SYNTAX

```
Remove-AuthorizedSender [-EmailAdressObject] <Object>
```

## DESCRIPTION
Elimina registros de remitentes autorizados.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-AuthorizedSender | Remove-AuthorizedSender
```

## PARAMETERS

### -EmailAdressObject
Información de las cuentas remitentes autorizadas que se desea eliminar.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

### Ninguna

## OUTPUTS

### Ninguna

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Remove-AuthorizedSender](Remove-AuthorizedSender.md)

[Get-AuthorizedSender](Get-AuthorizedSender.md)

