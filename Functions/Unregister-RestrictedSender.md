---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Unregister-RestrictedSender

## SYNOPSIS
Elimina registros de remitentes prohibidos.

## SYNTAX

```
Unregister-RestrictedSender [-EmailRestrictedObject] <Object>
```

## DESCRIPTION
Elimina registros de remitentes prohibidos, los cuales, aplican para todas las reglas y buzones.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-RestrictedSender | Unregister-RestrictedSender
```

Elimina TODOS los registros de remitentes prohibidos.

### -------------------------- EXAMPLE 2 --------------------------
```
Get-RestrictedSender -EmailAccount blackMailer@airmail.net | Unregister-RestrictedSender
```

Elimina la cuenta de correo blackMailer@airmail.net de la lista de remitentes prohibidos.

### -------------------------- EXAMPLE 3 --------------------------
```
Get-RestrictedSender -EmailAccount *yellow*.com | Unregister-RestrictedSender
```

Elimina todas las cuentas remitentes prohibidas que contengan la palabra yellow y cuyo 
dominio finalize con '.com'.

## PARAMETERS

### -EmailRestrictedObject
{{Fill EmailRestrictedObject Description}}

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

## INPUTS

### Ninguna

## OUTPUTS

### Ninguna

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 19/Ene/18

---------------------------------------------------------

## RELATED LINKS

[[Unregister-RestrictedSender](Unregister-RestrictedSender.md)]()

[[Get-RestrictedSender](Get-RestrictedSender.md)]()

