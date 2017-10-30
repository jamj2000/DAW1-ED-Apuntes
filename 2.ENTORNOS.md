
# Entornos integrados de desarrollo

- [Diapositivas](http://jamj2000.github.io/entornosdesarrollo/2/diapositivas)
- [Actividades](http://jamj2000.github.io/entornosdesarrollo/2/actividades)




## Introducción


En esta Unidad aprenderemos a:

- Instalar entornos de desarrollo, propietarios y libres.
- Personalizar y automatizar el entorno de desarrollo.
- Generar ejecutables a partir de código fuente.
- Identificar las características comunes y específicas de diversos entornos de desarrollo.


### Conceptos

- Codigo fuente
- Codigo intermedio u objeto
- Codigo binario
- Bibliotecas (librerías)
- Compilar
- Enlazar (Link)
- Interpretar



## Herramientas básicas


### Lo básico

- Editor de texto: permite escribir código fuente
- Compilador: genera código objeto a partir del código fuente
- Enlazador: agrupa varios archivos objeto en uno binario
- Interprete: lee código fuente y genera código binario para su ejecución


### Bibliotecas (o librerías) (I)

> Conjunto de archivos objeto que extienden la funcionalidad del lenguaje

- __Biblioteca estándar__ del lenguaje
- __Bibliotecas adicionales__


### Bibliotecas (o librerías) (II)

- __Biblioteca estándar del lenguaje C__
  - Entrada y salida por terminal
  - Manejo de archivos
  - Funciones matemáticas
- __Biblioteca estándar del lenguaje Java__
  - Entrada y salida por terminal
  - Manejo de archivos
  - Funciones matemáticas
  - Interfaz gráfica 
  - Red
  - Bases de datos
  - Gráficos (sólo 2D)


### Bibliotecas (o librerías) (III)

- Cada biblioteca está compuesta por varios archivos objeto
- Tipos
  - bibliotecas dinámicas (.DLL o .so) (.jar en Java)
    - muy usadas
  - bibliotecas estática (.LIB o .a)
    - menos usadas actualmente


### Bibliotecas (o librerías) (IV)

- Una biblioteca se compone de 2 partes:
  - Especificación (ofrece una API)
  - Implementación 

__API__ = Interfaz de Programación de Aplicaciones


### Entorno necesario en java

- JRE: necesario para ejecutar programas
  - JVM (inteprete java)
  - Biblioteca estándar
- JDK: necesario para desarrollar programas
  - Herramientas: javac, jar, javadoc, ...


### Construir (Build) (I) 

> Construir (Build) = Compilar + Enlazar

- Dos opciones:
 - Herramientas de construcción
 - Servidor de construcción


### Construir (Build) (II) 
#### __Herramientas de construcción__

  - make, ninja (C, C++)
  - ant, maven, gradle (Java)
  - grunt, gulp (Javascript)
  - rake (ruby)


### Construir (Build) (III) 
#### __Archivos de construcción (buildfiles)__

  - make: __Makefile__
  - ninja: __build.ninja__
  - ant: __build.xml__
  - maven: __pom.xml__
  - gradle: __build.gradle__
  - grunt: __Gruntfile.js__
  - gulp: __gulpfile.js__
  - rake: __Rakefile__


### Construir (Build) (IV) 

- Generadores de archivos de construcción
  - CMake: CMakeLists.txt
  - Meson: meson.build  


### Construir (Build) (V) 

 - Servidores de construcción
  - Jenkins 
  - TravisCI
  - CircleCI
  - Bamboo
  - TeamCity



## Entornos integrados de desarrollo (IDE)


### Ejemplos

- Destinados principalmente a C++:
  - DevC++
  - Microsoft Visual Studio
  - QtCreator
- Destinados principalmente a Java:
  - Netbeans
  - Eclipse
  - IntelJ IDEA
  - Oracle JDeveloper

 
