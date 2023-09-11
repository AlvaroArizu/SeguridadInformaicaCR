# Obteniendo meterpreter
### ¿Qué es meterpreter?

Meterpreter es un programa malicioso de tipo troyano que permite a los ciberdelincuentes controlar de forma remota las computadoras infectadas. Este malware se ejecuta en la memoria de la computadora sin escribir nada en el disco.

### ¿Qué es un handler?
Un handler es un “escuchador” y es lo que se utiliza para poder crear la conexión con un payload, o iniciar una conexión hacia un host  en un puerto especifico.

Por lo general el mas utilizado en Kali Linux es el multi/handler

**Un ejemplo de multi handler**

Así es como se aprecia un multi handler configurado:

![](Pic/1.png)

### Obtención de meterpreter
Existen diversas formas de obtener una sesión de meterpreter veamos algunos ejemplos:

* Ofuscamiento de un ejecutable
* Bindeo de un payload
* Creación de un payload con falsificación de permisos
* Ejecución de un .apk (aplica para Android)

# Evasion de antivirus

## Que es msfvenom?
Es un herramienta my util para generar rapidamente shellcode utilizando diferentes cargas utiles(payloads)
## Que es un shellcode
Son un conjunto de ordenes programadas generalmente en lenguaje ensamblador y suelen ser inyectadaas en la pila de ejecucion de un programa para cumplir la instruccion programa

## Encoders disponibles
Son subherramientas para hacer pasar la carga malisiosa

Para poder visualizar los encoders disponibles en msfvenom utilizamos el comando **msfvenom -l encoders**

## Opciones de evasion de antivirus
Hay otras herramientas que suelen ser mas silenciosas al momento de evadir antivirus:
1. Winplayloads https://github.com/nccgroup/Winpayloads
2. Thefatrat https://github.com/Screetsec/TheFatRat
3. Veil-Evasion https://github.com/Veil-Framework/Veil-

## Acciones que deben evitarse 
Es de suma importancia evitar realizar escaneos de muestra en virustotal, debido a que esta plataforma comparte los resultados de los archivos escaneados con las firmas antivirus





















