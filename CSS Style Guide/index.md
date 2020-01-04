# CSS - Guia de Estilos y Arquitectura

## Indice
1. Fuentes
2. Resumen
2. Organizacion en Archivos
3. Tabla de Contenidos


## Fuentes
* Good Practices : https://cssguidelin.es/#syntax-and-formatting

## Resumen
* Encontrar patrones o componentes comunes en el diseño de tu sitio, y construye tu CSS alrededor de ellos.
* Organizacion en archivos
* Contruir una tabla de contenidos en el CSS
* Utilizar selectores con poca especificidad.
* Evitar encadenar los selectores de clase.



## Organizacion en Archivos
Parte de una buena arquitectura CSS es la organizacion de archivos. Dividir tu archivo CSS en varios archivos facilita la division de tareas en equipos.

Una posible estructura de archivos podria ser:
* typography.css: font faces, weights, line heights, sizes, and styles for 
* headings and body text
* forms.css: styles for form controls and labels
* lists.css: list-specific styles
* tables.css: table-specific styles
* accordion.css: styles for the accordion component
* cards.css: styles for the card component

Los detalles de cómo dividir tu CSS dependerán de tus propias preferencias y prácticas. Si tu flujo de trabajo incluye un pre-procesador como Sass o Less, estos serían parciales con una extensión .scss o .less. También puede agregar un archivo _config.scss o _config.less que contenga variables de color y de fuente.

O quizás tenga un flujo de trabajo más centrado en los componentes, como con la herramienta de biblioteca de patrones Fractal, o con marcos de trabajo JavaScript como React y Vue.js. En su lugar, puede optar por un único archivo base.css o global.css que suaviza las diferencias del navegador, y utilizar un archivo CSS separado para cada patrón o componente.

Algo que hay que evitar: organizar su CSS por página o vista. Los enfoques centrados en la página fomentan la repetición de código y las inconsistencias de diseño; probablemente no necesites tanto la etiqueta .contact-page como las reglas de la etiqueta .home-page. En su lugar, trata de encontrar patrones o componentes comunes en el diseño de tu sitio, y construye tu CSS alrededor de ellos.

El uso de varios archivos durante el desarrollo del sitio no significa necesariamente que vaya a utilizar varios archivos en la producción. En la mayoría de los casos, usted querrá optimizar la entrega de CSS mediante la concatenación de archivos y la separación de los CSS críticos de los no críticos. Discutimos las técnicas de optimización en el capítulo Depuración y Optimización.


## Tabla de Contenidos



CONTENTS

SETTINGS
Global...............Globally-available variables and config.

TOOLS
Mixins...............Useful mixins.

GENERIC
Normalize.css........A level playing field.
Box-sizing...........Better default `box-sizing`.

BASE
Headings.............H1–H6 styles.

OBJECTS
Wrappers.............Wrapping and constraining elements.

COMPONENTS
Page-head............The main page header.
Page-foot............The main page footer.
Buttons..............Button elements.

![Especificidad](\images\Tabla_De_Contenidos_02.JPG)


## Especificidad

### Utilizar especificidad Baja

Errar en el lado del uso de selectores de baja especificidad. Hacen más fácil reutilizar tu CSS, y extienden los patrones de nuevas maneras.
Por lo que a la hora de utilizar selectores debemos utilizar aquellos que sean lo mas bajo posible.

### EVITAR ENCADENAR LOS SELECTORES DE CLASE

Otra forma de minimizar la especificidad es evitar encadenar los selectores de clase. Los selectores como .message.warning tienen una especificidad de 0,2,0. Una mayor especificidad significa que son difíciles de anular. Además, encadenar clases puede causar efectos secundarios. 

Si te encuentras encadenando selectores, vuelve al tablero de dibujo. O bien el diseño tiene inconsistencias o está encadenando prematuramente en un intento de evitar problemas que no tiene. Los dolores de cabeza de mantenimiento que evitará y la reutilización que obtendrá valen la pena.

### EVITAR EL USO DE SELECTORES DE ID
HTML sólo permite que cada identificador (es decir, un atributo id) sea usado una vez por documento. Como resultado, los conjuntos de reglas que usan selectores de id son difíciles de reutilizar. Hacer esto típicamente implica usar una lista de selectores de id - por ejemplo, #sidebar-feature, #sidebar-sports, y así sucesivamente.

Los identificadores también tienen un alto grado de especificidad, por lo que necesitaremos selectores más largos para anular las declaraciones. En el CSS que sigue, necesitamos usar #sidebar.sports y #sidebar.local para anular el color de fondo de #sidebar:

![Especificidad](\images\Especificidad_01.JPG)
