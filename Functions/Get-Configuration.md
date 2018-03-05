---
external help file: ProMail-help.xml
Module Name: ProMail
online version: 
schema: 2.0.0
---

# Get-Configuration

## SYNOPSIS
Obtiene la información de los datos de configuración del módulo.

## SYNTAX

```
Get-Configuration
```

## DESCRIPTION
Obtiene la información de los datos de configuración del módulo a partir de los datos en el archivo \<%=$PLASTER_PARAM_ModuleName%\>.config

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-Configuration
```

Obtiene la información de configuración del módulo.

### -------------------------- EXAMPLE 2 --------------------------
```
Get-Configuration | Get-Member -MemberType Properties
```

Obtiene los nombres de las propiedades incluidas en el objeto de retorno.

## PARAMETERS

## INPUTS

### Ninguna

## OUTPUTS

### System.Management.Automation.PSObject

## NOTES
Autor:              \<Magudelo\> 
Autor Modificacion: \<Jarodriguezc\>
Última Modificación: 23/Feb/18

## RELATED LINKS

[[Set-Configuration](Set-Configuration.md)
[Test-Configuration](Test-Configuration.md)]()

