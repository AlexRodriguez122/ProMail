---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-Attachment

## SYNOPSIS
Obtiene los nombre de los adjuntos permitidos por regla.

## SYNTAX

```
Get-Attachment [[-Attachment] <String>] [[-IdRule] <String>]
```

## DESCRIPTION
Obtiene los nombre de los adjuntos permitidos por regla.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Attachment
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Attachment -Attachment Prueba.txt
```

### -------------------------- EXAMPLE 3 --------------------------
```
Get-Attachment -Attachment Prueba.txt -IdRule 2
```

### -------------------------- EXAMPLE 4 --------------------------
```
Get-Attachment -IdRule 2
```

## PARAMETERS

### -Attachment
nombre del adjuntos que se desea obtener.

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
Identificador de la regla de la cual se desea obtener los adjuntos.

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

### Processa.Management.Automation.ProMail.Attachment

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Get-Attachment](Get-Attachment.md)

[Add-Attachment](Add-Attachment.md)

[Remove-Attachment](Remove-Attachment.md)

