# Elaboración de diagramas de clases

- [Diapositivas](http://jamj2000.github.io/entornosdesarrollo/5/diapositivas)
- [Actividades](http://jamj2000.github.io/entornosdesarrollo/5/actividades)

## Introducción

En esta Unidad aprenderemos a:

- Identificar las herramientas para la elaboración de diagramas de clases.
- Interpretar el significado de diagramas de clases.
- Generar código a partir de un diagrama de clases.
- Generar un diagrama de clases mediante ingeniería inversa.



## UML

**Lenguaje de modelado unificado**

- Es un lenguaje visual de propósito general para representar **modelos**.
- Pretende proporcionar una forma estándar de representar el diseño de un sistema.
- Dispone de numerosos tipos de diagramas.
- Cada tipo de diagrama muestra un aspecto diferente del modelo.
- Actualmente disponible la versión 2.5. Existen algunas diferencias respecto a las versiones 1.x.


###  UML: Tipos de diagramas (I)

- **diagramas de estructura** (aspecto estático)
- **diagramas de comportamiento** (aspecto dinámico)


### UML: Tipos de diagramas (II)

![Tipos de diagramas](http://jamj2000.github.io/entornosdesarrollo/5/assets/uml-diagrams.png)


### UML: Diagramas de estructura

Los más utilizados son:

- Diagramas de clases
- Diagramas de paquetes
- Diagramas de componentes
- Diagramas de implementación



## Diagramas de clases


![Diagrama introductorio](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-diagram-domain-overview.png)


### Clases

![Clase](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-no-compartments.png)

![Clase con compartimentos](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-compartments-impl.png)


### Objetos

![Objeto anónimo](http://jamj2000.github.io/entornosdesarrollo/5/assets/object-anonymous.png)

![Objeto](http://jamj2000.github.io/entornosdesarrollo/5/assets/object-named-slots-value.png)


### Interfaces

![Interface](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-interface.png)

![Interface con compartimentos](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-interface-compartments.png)


### Relaciones

- Asociación
    - Agregación
    - Composición
- Dependencia
- Generalización
- Realización


#### Asociación

![Asociación](http://jamj2000.github.io/entornosdesarrollo/5/assets/association.png)

![Instancia de asociación](http://jamj2000.github.io/entornosdesarrollo/5/assets/link.png)

![Nota](http://jamj2000.github.io/entornosdesarrollo/5/assets/core-comment-note.png)


#### Agregación

![Agregación](http://jamj2000.github.io/entornosdesarrollo/5/assets/shared-aggregation.png)


#### Composición

![Composición](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-composition.png)

![Composición opcional](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-composition-optional.png)


#### Dependencia

![Dependencia de instanciación](http://jamj2000.github.io/entornosdesarrollo/5/assets/instantiate.png)

![Dependencia de uso de clase](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-dependency-usage.png)

![Dependencia de uso de paquete](http://jamj2000.github.io/entornosdesarrollo/5/assets/use-package.png)


#### Generalización (herencia)

![Generalización separada](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-generalizaion-separate.png)

![Generalización compartida](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-generalizaion-shared.png)


#### Realización (implementación de interfaces)

![Realización bola](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-interface-realization-ball.png)

![Realización](http://jamj2000.github.io/entornosdesarrollo/5/assets/class-interface-realization.png)


### Ejemplos


#### Karts

![Karts](https://raw.githubusercontent.com/iesvelez-daw/karts/master/img/kartsUML.png)


#### Videojuego

![Videojuego](https://raw.githubusercontent.com/iesvelez-daw/videojuego/master/img/videojuegoUML.png)


#### Colegio

![Colegio](https://raw.githubusercontent.com/iesvelez-daw/colegio/master/img/colegioUML.png)


#### Zoo

![Zoo](https://raw.githubusercontent.com/iesvelez-daw/zoo/master/img/zooUML.png)



## Diagramas de paquetes


![Diagrama de paquetes](http://jamj2000.github.io/entornosdesarrollo/5/assets/package-diagram-elements.png)



## Diagramas de componentes


![Diagrama de componentes](http://jamj2000.github.io/entornosdesarrollo/5/assets/component-diagram-overview.png)



## Diagramas de implementación (deployment)


![Diagrama de implementación](http://jamj2000.github.io/entornosdesarrollo/5/assets/deployment-diagram-overview-specification.png)



## Software

- Enterprise Architect
- Visual Paradigm
- Microsoft Visio
- Dia, ArgoUML, Umbrello
- Plugins para Netbeans (**easyUML**, plantUML)
- Plugins para Eclipse (...)
- Plugins para IntellJ Idea (...)
- [Lista exhaustiva](https://en.wikipedia.org/wiki/List_of_Unified_Modeling_Language_tools)
