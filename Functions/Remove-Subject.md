---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Remove-Subject

## SYNOPSIS
Elimina registros de asuntos válidos para los mensajes de correo entrantes.

## SYNTAX

```
Remove-Subject [-SubjectObject] <Object>
```

## DESCRIPTION
Elimina registros de asuntos válidos para los mensajes de correo entrantes.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Subject | Remove-Subject
```

## PARAMETERS

### -SubjectObject
Información de los asuntos que se desea eliminar.

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

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguez\>
Última Modificación: 19/Ene/18

---------------------------------------------------------

## RELATED LINKS

[Remove-Subject](Remove-Subject.md)

[Get-Subject](Get-Subject.md)

