# Monitoreo de Correos Electronicos
**Inicio de Monitoreo de Correo Electronico**
```powershell
Start-Monitor
```
Cuando inicie el proceso de monitoreo se espera a que un correo recibido cumpla con alguna de las reglas asociadas a alguna de las cuentas monitoreadas para ser procesado.
En cuanto se detecte un correo que cumpla con la regla se iniciara el proceso pertinente indicado en la regla como [Plugin](Plugin-Manager.md).

Para validar el estado de ejecucion del monitoreo:
```powershell
Get-MonitorState
```
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
