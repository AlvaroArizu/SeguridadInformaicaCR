# Comandos 
* nmap -sP 192.168.64.* /192.168.0.* (Para ver todos los equipos conectados)
* netdiscover (Descubir direcciones IP en forma local)
* nmap -sV IP (Info de la IP)
* nmap --script smb-os-discovery.nse -p445 IP (Correr los scripts)
* crackmapexec smb 445 IP (Forma corta)
* nmap -f --script vuln IP
* nmap -p445 -f IP

# Clase 6 - Escaneos especificos en Nmap

### Escaneo general
nmap -sV IP > resul.txt (Paquete)
cat resul.txt


### Comando para ver si los puertos estan abiertos 

* nmap -sS IP > sS.txt
* cat sS.txt

### Escaneo de tipo UDP (No orientado a conexiones)
* nmap -sU IP > sU.txt

### Escaneo que muestra los scrips e info basico
* nmap -sC IP
  
### Escaeneo de ping, para descubir host activos
* nmap -sn IP.0/24

**Direcciones MAC:** muy importante 

### Escaneo para encontrar vulnerabilidades 
* nmap --script vuln IP (Basico)
* nmap -p445 IP (ESCANEO DE PUERTOS)
* nmap -p 1-65535 --script vulners IP (Agresivo)



