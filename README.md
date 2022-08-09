# Curso-de-Introducci-n-a-la-Automatizacion-de-Prueba

# La automatización de pruebas
> Es la práctica de ejecutar pruebas de una manera repetible, que permita utilizar la información y los resultados obtenidos para:
* Mejorar la calidad del software.
* Maximizar el retorno de la inversión (ROI).

El valor de la automatización de pruebas ya está probado, por lo tanto las empresas ya las están implementando.

Para comprender mejor la automatización de pruebas, es necesario tener claro las ventajas y desventajas asociadas a ellas. Esto permitirá saber en qué condiciones debemos utilizarlas.
## Ventajas de la automatización de pruebas
Las ventajas que nos ofrece la automatización de pruebas son las siguientes:
> 
* Mejorar la eficiencia de las pruebas.
* Proporcionar una cobertura de pruebas más amplia con respecto a las pruebas manuales.
* Reducir el costo total de las pruebas, es decir, no implicar costos que generarían acciones innecesarias como las pruebas manuales.
* Acortar el periodo de ejecución de las pruebas.
* Aumentar la frecuencia de las pruebas reduciendo el tiempo requerido para los ciclos de prueba.
* Se pueden ejecutar más pruebas por compilación o por liberación.
* La posibilidad de crear pruebas que no se pueden realizar manualmente, como las pruebas en tiempo real o pruebas paralelas.
* Las pruebas están menos sujetas a errores del operador. Una vez que se haya programado, no van a fallar.

## Desventajas de la automatización de pruebasDesventajas de la automatización de pruebas
Las desventajas que nos ofrece la automatización de pruebas son las siguientes:
> 
* Costos adicionales en herramientas, soluciones o profesionales.
* Requiere de conocimientos de programación, lo que implica que sea más difícil de solucionar errores o debuggear.
* Requiere un mantenimiento continuo porque el software evoluciona rápidamente.
* Es necesario agregar tecnologías adicionales en el stack de tu empresa.
* Las pruebas pueden volverse complejas.
* Distracción de los objetivos de la prueba, a veces no se evalúa correctamente lo que se debe automatizar o lo que no.
* Tiempos innecesarios en automatizar pruebas que hubieran sido resueltas más rápido de forma manual.
Contribución creada con los aportes de: Andrés Guano.

## Las limitaciones de la automatización de pruebas
Las limitaciones de la automatización de pruebas se refieren a aquellas cosas que serán difíciles de automatizar, es decir, debes tener claro que no todo se puede automatizar.
Funcionalidades difíciles de probar automatizadamente
A continuación se expondrán ciertas funcionalidades que son difíciles de probar de forma automática:
- Probar la verificación de dos pasos
La verificación de dos pasos (Two Factor Authentication) consiste en enviar un código de seguridad para identificar a un usuario, por lo tanto, por cuestiones de seguridad y de la complejidad que se requiere, no es posible automatizar este procedimiento.
- Probar los sistemas anti-spam
El sistema de reCAPTCHA consiste en verificar que el usuario es una persona y no un robot o un programa.
Usualmente, estas técnicas son usadas por empresas que desean generar spam.
La verificación consiste en seleccionar imágenes relacionadas entre sí o un código, por lo que por su complejidad, no es posible automatizarlo.
- Probar los correos automatizados
La automatización de correos, ya sea para realizar una restauración de contraseña o probar que un correo haya sido enviado correctamente, no es posible en su totalidad.
Existen muchas limitaciones para probar el envío de correos, aunque no es imposible porque hay herramientas que te permiten conectarte a un servidor y observar algunos de los resultados que se desean probar.
Sin embargo, el costo de automatizar estas pruebas puede ser elevado porque es necesario adquirir el servicio de correos.
Por el motivo anterior y el tiempo que es necesario invertir para este tipo de automatizaciones, no es rentable hacerlo.
* Probar los sensores de los dispositivos móviles
Los sensores de los dispositivos móviles son difíciles de probar de manera automatizada, porque su comportamiento es difícil de emular por código.
Por ejemplo, si se quiere imitar el comportamiento del giroscopio, es necesario mover el dispositivo, quizás haya formas de emularlo por código, pero al final no va a ser una prueba que se acerque al uso real de un humano.
Otro ejemplo es escanear un código QR, que para automatizarlo se necesita que el celular esté bien soportado y que la distancia de lectura esté dentro de un rango específico.
Por lo tanto, siempre es importante que puedas analizar los beneficios y riesgos en una prueba automatizada.
## Limitaciones comunes de las pruebas automatizadas
Al momento de pensar en la automatización de pruebas, ten presente las siguientes limitaciones antes de diseñar las pruebas:
Solo se puede probar funcionalidades cuyo resultado sea interpretable por la máquina
Que los resultados sean interpretables por la máquina quiere decir que el criterio de aceptación elegido debe ser medible automáticamente.
Por ejemplo, no se puede medir si el usuario está feliz al usar la aplicación. Lo que sí se puede cuantificar es el color, el número de clics, o si le salió una alerta, entre otros.
Las pruebas automatizadas no reemplazan las pruebas exploratorias
Las pruebas exploratorias son las acciones manuales que realiza una persona. La curiosidad, impredecibilidad e imaginación humana no se pueden automatizar.
La Experiencia de Usuario (UX) no es medible
No se puede medir ni automatizar la experiencia de usuario. Solo es posible recopilar datos para realizar análisis futuros.
Contribución creada con los aportes de: Andrés Guano.

## Pruebas funcionales y no funcionales
* Funcionales: Nos permiten analizar los requisitos comerciales (lo que el cliente va a ver, etc)
* No funcionales: Nos permiten probar las cosas que son necesarias para que el cliente vea y tenga una experiencia agradable. (Rendimiento, seguridad, alacenamiento de datos … etc)
La automatización de pruebas nos permitirá automatizar ambos tipos de pruebas.

## Tipos de pruebas (funcionales y no funcionales)
####  Pruebas unitarias:
pequeños bloques de tu software que puedes ir automatizando y probando una funcionalidad pequeña concreta. Son las más baratas y las hacen los mismos desarrolladores.
#### Pruebas de integración:
nos permite probar bloques en conjunto.
#### Pruebas de humo:
son pruebas que se corren después de una liberación o compilación para asegurar que nada se haya “incendiado” y que todo funciona correctamente.
#### Pruebas de regresión: 
Nos va a servir para garantizar que todo sigue funcionando correctamente cuando incluimos nuevas funcionalidades.
#### Pruebas de APIs:
puedes automatizar pruebas a los endPoints de una API para garantizar que funciona como debe.
#### Pruebas de seguridad: 
su proposito es identificar las vulnerabilidades de seguridad de un sistema (también conocidas como pruebas de Pentesting)
#### Pruebas de rendimiento:
son un tipo de pruebas no funcionales, por que nos permiten evaluar la estabilidad y aseguran que el software funcione adecuadamente.
#### Pruebas de aceptación:
Intentan determinar cual es el resultado esperado del cliente
#### Pruebas de UI:
Son las pruebas de interfaz y nos permiten garantizar que el proyecto interacture como debería. Se pueden hacer por bloques, por funcionalidad o pruebas end-to-end.
________________________________________
## Todas pueden ser agrupadas en tres grupos:
#### Pruebas unitarias
( como desarrollador )
#### Pruebas de API
( desarrollador backend, test automation o QA)
#### Pruebas de UI 
( pruebas end-to-end )



## Un framework
> (marco de trabajo) dará pautas, estructura e incluso buenas prácticas para probar un sistema, lo que provocará seguir un estándar para facilitar el trabajo en equipo.
Algunos de los frameworks más famosos o más usados son:
* Capture/Playback
* Linear Scripting
* Structured Scripting
* Module Based
* Data-driven
* Keyword-driven
* Hybrid
* Behavior Driven Development (BDD)

## Frameworks de pruebas más usados
A continuación se explicarán los frameworks de pruebas más usados:
## Capture/Playback
> El framework Capture/Playback consiste en grabar con una herramienta lo que el usuario ejecuta y reproducirlo como casos de prueba (scripts) grabados.El framework Capture/Playback consiste en grabar con una herramienta lo que el usuario ejecuta y reproducirlo como casos de prueba (scripts) grabados.

#### Las ventajas de capture/playback son:
> 
•	El enfoque captura/reproducción se puede utilizar para el System Under Test (sistema bajo prueba, SUT) en el nivel de una interfaz de usuario y/o API.
•	Es fácil de configurar y usar para alguien sin experiencia previa.
Las desventajas de capture/playback son:
•	Es difícil de mantener, porque es necesario grabar la aplicación cada vez que esta cambie.
•	La implementación de los casos de prueba (scripts) solo puede comenzar hasta que el sistema esté disponible.

#### Linear Scripting
> 
El framework Linear Scripting se asemeja a Capture/Playback, pero se diferencia en que el linear scripting permite observar y manipular el código grabado, mientras que en el Caputure/playback es inaccesible. Algunos autores los agrupan en el mismo tipo.
 
#### Las ventajas de linear scripting son:
•	Se puede utilizar parar probar el sistema a nivel de interfaz de usuario y/o API.
•	Fácil de configurar.
Las desvetajas de linear scripting son:
•	El costo de mantenimiento es lineal, no se pueden reutilizar los scripts, por lo que en productos grandes no es recomendable.
•	La cantidad de esfuerzo es lineal, para cada caso de prueba necesitas un archivo de código.
•	Es difícil de mantener, porque es necesario grabar la aplicación cada vez que cambie.
 #### Structured Scripting 
> 
El framework Structured Scripting permite reutilizar el código de los casos de prueba.
 
#### Las ventajas de structured scripting son:
•	Existe una reducción del mantenimiento, por la reutilización de código.
•	Reutilización de secuencias de comandos.
•	Reducción de costos de construcción y manteniento.
Las desventajas de structured scripting son:
•	Requiere un mayor esfuerzo inicial, tratar de dividir los scripts para que sean reutilizables.
•	El equipo o encargado debe poseer habilidades de programación.
•	Se necesita una buena administración.
#### Module Based
> 
El framework Module Based se basa en módulos relacionados con los principios de la programación orientada a objetos (POO). Los módulos están separados por una capa de abstracción, de tal forma que los cambios puedan ser realizados en las secciones de la aplicación.
 
#### Las ventajas del Module Based son:
•	Escalabilidad, podrás heredar atributos o propiedades en el código siguiendo la programación orientada a objetos.
•	Flexibilidad y facilidad de mantenimiento.
•	Modularización.
Las desventajas de Module Based son:
•	No se tiene flexibilidad en los datos, la información debe estar escrita en el código.
#### Data-Driven
> 
El framework Data-Driven se basa en una estructura semejante a la de Module Based, la diferencia es que maneja entradas de datos al ser ingresados por el usuario, sin la necesidad de tener la información en el código.
Por ejemplo, si se requiere probar un inicio de sesión, no es necesario ir al código y cambiar las credenciales manualmente, sino extraer la información de un archivo de Excel, bases de datos, API, entre otros.
 
#### Las ventajas de Data driven son:
•	Comparado con los frameworks anteriores, el costo se reduce considerablemente, ya que la información es más fácil de manejar.
•	Aumenta la cobertura, porque será más fácil cubrir diferentes escenarios y probar la aplicación con diferentes valores.
•	Flexibilidad de ejecución.
Las desventajas de Data driven son:
•	Esfuerzo adicional para establecer, configurar y mantener las fuentes de datos.
•	Dominio de algún lenguaje de programación.
#### Keyword-Driven
> 
El framework Keyword-Driven consiste en realizar acciones en el código a través de una palabra reservada (keyword). Lo que hará será activar una determinada acción según el procedimiento (step number), por ejemplo en la siguiente imagen observarás que primero se ejecutará un inicio de sesión (login), después un clic en un botón (clickButton) y así sucesivamente.
 
#### Las ventajas de Keyword-driven son:
•	Flexibilidad en la creación de pruebas, porque puedes utilizar cualquier combinación de pasos.
•	Reutilización de código y, por lo tanto, el costo de mantenimiento es menor.
•	No se requiere conocimiento de las secuencias de comando, solo se necesita conocer qué hace cada palabra clave (keyword).
Las desventajas de Keyword-driven son:
•	Incremento de dificultad a medida que se introducen nuevas palabras clave.
•	Complejidad de aprendizaje.
#### Hybrid (Data-driven + Keyword-driven)
> 
El framework Hybrid consiste en una combinación de Data-driven y Keyword-driven, en el cual se tiene la información que desea utilizar en una acción determinada por la palabra clave (keyword) en un determinado paso (step number).
 
#### Behavior Driven Development
> 
El framework Behavior Driven Development (BDD) es un marco de desarrollo impulsado por el desarrollo que contiene un lenguaje sencillo de leer para cualquiera. Normalmente, se utiliza un lenguaje natural Gherkin que consta de tres partes:
•	Given: nos da las precondiciones de la prueba.
•	When: nos da el detonante de la acción.
•	Then: permite validar con un criterio de aceptación.
 
#### Las ventajas de BDD son:
•	Existe una mayor compatibilidad entre historias de usuario y casos de prueba (test cases).
•	Claridad en los casos de prueba.
•	Hay una reutilización de código, porque cada sentencia tiene un componente reutilizable.
•	Es Data-Driven, porque tiene una funcionalidad llamada escenarios outline que permiten guardar información y utilizarla.
Las desventajas de BDD son:
•	Mayor dedicación de tiempo.
•	Mayor tiempo de planificación en la estructura del código y sus sentencias.
•	Conocimiento de Gherkin o similar.

#### El proceso de automatización de pruebas
> consiste en integrar tus conocimientos de automatización, ventajas, desventajas, frameworks con tu flujo de trabajo o el de la empresa.
Ciclo de desarrollo de una aplicación o de una solución automatizada

Este ciclo es muy parecido al proceso que se emplea para el desarrollo de un sistema:
•	Análisis
•	Diseño
•	Desarrollo
•	Test
•	Deploy
•	Evolución
#### ¿Cómo se integra con otras metodologías?
El proceso de automatización de pruebas se integra con otras metodologías, como Scrum, de la siguiente manera:
 
-El análisis de la automatización se basa en el diseño del sistema de desarrollo
-El test requiere del despliegue de la automatización, ya que no es posible probar el sistema si la solución de la prueba no está lista para utilizarla.
¿Cómo se integra con un equipo de pruebas manuales?
El proceso de automatización de prueba se integra con otras metodologías y con pruebas manuales de la siguiente manera:
 
•	El diseño del sistema también va a mejorar el análisis de las pruebas manuales.
•	El despliegue de las pruebas manuales mejorará el análisis de la automatización de pruebas.
Por otro lado, no se podrá realizar una prueba en el sistema sin un despliegue de las pruebas automáticas y manuales. Esto permite desarrollar pruebas más estables y flujos que el negocio necesite.

Existen varias herramientas para la automatización de pruebas, dependiendo para qué las vas a utilizar.
Los siguientes ejemplos son software de código abierto, pero existen aplicaciones de pago que te ofrecerán servicios para mejorar tu desarrollo, como el soporte, configuración, solución de problemas. Por lo que debes ser capaz de evaluar las ventajas y desventajas de una herramienta de pago.
Unit testing
Para pruebas unitarias, algunas herramientas para la automatización de pruebas son:
•	Jest y Mocha: se utilizan con el lenguaje de programación JavaScript
•	React/Vue Testing Library: para pruebas en el frontend
•	Enzyme
 
#### API testing
Para API testing, algunas herramientas para probar endpoints son: Rest assured, Postman, Insomnia.
 
#### Web browser testing
Para Web browser testing, algunas herramientas para interactuar con el navegador son: Selenium, Puppeteer, Playwright, Testcafe, Cypress.
 
#### Mobile testing
Para Mobile testing, algunas herramientas para la automatización de pruebas son: Appium, Detox, Calabash.
 
#### Performance
Algunas herramientas para probar el rendimiento son: Jmeter, Gatling.
 

