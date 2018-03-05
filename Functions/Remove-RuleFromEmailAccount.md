---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Remove-RuleFromEmailAccount

## SYNOPSIS
Desvincula n reglas a su respectivas cuentas.

## SYNTAX

```
Remove-RuleFromEmailAccount [-ObjectEmailAccount] <Object> [-IdRule] <Int32[]>
```

## DESCRIPTION
Desvincula n reglas a su respectivas cuentas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-EmailAccount | Remove-RuleFromEmailAccount -Idrule 1
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-EmailAccount -Emailaddres 'prueba@prueba.com' | Remove-RuleFromEmailAccount -Idrule 1
```

### -------------------------- EXAMPLE 3 --------------------------
```
Get-EmailAccount | Remove-RuleFromEmailAccount -IdRule 1,2,3
```

## PARAMETERS

### -ObjectEmailAccount
Objeto con las cuentas a las cuales se desvincularan con las regalas definidas.

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

### -IdRule
identificador de las reglas que seran desvinculadas de las cuentas.

```yaml
Type: Int32[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### System.Void

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Remove-RuleFromEmailAccount](Remove-RuleFromEmailAccount.md)

[Add-RuleToEmailAccount](Add-RuleToEmailAccount.md)
