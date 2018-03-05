---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-RestrictedSender

## SYNOPSIS
Obtiene la lista de los remitentes prohibidos para el módulo.

## SYNTAX

```
Get-RestrictedSender [[-EmailAddress] <String>]
```

## DESCRIPTION
Obtiene la lista de los remitentes prohibidos para el módulo.
La salida 
puede ser canalizada como entrada de la función Remove-RestrictedSender.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-RestrictedSender -RestrictedSender canallatino@universaltv.com
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-RestrictedSender
```

## PARAMETERS

### -EmailAddress
Direcciones de correo para limitar las búsqueda

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

## INPUTS

## OUTPUTS

### Nombres de las cuentas bloqueadas obtenidas desde la base de datos

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 19/Ene/18

---------------------------------------------------------

## RELATED LINKS

[Register-RestrictedSender](Register-RestrictedSender.md)

[Unregister-RestrictedSender](Unregister-RestrictedSender.md)

