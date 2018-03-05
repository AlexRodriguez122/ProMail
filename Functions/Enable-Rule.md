---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Enable-Rule

## SYNOPSIS
Habilita las reglas a ser monitoreadas.

## SYNTAX

### WithIdRule
```
Enable-Rule -IdRule <Int32>
```

### WithObject
```
Enable-Rule -ObjectRule <Object>
```

## DESCRIPTION
Habilita las reglas a ser monitoreadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Rule | Enable-Rule
```

### -------------------------- EXAMPLE 2 --------------------------
```
Enable-Rule -IdRule 2
```

## PARAMETERS

### -IdRule
Identificador de la regla que se desea habilitar.

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
Objeto con la informacion de las cuentas a habilitar.

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
Última Modificación: 19/Ene/18

---------------------------------------------------------

## RELATED LINKS

[Enable-Rule](Enable-Rule.md)

[Disable-Rule](Disable-Rule.md)

