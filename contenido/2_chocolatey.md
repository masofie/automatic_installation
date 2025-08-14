# 🚀 Instalación de Programas en Windows con Chocolatey
<br>

- [🚀 Instalación de Programas en Windows con Chocolatey](#-instalación-de-programas-en-windows-con-chocolatey)
  - [📦 Chocolatey](#-chocolatey)
  - [1. Instalación](#1-instalación)

<br>

## 📦 Chocolatey
<br>

**``Chocolatey``** es un gestor de paquetes para Windows, similar a ``apt`` en Linux. Permite instalar y gestionar programas desde la terminal (PowerShell).

<br>

## 1. Instalación 
<br>


1 - Ve a la página oficial [Chocolatey](https://chocolatey.org/install) y sigue los pasos .

![Explicación inicial](./img/img_chocolatey/1_explicacion_inicial.png)
<br><br>




2 - Abrir PowerShell como administrador:

Busca PowerShell en el menú, haz clic derecho y selecciona "Ejecutar como administrador".

![Powershell admin](./img/img_chocolatey/2_admin_powershell.png)
<br><br>




3 - Verificar la política de ejecución:

Para permitir la instalación de scripts, copia y ejecuta este comando para ver tu política actual:

~~~~
# Politicas de Ejecución
Get-ExecutionPolicy

# Clausula
Restricted
~~~~

![Comando policy](./img/img_chocolatey/3_set-execution_policy.png)
<br><br>




3 - Cambiar la política de ejecución:

Cambia la política para permitir la ejecución de scripts firmados , Confirma escribiendo S (Sí) cuando te pregunte.

~~~~
Set-ExecutionPolicy AllSigned
~~~~

![Comando allsigned](./img/img_chocolatey/4_set-execution_allsigned.png)
<br><br>




4 - Permitir la ejecución temporal para este proceso. Para evitar problemas, ejecuta este comando:

~~~~
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
~~~~


![Comando process](./img/img_chocolatey/5_set-execution_process.png)
<br><br>



5 - Instalar Chocolatey:

Copia y ejecuta el script de instalación oficial desde la página de Chocolatey.


![Comando process](./img/img_chocolatey/6_comando_ejecucion.png)
<br><br>