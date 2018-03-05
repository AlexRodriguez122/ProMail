---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Register-RestrictedSender

## SYNOPSIS
Registra cuentas de correo remitentes que serán consideradas como prohibidas

## SYNTAX

### WithArray (Default)
```
Register-RestrictedSender -EmailRestricted <String[]>
```

### WithPath
```
Register-RestrictedSender -EmailRestrictedPath <String>
```

## DESCRIPTION
Registra cuentas de correo remitentes que serán consideradas como restringidas o
prohibidas, en consecuencia, los mensajes provenientes de estas cuentas de correo
serán almacenados ningún criterio adicional.
Estos remitentes prohibidos aplican
para todas las reglas de gestión creadas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Register-RestrictedSender -EmailRestricted mailbox1@gmail.com, mailbox34@gmail.com
```

### -------------------------- EXAMPLE 2 --------------------------
```
Register-RestrictedSender -EmailRestrictedPath 'C:\Ruta\Restringidos.txt'
```

## PARAMETERS

### -EmailRestricted
Direcciones de correo electrónico (remitentes) que serán bloqueadas.
Las diferentes
cuentas de correo deberán ingresarse separadas por comas.

```yaml
Type: String[]
Parameter Sets: WithArray
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EmailRestrictedPath
Ruta del archivo .txt con el cual se cargaran las direcciones de correo que seran restringidas.

```yaml
Type: String
Parameter Sets: WithPath
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Ninguna

## OUTPUTS

### Ninguna.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Unregister-RestrictedSender](Unregister-RestrictedSender.md)

[Get-RestrictedSender](Get-RestrictedSender.md)

