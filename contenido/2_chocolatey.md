# 🚀 Instalación de Programas en Windows con Chocolatey
<br>

- [🚀 Instalación de Programas en Windows con Chocolatey](#-instalación-de-programas-en-windows-con-chocolatey)
  - [📦 1. Chocolatey](#-1-chocolatey)
    - [1.1 Instalación](#11-instalación)

<br>

## 📦 1. Chocolatey
<br>

``Chocolatey`` es un gestor de paquetes para Windows, similar a apt en Linux. Permite instalar y gestionar programas desde la terminal (PowerShell).

<br>

### 1.1 Instalación 
<br>


1 - Ve a la página oficial [Chocolatey](https://chocolatey.org/install) y sigue los pasos .


<br><br>


2 - Abrir PowerShell como administrador:

Busca PowerShell en el menú, haz clic derecho y selecciona "Ejecutar como administrador".


<br><br>


2 - Verificar la política de ejecución:

Para permitir la instalación de scripts, copia y ejecuta este comando para ver tu política actual:

~~~~
Get-ExecutionPolicy
~~~~

<br><br>


3 - Ejecutamos el comando 

~~~~
Restricted
~~~~

<br><br>


4 - Cambiar la política de ejecución:

Cambia la política para permitir la ejecución de scripts firmados (Confirma con ``S`` o ``Y`` según el idioma.):

~~~~
Set-ExecutionPolicy AllSigned
~~~~

<br><br>


5 - 
