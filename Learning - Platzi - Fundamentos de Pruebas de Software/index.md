# Fundamentos de Prueba de Software

## Indice
    1. Fuentes
    2. Resumen
    3. Introduccion
    4. Proceso de Prueba y Estandares

## Fuentes
* Platzi : [Platzi - Fundamentos de Pruebas de software](https://platzi.com/clases/1421-pruebas-software/)

## Resumen



## Introduccion

### Que son las pruebas de software?
Las pruebas son el proceso de evaluar un producto, aprendiendo a traves de la exploracion y experimentacion.
### Razones para hacer Pruebas:
* Tenemos un problema o resultado no esperado
* Costo alto o fuera de presupuesto
* Implicaciones legales o de estandares tecnologicos
* Detectar errores antes de que la app se lance a produccion
* Disminuir el tiempo invertido en resolver problemas


## Proceso de pruebas del software y los estándares internacionales

* Metodología: Es donde estableces el criterio o estrategia de cómo se llevaran acabo las pruebas.
* Recursos: Si quieres realizar pruebas y no estás preparado, con el tiempo esas carencias se pueden visualizar como defectos.
* Herramientas: Nos ayudarán a optimizar nuestro trabajo.

## Proceso de pruebas del software: Calidad y Defectos

__Que es la calidad?__

> La calidad es una percepcion entre lo deseado, analisado y entregado.

> La calidad la define el cliente

> Validar el producto respecto a los requerimientos.

> Definir que es la calidad para el cliente

> Segun la I.E.E.E la calidad es el grado con el que un sistema, componente o proceso cumple con los requisitos especificados y las necesidades o expectativas del cliente o usuario.

__Etapa de Verificacion y verificacion__
* Verificación: Es ir en cada etapa revisando que se cumpla lo propuesto por el cliente.
* Validación: Antes de entregar al cliente, validamos que efectivamente el conjunto de requerimientos esta siendo cumplido con lo entregado. 

__Tipos de Inconsistencias:__
* Anomalía :Cualquier insatisfactoria condición. No se puede reproducir, situaciones unicas.
* Defecto: No desempeña funciones. Un problema que se puede reproducir.
* Fallo: Incapacidad dentro de márgenes . Situaciones no asociadas al software, ejemplo corte de internet. Se da segun el contexto del uso.
* Error: Acción humana incorrecta. 

## Principios del testing moderno
7 Principios del Testing Moderno
Los testers podemos comenzar a pasar de ser los dueños de las pruebas de calidad

1. Nuestra prioridad es mejorar el negocio: El producto que se va a entregar al cliente permitirá hacer funcionar el negocio. Si en algún momento no quieres hacerlo, estás poniendo en riesgo ese negocio porque si el producto no se vende o no es aceptado la empresa puede cerrar o puedes perder el trabajo.
2. Nosotros aceleramos el equipo y usamos modelos como Lean Thinking y Teoría de las Restricciones para ayudar a identificar, priorizar y mitigar cuellos de botella en el sistema: Cuando queremos hacer algo, lo queremos hacer perfecto y eso puede ser demasiado. Deberías construir en base a procesos cortos para poder encontrar los defectos de una manera más rápida.
3. Nosotros somos la fuerza para la mejora continua, ayudando al equipo a adaptarse y optimizar para tener éxito, en lugar de proporcionar una red de seguridad para detectar fallas: El cliente puede entender que el producto se va a liberar por fases, es importante que nosotros enfoquemos nuestras pruebas en cada una de esas fases. No tiene que ser todo al inicio y al final, debe haber una distribución que nos permita manejar el riesgo del software
4. Nos preocupamos profundamente acerca de la cultura de calidad en nuestro equipo, y asesoramos, lideramos y nutrimos el equipo para llevarlos a una cultura de calidad más madura: Al inicio los testers eran personas desarrollando software y un día con tantos defectos y trabajo, separaron los roles para que así hubiese una persona dedicada a realizar las pruebas. El tester puede hacer recomendaciones de herramientas, mejorar el proceso o volverse un coach.
5. Nosotros creemos que el cliente es el único capaz de juzgar y evaluar la calidad de nuestro producto: Si el cliente esta satisfecho con lo entregado y cumple las expectativas entonces has alcanzado la calidad deseada.
6. Nosotros usamos datos de manera extensa y profunda para entender los casos de uso del cliente y entonces cerrar huecos entre hipótesis del producto e impacto del negocio.
7. Expandimos las habilidades de testing y el conocimiento en todo el equipo; entendemos que esto reduce o elimina la necesidad de una especialista dedicado al testing.

__Lean Thinking:__ es un sistema enfocado en la creación de valor para el cliente, a través de la persistente búsqueda y eliminación de desperdicio, así como también la mejora continua, el respeto hacia las personas, el trabajo en equipo y abordar desafíos.

__Theory of Constraints:__ en una organización siempre habrán restricciones (maquinaria, procesos, políticas, personas…), en las cuales debemos enfocarnos y atacarlos de la sigueinte manera:

1. Identificar el cuello de botella
2. Explotarlo, llevándolo a su máxima capacidad.
3. Subordinar todo lo demás con el fin de solucionar el cuello de botella.
4. Elevar la capacidad con más maquinaria, personas, etc.
5. Iterar: siempre habrán más restricciones. Se debe evitar la inercia.
.