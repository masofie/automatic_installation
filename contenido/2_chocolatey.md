# 🚀 Instalación de Programas en Windows con Chocolatey
<br>

- [🚀 Instalación de Programas en Windows con Chocolatey](#-instalación-de-programas-en-windows-con-chocolatey)
  - [📦 Chocolatey](#-chocolatey)
    - [1. Instalación](#1-instalación)
    - [2. Instalación de Programas](#2-instalación-de-programas)

<br>

## 📦 Chocolatey
<br>

**``Chocolatey``** es un gestor de paquetes para Windows, similar a ``apt`` en Linux. Permite instalar y gestionar programas desde la terminal (PowerShell).

<br>

### 1. Instalación 
<br>


1 - Ve a la página oficial de [Chocolatey](https://chocolatey.org/install) , sigue los pasos marcados.

![Explicación inicial](./img/img_chocolatey/1_explicacion_inicial.png)
<br><br>




2 - Abrir ``PowerShell`` como administrador:

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

Cambia la política para permitir la ejecución de scripts firmados , Confirma escribiendo ``S (Sí)`` cuando te pregunte.

~~~~
Set-ExecutionPolicy AllSigned
~~~~

![Comando allsigned](./img/img_chocolatey/4_set-execution_allsigned.png)
<br><br>




4 - Permitir la ejecución temporal para este proceso. Para evitar problemas, ejecuta este comando:

~~~~
ExecutionPolicy Bypass -Scope Process
~~~~

![Comando process](./img/img_chocolatey/5_set-execution_process.png)
<br><br>



5 - Instalar Chocolatey:

Copia y ejecuta el script de instalación oficial desde la página de Chocolatey.

~~~~
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
~~~~

![Comando process](./img/img_chocolatey/6_comando_ejecucion.png)
<br><br>



6 - Verificar instalación:

Escribe choco en la terminal para ver que está instalado y obtener la ayuda con

~~~~
choco -?
~~~~

![Comando choco versión](./img/img_chocolatey/7_choco_version.png)
<br><br>



### 2. Instalación de Programas
<br>


1 - Buscar paquetes para instalar:

Usa el comando para buscar paquetes. Espera a que termine la instalación.

![Comando copiado firefox](./img/img_chocolatey/8_copiar_comando_firefox.png)
<br><br>




2 - Instalar paquetes. Para instalar un programa, usa:

~~~~
choco install firefox
~~~~

![Comando ejecucion firefox](./img/img_chocolatey/9_copiar_comando_firefox_cmd.png)
<br><br>



3 - 🎉 ¡Listo! Con estos método esta correctamente instalado

![Firefox instalado](./img/img_chocolatey/10_firefox_instalado.png)