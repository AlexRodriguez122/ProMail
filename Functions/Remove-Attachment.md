---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Remove-Attachment

## SYNOPSIS
Elimina registros de asuntos válidos para los mensajes de correo entrantes.

## SYNTAX

```
Remove-Attachment [-AttachmentObject] <Object>
```

## DESCRIPTION
Elimina registros de asuntos válidos para los mensajes de correo entrantes.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Subject | Remove-Subject
```

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Subject -IdRule 19 | Remove-Subject
```

Elimina todos los asuntos vinculados a la regla de gestión cuyo identificador es 19.

## PARAMETERS

### -AttachmentObject
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
Autor: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

---------------------------------------------------------

## RELATED LINKS

[Add-Attachment](Add-Attachment.md)

[Get-Attachment](Get-Attachment.md)

