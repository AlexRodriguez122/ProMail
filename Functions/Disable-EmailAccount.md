---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Disable-EmailAccount

## SYNOPSIS
Deshabilita las cuentas indicadas para que no sean monitoreadas.

## SYNTAX

### WithIdEmailAccount
```
Disable-EmailAccount -IdEmailAccount <Int32>
```

### WithObject
```
Disable-EmailAccount -ObjectEmailAccount <Object>
```

## DESCRIPTION
Deshabilita las cuentas indicadas para que no sean monitoreadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-EmailAccount -EmailAddress 'prueba@prueba.com' | Disable-EmailAccount
```

### -------------------------- EXAMPLE 2 --------------------------
```
Disable-EmailAccount -IdEmailAccount 2
```

## PARAMETERS

### -IdEmailAccount
Identificador de la cuenta que se deshabilitara.

```yaml
Type: Int32
Parameter Sets: WithIdEmailAccount
Aliases: 

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectEmailAccount
Objeto que contiene la informacion de las cuentas que se deshabilitaran.

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

[Disable-EmailAccount](Disable-EmailAccount.md)

[Enable-EmailAccount](Enable-EmailAccount.md)

