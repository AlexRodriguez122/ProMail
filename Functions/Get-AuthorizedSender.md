---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-AuthorizedSender

## SYNOPSIS
Obtiene la lista de remitentes autorizados.

## SYNTAX

```
Get-AuthorizedSender [[-EmailAuthorized] <String>] [[-IdRule] <String>]
```

## DESCRIPTION
Obtiene la lista de remitentes autorizados.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-AuthorizedSender -EmailAuthorized 'inversionesardila@yahoo.com'
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-AuthorizedSender -IdRule 2
```

### -------------------------- EXAMPLE 3 --------------------------
```
Get-AuthorizedSender -IdRule 2 -EmailAuthorized 'inversionesardila@yahoo.com'
```

## PARAMETERS

### -EmailAuthorized
Remitente autorizado que se desea consultar.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: *
Accept pipeline input: False
Accept wildcard characters: True
```

### -IdRule
Identificador de regla de los remitentes que desea consultar.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: *
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: True
```

## INPUTS

## OUTPUTS

### Processa.Management.Automation.ProMail.AuthorizedMailbox

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Add-AuthorizedSender](Add-AuthorizedSender.md)

[Remove-AuthorizedSender](Remove-AuthorizedSender.md)

