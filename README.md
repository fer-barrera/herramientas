<h1 align="center">
🔸 Herramientas 🔸
</h1>
Guia rápida de instalación de herramientas para el desarrollo de aplicaciones con python

## 1. Anaconda.

Anaconda es una distribución de Python que incluye un conjunto de herramientas y bibliotecas preinstaladas, diseñadas para facilitar el desarrollo y la gestión de entornos de programación en ciencia de datos, aprendizaje automático y análisis de datos, proporcionando una instalación simplificada, y gestión de paquetes y dependencias a través de la herramienta conda.

Conda está disponible en dos versiones: una versión completa que incluye numpy, scipy, PyQt, el entorno de desarrollo Spyder, entre otros, y una versión minimalista, conocida como Miniconda, que permite instalar solo los componentes necesarios, según las necesidades del usuario.

### 1.1. Ventajas.

* Conda permite instalar y actualizar paquetes de manera completamente independiente de las bibliotecas del sistema, sin necesidad de modificar los privilegios del usuario. Esta herramienta es particularmente útil cuando no se dispone de permisos suficientes para la instalación de bibliotecas necesarias, ya que instala paquetes binarios en lugar de compilar requerir recursos para su compilación, como sucede con pip.

* Conda simplifica en gran medidad la gestión de dependencias, eliminando las complejidades de compatibilidad entre versiones de paquetes. Esto es esencial cuando se necesitan múltiples versiones de paquetes para una instalación específica.

* Utilizando conda no existe el riesgo de alterar las bibliotecas del sistema, lo que garantiza un entorno estable y seguro para tu desarrollo.

### 1.2. Guia de instalación.

1. Descargue el instalador del siguiente enlace: https://www.anaconda.com/download (912.3M).
   - Para descargar el instalador no es necesario suministrar su dirección de correo electronico, o realizar la suscripción al servicio anaconda cloud.
   - Seleccione la opcion [skip registration](https://www.anaconda.com/download/success).
2. Ejecute el instalador de anaconda teniendo precaución con las siguientes opciones (formularios):
   - Cuando se pregunte por tipo de instalación (installation type), seleccione la opción ''all users'', esta permite instalar anaconda en la raiz del disco, lo cual facilita enormemente su gestión (puede requerir la clave de administrador).
   - Cuando se pregunte por la ruta de instalación (choose install location), escriba: C:\apps\anaconda3
   - Cuando se pregunte por las opciones avanzadas de instalación (advanced installation options), selecciones la opción: “Anaconda” as my “default Python 3.X” environment. Esto habilita el entorno virtual base de anaconda como el interprete por defecto del sistema.
3. Finalice el proceso de instalación.

## 2. Configuración del entorno vistual.

1. Inicie una sesión en la consola de comandos de anaconda, para ello ejecute Anaconda>Anaconda powershell prompt desde el menu de aplicaciones de windows.
2. Cree un nuevo entorno virtual desde la línea de comandos.
```md
conda create --name dl python
```
Teclee [y] para continuar con la instalación.
3. Active el entorno virtual
```md
conda activate dl
```
4. Instalación de OpenCV
```md
pip install opencv-contrib-python
```
Contiene tanto los módulos principales como los módulos adicionales/contribuciones.

https://docs.nvidia.com/cuda/wsl-user-guide/index.html

2. Getting Started with CUDA on WSL 2
To get started with running CUDA on WSL, complete these steps in order:

2.1. Step 1: Install NVIDIA Driver for GPU Support
Install NVIDIA GeForce Game Ready or NVIDIA RTX Quadro Windows 11 display driver on your system with a compatible GeForce or NVIDIA RTX/Quadro card from https://www.nvidia.com/Download/index.aspx. Refer to the system requirements in the Appendix.)

Note

This is the only driver you need to install. Do not install any Linux display driver in WSL.

2.2. Step 2: Install WSL 2
Launch your preferred Windows Terminal / Command Prompt / Powershell and install WSL:

wsl.exe --install
Ensure you have the latest WSL kernel:

wsl.exe --update
2.3. Step 3: Set Up a Linux Development Environment
From a Windows terminal, enter WSL:

C:\> wsl.exe
The default distro is Ubuntu. To update the distro to your favorite distro from the command line and to review other WSL commands, refer to the following resources:
