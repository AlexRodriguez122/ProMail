# ¿Cómo instalar?

### Versión Online

1. Abra una ventana de PowerShell como usuario administrador y registre el repositorio de Nuget

```powershell
Register-PSRepository -Name 'Processa GT' -SourceLocation 'http://proget:8020/nuget/PowerShell' -InstallationPolicy Trusted
```
**En el valor del parametro -SourceLocation se debe cambiar el token 'proget' por la ip donde se encuentre el repositorio** 
- Nota: si desea validar que repositorios tiene registrados
``` powershell
Get-PSRepository
```

2. Instale el módulo desde el Repositorio

```powershell
Install-Module -Name 'ProMail' -Repository 'Processa GT'
```

# ¿Cómo actualizar?

Si el módulo ya está instalado solo tiene que actualizarlo. 

1. Asegurese de tener registrado el repositorio de Nuget.

```powershell
Get-PSRepository -Name 'Processa GT'
```

2. Actualice el módulo desde el Repositorio

```powershell
Update-Module -Name 'ProMail' -Force
```
