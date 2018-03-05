---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-EmailAccount

## SYNOPSIS
Obtiene las de cuentas de correo registradas para ser monitoreadas.

## SYNTAX

```
Get-EmailAccount [[-EmailAddress] <String>] [[-Name] <String>]
```

## DESCRIPTION
Obtiene las cuentas de correo registradas para ser monitoreadas.
Por defecto se muestran todas las cuentas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-EmailAccount
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-EmailAccount -EmailAddress 'MyName@gmail.com'
```

### -------------------------- EXAMPLE 3 --------------------------
```
Get-EmailAccount -Name 'MyName'
```

## PARAMETERS

### -EmailAddress
Cuenta de correo que se desea buscar.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: *
Accept pipeline input: True (ByValue)
Accept wildcard characters: True
```

### -Name
Nombre de la cuenta para filtrar la consulta.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: *
Accept pipeline input: False
Accept wildcard characters: True
```

## INPUTS

## OUTPUTS

### Información de las cuentas receptoras en objetos.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[[Get-EmailAccount](Get-EmailAccount.md)
[Register-EmailAccount](Register-EmailAccount.md)]()

