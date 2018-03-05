---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-Template

## SYNOPSIS
Obtiene la informacion de la plantilla de una regla.

## SYNTAX

```
Get-Template [-IdRule] <Int32>
```

## DESCRIPTION
Obtiene la informacion de la plantilla de una regla.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Template -IdRule 1
```

## PARAMETERS

### -IdRule
Identificador de la regla de la cual se desea obtener los adjuntos.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 0
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
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

[Update-RuleTemplate](Get-RuleTemplate.md)

