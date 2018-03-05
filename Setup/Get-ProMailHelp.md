
# ¿Qué hace cada una de las funciones?

Para obtener ayuda sobre cada una de las funciones puede utilizar el comando [Get-Help](https://msdn.microsoft.com/en-us/powershell/reference/5.1/microsoft.powershell.core/get-help) de PowerShell. La sintaxis es Get-Help seguido del nombre de la función. Supongamos que desea observar la ayuda del comando Set-ReportConfig del módulo.

```powershell
Get-Help Register-EmailAccount
```

Get-Help inicialmente muestra un resumen de la ayuda. Si desea observar toda la ayuda, ejecute:

```powershell
Get-Help Register-EmailAccount -Full
```

Observar los ejemplos:

```powershell
Get-Help Register-Rule -Examples
```

Observar la ayuda de un parámetro (en este caso EncryptedKey):

```powershell
Get-Help Register-Rule -Parameter EncryptedKey
```

Observar la ayuda en una ventana de Windows (en lugar de en la consola)

```powershell
Get-Help Register-Rule -ShowWindow
```

Observar la ayuda en línea (a través del Browser)

```powershell
Get-Help Register-Rule -Online
```
