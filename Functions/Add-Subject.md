---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Add-Subject

## SYNOPSIS
Registra los asuntos válidos para los mensajes entrantes.

## SYNTAX

```
Add-Subject [-IdRule] <Int32> [-Subject] <String[]>
```

## DESCRIPTION
Registra los asuntos válidos para los mensajes entrantes, vinculándolos a la regla 
de gestión cuyo identificador se especifica.
Los diferentes enunciados de los asuntos
deberán ingresarse separados por comas.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-Subject -IdRule 114 -Subject 'activaciones', 'activar nuevos', 'bonos nuevos'
```

## PARAMETERS

### -IdRule
Identificador de la regla  a la cual desea vincular los asuntos que se ingresan.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: 0
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Subject
Enunciados de los asuntos que serán vinculados a las reglas previamente creadas cuyos identificadores se 
especifican.
Los diferentes enunciados deberán ir separados por comas.

```yaml
Type: String[]
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

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[[Add-Subject](Add-Subject.md)
[Remove-Subject](Remove-Subject.md)]()

