---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Update-RuleTemplate

## SYNOPSIS
Actualiza la plantilla de respuesta de correo a una regla indicada.

## SYNTAX

### WithIdRule
```
Update-RuleTemplate -IdRule <Int32> [-ResponseTemplatePath <String>]
```

### WithObject
```
Update-RuleTemplate -ObjectRule <Object> [-ResponseTemplatePath <String>]
```

## DESCRIPTION
Actualiza la plantilla de respuesta de correo a una regla indicada.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Update-RuleTemplate -IdRule 1 -ResponseTemplatePath 'c:\Template.html'
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Rule -id 1 | Update-RuleTemplate -ResponseTemplatePath 'c:\Template.html'
```

## PARAMETERS

### -IdRule
Identificadores de la regla a la cual se realizara el cambio de plantilla.

```yaml
Type: Int32
Parameter Sets: WithIdRule
Aliases: 

Required: True
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectRule
Objeto con la regla a la cual se realizara el cambio de plantilla.

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

### -ResponseTemplatePath
ruta de la plantilla nueva para la respuesta de correos

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### Ninguna

## OUTPUTS

### Registros nuevos de nombres de archivos adjuntos permitidos en una regla de gestión.

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[[Update-RuleTemplate](Update-RuleTemplate.md)]()

