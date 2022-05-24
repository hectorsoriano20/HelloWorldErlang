# Lenguaje Erlang

## Ficha Tecnica

**Propósito:** General.

**Paradigma:** Concurrente, funcional.

**Ventajas:** Toda la parte compleja de la aplicación estaría en el servidor, teniendo el cliente que preocuparse únicamente de comunicarse con el socket java del servidor. Los usuarios no tendrían ninguna limitación a la hora de escoger sus identificadores o a la hora de usar cualquier tipo de caracteres en los mensajes.

**Desventajas:** Es una elección muy buena para servicios altamente disponibles, también es muy bueno en la concurrencia y en la creación de muchos hilos de forma simultánea. Tener un proceso Java en el servidor implica que hay un proceso del cual la estructura de Erlang para la recuperación de procesos no se puede hacer cargo de forma automática. Por otro lado, la creación de hilos en Java suele ser mucho más costosa que la creación de hilos en Erlang, por lo que puede ser un cuello de botella en la velocidad de nuestra aplicación.

**Implementación:** Interpretado, con la opción de ser compilado en el compilador HiPE.

**Runtime / Maquina Virtual:** El entorno de tiempo de ejecución de Erlang (una máquina virtual, muy parecida a la máquina virtual de Java) significa que el código compilado en una arquitectura se ejecuta en cualquier lugar. El sistema de tiempo de ejecución también permite que el código en un sistema en ejecución se actualice sin interrumpir el programa.

**Plataformas soportadas:** BSD, Linux, Microsoft Windows, OSX, Solaris, TRU64, VxWorks.

**Usuarios notables:** Empresas de telecomunicación.

**Historia:** Su creador fue la compañía Ericcson, diseñado por Joe Armstrong, Robert Virding, Mike Williams. Primera versión fue en 1986, versión 1.0. La última versión salió al mercado el 20 de mayo 2021, versión 24.0.1.

**Estado:** Activo

## Pasos para ejecutar el programa

1. Descargar erlang desde [Enlace](https://www.erlang.org/downloads)
2. Agregar el directorio de la carpeta **bin** contenida dentro de la carpeta de Erlang, en los entornos de ejecucion:
a. Click derecho en **Mi equipo**
b. Seleciconar **Propiedades**, luego **Avanzado**, luego **Variables del entorno**, finalmente agregar la ruta al final del apartado **"PATH"**
3. Abrimos el interprete de **comandos**
4. Escribir el comando **erl** para ejecutar erlang en la consola de comandos
5. Escribir el comando **cd ("ruta donde se encuentre el archivo").** para dirigirse al directorio donde tengamos el archivo.
6. Ejecutar el comando **c(Nombre del archivo).** para compilar
7. Ejecutar el comando **Nombre del archivo:start().** para ejecutar el archivo
