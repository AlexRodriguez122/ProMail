---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Add-Attachment

## SYNOPSIS
Registra nombres válidos para los archivos adjuntos a los mensajes entrantes,
vinculándolos a una regla de gestión.

## SYNTAX

```
Add-Attachment [-IdRule] <Int32> [-AttachmentsName] <String[]>
```

## DESCRIPTION
Registra nombres válidos para los archivos adjuntos a los mensajes entrantes, vinculándolos 
a reglas previamente creadas.
La extensión admitida para los archivos adjuntos es '.txt'.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-AttachmentName -IdRule 75 -AttachmentsName 'Listado Enero.txt', 'Activaciones enero.txt'
```

## PARAMETERS

### -IdRule
Identificador de la regla a la cual sera agregado el asunto.

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

### -AttachmentsName
Nombres de archivos adjuntos que serán considerados válidos, admite varios nombres 
separados por comas, cada nombre debe incluir la extensión '.txt'.

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
Autor: \<jarodriguezc\>
Última Modificación: 23/02/18
---------------------------------------------------------

## RELATED LINKS

[Get-Attachment](Get-Attachment.md)

[Remove-Attachment](Remove-Attachment.md)

