---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-Subject

## SYNOPSIS
Obtiene los enunciados de asuntos de mensajes entrantes.

## SYNTAX

```
Get-Subject [[-Subject] <String>] [[-IdRule] <String>]
```

## DESCRIPTION
Obtiene los enunciados de asuntos de mensajes entrantes.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Subject -Subject prueba
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Subject -IdRule 4
```

### -------------------------- EXAMPLE 3 --------------------------
```
Get-Subject
```

### -------------------------- EXAMPLE 4 --------------------------
```
Get-Subject -IdRule 4 -Subject prueba
```

## PARAMETERS

### -Subject
Obtiene los asuntos por las reglas indicadas.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: *
Accept pipeline input: False
Accept wildcard characters: True
```

### -IdRule
Identificador de la regla de la cual se desean obtener los asuntos.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: *
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: True
```

## INPUTS

## OUTPUTS

### Asuntos vinculados al identificador de regla especificado. Obtenidos desde la base de datos.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 19/Ene/18

---------------------------------------------------------

## RELATED LINKS

[[Get-Subject](Get-Subject.md)]()

[[Remove-Subject](Remove-Subject.md)]()

