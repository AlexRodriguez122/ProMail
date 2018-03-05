---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Update-EmailAccountPassword

## SYNOPSIS
Actualiza la contraseña de una cuenta de correo indicada.

## SYNTAX

```
Update-EmailAccountPassword [-ObjectEmailAccount] <Object> [-Force]
```

## DESCRIPTION
Actualiza la contraseña de una cuenta de correo indicada.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-EmailAccount -EmailAddress 'prueba@prueba.com' | Update-EmailAccountPassword
```

## PARAMETERS

### -ObjectEmailAccount
Objeto con la cuenta a la cual sera actualizada la contraseña.

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

### -Force
Si esta presente no se validaran las nuevas credenciales.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
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

[Update-EmailAccountPassword](Update-EmailAccountPassword.md)

[Get-EmailAccount](Get-EmailAccount.md)

[Register-EmailAccount](Register-EmailAccount.md)

