---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Register-EmailAccount

## SYNOPSIS
Registra una cuenta de correo para monitorear.

## SYNTAX

```
Register-EmailAccount [-Name <String>] [-EmailAddress <String>] [-Password <SecureString>] [-Force]
```

## DESCRIPTION
Registra una cuenta de correo receptora, la cual ha de ser vinculada a una regla de gestión.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Register-EmailAccount
```

## PARAMETERS

### -Name
Nombre con el que se guardara la cuenta a monitorear, en caso de no enviarse se utilizara la direccion de correo.

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

### -EmailAddress
Direccion de correo electronico que se monitoreara.
si no son enviados los parametros EmailAddress y Password se abrira un cuadro de dialogo que solicitara la informacion.

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

### -Password
Secure String con la contraseña de la cuenta a monitorear. 
si no son enviados los parametros EmailAddress y Password se abrira un cuadro de dialogo que solicitara la informacion.

```yaml
Type: SecureString
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
{{Fill Force Description}}

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

## OUTPUTS

## NOTES
---------------------------------------------------------
Autor: \<Jarodriguezc\>
Última Modificación: 15/Dic/17

---------------------------------------------------------

## RELATED LINKS

[Get-EmailAccount](Get-EmailAccount.md)

[Update-EmailAccountPassword](Update-EmailAccountPassword.md)

[Add-RuleToEmailAccount](Add-RuleToEmailAccount.md)

[Remove-RuleFromEmailAccount](Remove-RuleFromEmailAccount.md)

