# ¿Como funciona el módulo?
Este módulo permite la automatización de procesos por correo electrónico, permitiendo crear reglas para la ejecución de procesos previos una vez se reciba un correo que cumpla la regla creada.

Para registrar una cuenta a monitorear :
```powershell
Register-EmailAccount
Register-EmailAccount -Name 'NombreDeseado'
Register-EmailAccount -EmailAddress 'correo@correo.com' -Password (SecureString)
Register-EmailAccount -Name 'NombreDeseado' -EmailAddress 'correo@correo.com' -Password (SecureString)
```
- **Nota:**
En caso de no enviar los parametros EmailAddress y Pasword aparecera una ventana emergente solicitando las credenciales.
Todas las combinaciones del comando anterior permiten el parametro -Force el cual permite registrar una cuenta sin validar la conexion .

Una vez registrada una cuenta es necesario crear una regla para obtener un correo especifico de la bandeja de entrada.

```powershell
Register-Rule -Name (NombreIntuitivo) -AuthorizedSender 'Correo@correo.com' -Subject 'Asunto' -AttachmentsName 'Adjunto.txt' -PluginName 'ProcesoAEjecutar'
Register-Rule -Name (NombreIntuitivo) -AuthorizedSender 'Correo@correo.com','Prueba@Prueba.com' -Subject 'Asunto','Asunto2' -AttachmentsName 'Adjunto.txt','Adjunto2.txt' -PluginName 'ProcesoAEjecutar'
Register-Rule -Name (NombreIntuitivo) -AuthorizedSenderPath 'C:\RutaArchivoConCorreosAuthorizados.txt' -Subject 'Asunto' -AttachmentsName 'Adjunto.txt' -PluginName 'ProcesoAEjecutar'
Register-Rule -Name (NombreIntuitivo) -AuthorizedSender 'Correo@correo.com' -Subject 'Asunto' -AttachmentsName 'Adjunto.txt' -PluginName 'ProcesoAEjecutar' -ResponseTemplatePath 'C:\RutaPlantillaEnviodeCorreo.hmtl'
```
- **Nota:**
El Nombre debe ser Intuitivo ya que permite que varias reglas puedan tener el mismo nombre.

Cuando se tenga la regla creada se debe asociar la regla a la cuenta.

```powershell
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Add-RuleToEmailAccount -IdRule (Get-Rule -Name 'NombreIntuitivo').IdRule
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Add-RuleToEmailAccount -IdRule 1
```
- **Nota:**
Para obtener el Identificador de Regla (IdRule) se debe utilizar la funcion Get-Rule.
```powershell
Get-Rule -Name 'NombreIntuitivo'
Get-Rule -IdRule 1
Get-Rule
```

Para validar que reglas tiene asociada una cuenta se puede utilizar el siguiente comando :
```powershell
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Get-Rule
```

**Inicio de Monitoreo de Correo Electronico**
```powershell
Start-Monitor
```
Cuando inicie el proceso de monitoreo se espera a que un correo recibido cumpla con alguna de las reglas asociadas a alguna de las cuentas monitoreadas para ser procesado.
En cuando se detecte un correo que cumpla con la regla se iniciara el proceso pertinente indicado en la regla como Plugin.

Para validar el proceso de un correo recibido se puede utilizar el sigueinte comando:
```powershell
Get-JobState
```
- **Nota:**
despues de completado el proceso del plugin la informacion del job sera eliminada de la base de datos pero no del log del proceso.

Para detener el monitoreo de la cuenta se debe utilizar el sigueinte comando:
```powershell
Stop-Monitor
```
Para deshabilitar el monitoreo a una cuenta de correo:
```powershell
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Disable-EmailAccount
```
Para habilitar el monitoreo a una cuenta de correo:
```powershell
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Enable-EmailAccount
```
Para deshabilitar una regla **(Para todas las cuentas asociadas)** :
```powershell
Get-Rule -IdRule 1 | Disable-Rule
Get-Rule -IdRule 1,2 | Disable-Rule
```
Para habilitar una regla **(Para todas las cuentas asociadas)** :
```powershell
Get-Rule -IdRule 1 | Enable-Rule
Get-Rule -IdRule 1,2 | Enable-Rule
```
Para remover la asociacion de la regla a una cuenta:
```powershell
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Remove-RuleFromEmailAccount -IdRule 1
Get-EmailAccount -EmailAddress 'correomonitoreado@correo.com' | Remove-RuleFromEmailAccount -IdRule 1,2
```



