# Índice

#### [Introducción](#introduccion)
#### [Herramientas de desarrollo](#herramientas)
#### [Entornos integrados de desarrollo](#IDE)



<pre>
</pre>


<pre>
</pre>


# [Introducción](#indice) 
1. ¿Para que sirve un compilador? ¿Qué tipo de archivo obtenemos tras compilar?
<hr>

2. ¿Para que sirve un enlazador? ¿Qué tipo de archivo obtenemos tras enlazar?
<hr>

3. ¿Para que sirve un interprete? ¿Obtenemos algún archivo tras interpretar?
<hr>

4. Explica cada uno de los siguientes conceptos e indica la relación entre ellos.
 
 - código fuente
 - código objeto
 - código binario
<hr>

5. ¿Qué tipo de código es el `bytecode` generado por el compilador de Java?
<hr>


<pre>
    
    
</pre>
    

# [Herramientas de desarrollo](#indice) 

1. Ejecuta el programa "Hola mundo" en los siguientes lenguajes:
 
 - bash
 - python
 - php
 - javascript (nodejs)
 - c
 - c++
 - java
 - ruby
 - go
 - rust
 - lisp
 - ensamblador (nasm)

 Los paquetes a instalar en Ubuntu son: `python`, `php`, `nodejs`, `gcc`, `g++`, `openjdk-8-jdk`, `ruby`, `golang`, `rustc` , `clisp` y `nasm`.

 El código fuente para algunos lenguajes de programación está disponible en:
 https://es.wikipedia.org/wiki/Hola_mundo#Ejemplos

 Instrucciones en https://github.com/jamj2000/HolaMundo.
<hr>
 
2. Para cada uno de los lenguajes anteriores, indica el proceso realizado para conseguir ejecutar el código: ¿compilación o interpretación?
<hr>

3. Para cada uno de los lenguajes anteriores, indica el nombre del compilador o interprete utilizado en GNU/Linux.
<hr>

4. Investiga y averigua que extensión tienen los archivos de código fuente de los siguientes lenguajes:

  - bash
  - python
  - php
  - javascript
  - c
  - c++
  - java
  - ensamblador
  - ruby
  - go
  - rust
  - lisp
<hr>

5. Scripts ejecutables para los lenguajes interpretados. Edita los scripts para los siguientes lenguajes:

  - bash
  - python
  - php
  - javascript
  - java
  - ruby
  - go
  - rust
  - lisp

  Instrucciones en https://github.com/jamj2000/HolaMundo.
<hr>

6. ¿Qué extensión tienen los archivos de código objeto?
<hr>

7. Lenguaje C. Código en varios archivos. Obtener el código objeto a partir del código fuente de los 3 archivos siguientes:

 ```c 
 //-------------
 // datos.c
 //-------------

 char *mensaje="Hola a todos y todas";
 int  num1 = 8;
 int  num2 = 10;
 ```

 ```c
 //-------------
 // suma.c
 //-------------

 int suma (int a, int b) {
     return a + b;
 }
 ```

 ```c 
 //-------------
 // main.c
 //-------------

 #include <stdio.h>

 int suma (int a, int b);

 extern char *mensaje;
 extern int  num1, num2;

 int main(){
     printf("%s\n", mensaje);
     printf("%d\n", suma (num1, num2) );
     return 0;
 }
 ```

 ```bash
 # Para obtener código objeto

 gcc  -c  main.c  datos.c  suma.c 
 ```

 Deberemos obtener 3 archivos:  `main.o`,  `suma.o`  y `datos.o`
<hr>

8. Lenguaje C. Código en varios archivos. Obtener el código binario ejecutable a partir del código objeto de los 3 archivos anteriores:

 ```bash
 # Para obtener código binario

 gcc  -o  programa  main.o  datos.o  suma.o 
 ```

 Deberememos obtener un archivo `programa` binario ejecutable. Si lo ejecutamos obtenemos el siguiente resultado:

 ```
 ./programa
 Hola a todos y todas
 18
 ```
<hr>

9. Lenguaje C++. Código en varios archivos. Obtener el código objeto a partir del código fuente de los 3 archivos siguientes:

 ```cpp
 //-------------
 // datos.cpp
 //-------------
 # include <string>

 std::string mensaje = "Hola a todos y todas";

 int  num1 = 8;
 int  num2 = 10;
 ```

 ```cpp
 //-------------
 // main.cpp
 //-------------
 #include <iostream>

 using namespace std;

 int suma (int a, int b);

 extern string mensaje;
 extern int  num1, num2;

 int main(){
     cout << mensaje << endl;
     cout << suma (num1, num2) << endl;
     return 0;
 }
 ``` 

 ```cpp
 //-------------
 // suma.cpp
 //-------------
 int suma (int a, int b) {
     return a + b;
 }
 ```
 
 ```bash
 # Para obtener código objeto

 g++  -c  main.cpp  datos.cpp  suma.cpp 
 ```

 Deberemos obtener 3 archivos:  `main.o`,  `suma.o`  y `datos.o`
<hr>

10. Lenguaje C++. Código en varios archivos. Obtener el código binario ejecutable a partir del código objeto de los 3 archivos anteriores:

 ```bash
 # Para obtener código binario

 g++  -o  programa  main.o  datos.o  suma.o 
 ```

 Deberememos obtener un archivo `programa` binario ejecutable. Si lo ejecutamos obtenemos el siguiente resultado:

 ```
 ./programa
 Hola a todos y todas
 18
 ```
<hr>

11. Bibliotecas. Define que se entiende por biblioteca o librería y los tipos que existen.
<hr>

12. Bibliotecas. ¿Qué tipo es el más utilizado actualmente? ¿Por qué?

  Más información en https://github.com/jamj2000/Bibliotecas
<hr>

13. Bibliotecas. Crea una biblioteca dinámica en C que proporcione las funciones para sumar, restar, multiplicar y dividir 2 números enteros.
Crea un programa que haga uso de ella y comprueba que se ejecuta correctamente.

  Instrucciones en https://github.com/jamj2000/Bibliotecas
<hr>

14. Bibliotecas. Crea una biblioteca dinámica en Java que proporcione las funciones para sumar, restar, multiplicar y dividir 2 números enteros.
Crea un programa que haga uso de ella y comprueba que se ejecuta correctamente.

  Instrucciones en https://github.com/jamj2000/Bibliotecas
<hr>

15. Bibliotecas. Busca información y explica las ventajas y desventajas de usar bibliotecas estáticas.
<hr>

16. Bibliotecas. Busca información y explica las ventajas y desventajas de usar bibliotecas dinámicas.
<hr>

17. Build. Automatiza el proceso de compilación de ejecutable y biblioteca, su enlazado y la generación del archivo ejecutable para código fuente en C con make. Haz uso de un buildfile.    

  Instrucciones en https://github.com/jamj2000/Bibliotecas/blob/master/Build.md 
<hr>

18. Build. Automatiza el proceso de compilación de ejecutable y biblioteca, su enlazado y la generación del archivo .jar para código fuente en Java con Ant. Haz uso de un buildfile.    

  Instrucciones en https://github.com/jamj2000/Bibliotecas/blob/master/Build.md 
<hr>

19. Build. Automatiza el proceso de compilación de ejecutable y biblioteca, su enlazado y la generación del archivo .jar para código fuente en Java con Maven. Haz uso de un buildfile.    

  Instrucciones en https://github.com/jamj2000/Bibliotecas/blob/master/Maven.md 
<hr>
 
20. Build. Automatiza el proceso de compilación de ejecutable y biblioteca, su enlazado y la generación del archivo .jar para código fuente en Java con Gradle. Haz uso de un buildfile.    

  Instrucciones en https://github.com/jamj2000/Bibliotecas/blob/master/Gradle.md 
<hr>
 
21. CMake. Automatiza el proceso de compilación de ejecutable y bibliotecas, su enlazado y la generación del archivo ejecutable para código fuente en C++. Crea un buildfile con CMake.   

  Instrucciones en https://github.com/jamj2000/Bibliotecas/blob/master/CMake.md
<hr>

<pre>

 
</pre>

# [Entornos integrados de desarrollo](#indice) 

1. Instala el editor sublime text. Saca una captura de pantalla una vez instalado.
<hr>

2. Personaliza Sublime text instalando los complementos más importantes. 

  Consulta la página https://www.genbetadev.com/desarrollo-web/10-packages-de-sublimetext-para-desarrolladores-web
<hr>

3. ¿Para que sirve el complemento __Emmet__? Haz uso de él al escribir un archivo html de prueba.
<hr>

4. Instala el editor Visual Studio Code. Saca una captura de pantalla una vez instalado y funcionando.
<hr>
 
5. Haz una comparativa de la funcionalidad ofrecida por Sublime text y la ofrecida por Visual Studio Code referente a los siguientes aspectos:

  - terminal integrado
  - emmet incorporado
  - iconos para los tipos de archivos
  - atajo de teclas para comentar (Ctrl+Shift+7)
  - atajo de teclas para buscar y seleccionar (Ctrl+D)
<hr>

6. ¿Qué paquetes básicos debemos instalar en Ubuntu para desarrollar en Java?
<hr>
 
7. Instala el entorno integrado Netbeans. Saca una captura de pantalla una vez instalado y funcionando. 
<hr>

8. Instala el entorno integrado Eclipse. Saca una captura de pantalla una vez instalado y funcionando. 
<hr>

9. Crea un proyecto en Java en Netbeans. Realiza su compilación y ejecución.
<hr>

10. ¿Qué sistema de construcción utiliza Netbeans para generar los archivos "ejecutables"? Mira en el directorio raíz del proyecto
y examina qué _buildfile_ utiliza de los vistos en el tema.
<hr>

11. Crea un proyecto en Java en Eclipse. Realiza su compilación y ejecución.
<hr>

12. ¿Qué sistema de construcción utiliza Eclipse para generar los archivos "ejecutables"? Mira en el directorio raíz del proyecto
y examina qué _buildfile_ utiliza de los vistos en el tema.
<hr> 


 
<pre>


</pre>
