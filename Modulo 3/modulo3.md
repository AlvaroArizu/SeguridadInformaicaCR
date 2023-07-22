# Introduccion a nmap
* Definicion
* Network Mapper

Es una herramineta de codigo abierto, se utiliza para realizar escaneos de puertos y servicios
Se utiliza para evaluar la seguridad en sistemas informaticos, asi como para descubur equipos dentro de una red informatica.

Informacion tras ciertos escaneos
* Detectar dispositivos conectados a la red
* Detectar puertos abiertos y los servicios que esta corriendo
* Detecta versiones de los servicios
* Detecta firewalls o paquetes bloqueados 
* Puede hacer evasiones defirewalls

Para poder detectar si un servicio esta corriendo, nmap realiza un intento de conexion aun puerto en especifico

Nmap utiliza una tabla de puertos comunes, e intenta conectarse a cada uno de ellos, partiendo de un determinado rango de direcciones IP.

## Network Mapper
Nmap entre sus funciones crea mapas de red, estos se generan cuando lanzamos algun tipo de escaneo. Nmap tiene posibilidad de identificar diversos datos que resultan de utilidad para un auditor en seguridad informatica

## Conexiones de 3 pasos 
1. El host A, envia un paquete SYN para abrir la conexion al host B
2. Recibe un paquete con los flags SYN y ACK activos
3. Responde con un flags ACK al host B

**Una vez se cumple los 3 pasos la conexion queda establecida**

## Deteccion de un sistema operativo
Realizar la deteccion de un firewall no es una tarea sencilla, debido a que nmap realiza su trabajo con normalidad y recibe una respuetsa negativa de todos los puertos.

Esto quiere decir que los puertos pueden estar de 2 formas
* Los puertos estan cerrados
* Los puertos estan siendo bloqueados por un firewall

## Evasion del Firewall
Paro poder evadir un firewall nmap tiene diversas opciones, la mas comun es la ejecucion de escaneos con fragmentacion de paquetes.

Al enviar un paquete fragmentado pued eobtenerse una respueta diferente, que en este caso se busca sea positiva.

## Deteccion del sistema operativo
Para detectar los sitemas operativos actuales podemos usar un SCRIP que obtiene la info mediante el puerto 445

```nmap --script smb-os-discovery.nse -p445 192.168.1.83```

### Comando 
* netdiscover
* nmap -sV "PUERTO IP"
* crackmapexex smb "PUERTO IP"
* nmap -R
* nmap -F
* nmap -f --script vuln
* nmap -p445 -f -sV

# Scripting con nmap
## Que es scripting engine?
Se trata de una potente funcion de nmap que permite la ejecucion de scripts para realizar de forma automatica diversas tareas

## Incorporaciones recientes
Nmap en sus ultimas actualizaciones ha incorporado diversos scripts entre los que podemos mencionar"
* Descubrimiento de red
* Deteccion de servicios mejorada
* Detteccion de vulnerabilidades

## Alcance de scripting engine
Estos scripts nos permiten de una forma muy comoda tanta prepararnos, para:
 1. Prevenir una posible intrusion
 2. Identificar si a hemos sufrido

## Version de nmap disponible 
* https://nmap.org/

## Uso de scripting engine
Dentro del sitio de nmap, cuenta con info de los diversos scripts que tenemos disponibles 

* https://nmap.org/nsedoc/
  
Categorias de scripting enige:
1. Discovery
2. Exploit
3. vuln 

Para poder utilizar los scripts de nmap debemos mandar a llamar a dicho motor de la siguiente manera:

    Nmap --script smb-os-discovery.nse -p445 DIRECCION IP

