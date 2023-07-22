# Comandos 
* nmap -sP 192.168.64.* /192.168.0.* (Para ver todos los equipos conectados)
* netdiscover (Descubir direcciones IP en forma local)
* nmap -sV IP (Info de la IP)
* nmap --script smb-os-discovery.nse -p445 IP (Correr los scripts)
* crackmapexec smb 445 IP (Forma corta)
* nmap -f --script vuln IP
* nmap -p445 -f IP