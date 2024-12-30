# Taller de preparación de ambientes para trabajar con Python

### Instalación de Python
Acá podés [descargar Python](https://www.python.org/downloads/), pueden coexistir varias versiones a la vez en tu sistema operativo. Seguí las instrucciones del instalado (siguiente, siguiente) pero asegurate de marcar la casilla "Add Python to PATH" antes de continuar, si no lo hacés es probable que tengas que hacerlo de forma manual.

- [Usar Python Online](https:///www.online-python.com)

Comprobar las versiones de Python y pip luego de la instalación:
  ```bash
  python --version # Si python no funciona, probar python3
  pip --version # Si pip no funciona, probar pip3
  ```

Listar paquetes instalados:
  ```bash
  pip list
  ```

Congelar versiones de paquetes:
  ```bash
  pip freeze > requirements.txt
  ```

Esto genera un archivo requirements.txt con las versiones de los paquetes instalados.

Instalar paquetes desde un archivo requirements.txt:
  ```bash
  pip install -r requirements.txt
  ```

### Instalación de Visual Studio Code
Acá podés [descargar VSCode](https://code.visualstudio.com/download) y también te recomiendo instalar algunas extensiones: Pylance, Python, Jupyter Notebook y WSL (todas de Microsoft).

- [Usar VSCode](https://vscode.dev/)


### Instalación de Windows Subsystem for Linux
Algunos requisitos a chequear para evitar problemas:
- Tener Windows 10 o superior (no Windows S).
- Activar la virtualización Hyper-V en la BIOS/UEFI.
- Windows Subsystem for Linux y Plataforma de Máquina Virtual activadas en las Características de Windows.

Ejecutar en PowerShell o en CMD con permisos de administrador:
  ```bash
  wsl --install
  ```

Luego de reiniciar la máquina, activamos la versión 2 por defecto:
  ```bash
  wsl --set-default-version 2
  ```

Luego, buscamos Ubuntu o la distro que queramos en el Microsoft Store, ejemplo: Ubuntu 22.04.5 LTS

- [Guía de instalación de WSL](https://learn.microsoft.com/es-es/windows/wsl/install)


### Uso de Virtual Enviroments

Crear un entorno virtual:
  ```bash
  python -m venv nombre_del_entorno
  ```

Activar el entorno virtual:

  ```bash
  nombre_del_entorno\Scripts\activate # En Windows
  source nombre_del_entorno/bin/activate # En Mac/Linux
  ```

Desactivar el entorno virtual:
  ```bash
  deactivate
  ```

### Uso de Notebooks
- [Usar Google Colab online](https://colab.google/)


Instalar Jupyter Notebook en local:
  ```bash
  pip install notebook
  ```

Ejecutar Jupyter Notebook:
  ```bash
  jupyter notebook --open
  ```

