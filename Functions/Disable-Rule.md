---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Disable-Rule

## SYNOPSIS
Deshabilita las reglas indicadas para no ser monitoreadas.

## SYNTAX

### WithIdRule
```
Disable-Rule -IdRule <Int32>
```

### WithObject
```
Disable-Rule -ObjectRule <Object>
```

## DESCRIPTION
Deshabilita las reglas indicadas para no ser monitoreadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Rule -IdRule 1 | Disable-Rule
```

### -------------------------- EXAMPLE 2 --------------------------
```
Disable-Rule -IdRule 1
```

## PARAMETERS

### -IdRule
Identificador de la regla que se deshabilitara.

```yaml
Type: Int32
Parameter Sets: WithIdRule
Aliases: 

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectRule
Objeto con las reglas que seran deshabilitadas.

```yaml
Type: Object
Parameter Sets: WithObject
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[[Disable-Rule](Disable-Rule.md)
[Enable-Rule](Enable-Rule.md)]()

