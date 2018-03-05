---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Enable-EmailAccount

## SYNOPSIS
Habilita las cuentas indicadas para ser monitoreadas.

## SYNTAX

### WithIdEmailAccount
```
Enable-EmailAccount -IdEmailAccount <Int32>
```

### WithObject
```
Enable-EmailAccount -ObjectEmailAccount <Object>
```

## DESCRIPTION
Habilita las cuentas indicadas para ser monitoreadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-EmailAccount | Enable-Emailaccount
```

### -------------------------- EXAMPLE 2 --------------------------
```
Enable-Emailaccount -IdEmailAccount 2
```

## PARAMETERS

### -IdEmailAccount
Indicador de la cuenta que se desea habilitar.

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
Objeto con la informacion de la cuenta a habilitar.

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

[[Enable-EmailAccount](Enable-EmailAccount.md)
[Disable-EmailAccount](Disable-EmailAccount.md)]()

