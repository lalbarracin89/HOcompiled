1. Escriban qué esperan de cada uno de los pasos

Pre-procesador:
	El comando: gcc -E calculator.c -o calculator.pp.c unicamente realizará 
	el primer paso de los 4 pasos de compilacion
	El wrapper analizará cuales librerias son internas y cuales externas
	
Compilacion I:
	gcc -S calculator.c -o calculator.asm 
	Traduce el codigo fuente en lenguaje assembler
		
Compilacion II:
	gcc -c calculator.c -o calculator.o
	Genera el objeto binario del codigo

Linkeo: 
	gcc calculator.o -o calculator.e
	Inserta al programa objeto el código máquina de las funciones de
las librerías en el programa y crea el ejecutable
 

2. ¿Qué agregó el preprocesador?
	Agregó una copia de las librerias internas que serán usadas por el programa
	
3. Identificar en la rutina de assembler las funciones
	call	add_numbers
	call	printf  que no es resuelto en este paso
	
4. Explicar qué quieren decir los símbolos que se crean en el objeto
	U: no esta definido
	T: Texto y es un segmento ejecutable
	En ambos casos al linkear, se resuelven las dependencias.
	
5. ¿En qué se diferencian los símbolos del objeto y del ejecutable?
	El código objeto posee un conjunto de instrucciones y datos escritos
	en binario que es entendido por la computadora. En cambio el código 
	ejecutable reúne diferentes objetos generados por los programadores 
	junto con las librerías propias del lenguaje de programación
	componiendo el programa final. Este es el código que se ejecuta, y 
	es específico para sistema operativo.	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
