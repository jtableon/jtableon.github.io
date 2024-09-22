# Metodologías de software
---

## Metodologías ágiles

Desarrollar productos de software no es una tarea fácil, por lo que existen diferentes metodologías que podemos seguir para este desarrollo. Una metodología es un conjunto de técnicas y métodos que nos ayudan a enfrentar cada etapa de un ciclo de vida. De esta manera, podemos:

- Optimizar el proceso y el producto final.
- Utilizar protocolos guiados para la planificación y el desarrollo.
- Establecer qué hacer, cómo hacerlo y cuándo, a lo largo de todo el proyecto.

Las metodologías tradicionales son realmente útiles para proyectos grandes (en términos de tiempo y presupuesto), pero tienen algunas desventajas para proyectos no tan grandes, o con un plazo cercano, o con requisitos inciertos. Por ejemplo, producen demasiada documentación y están sobreplanificadas.

Para enfrentar estos otros proyectos, muchos equipos han probado metodologías ágiles, que son especialmente adecuadas para proyectos pequeños, que se desarrollan en un corto período de tiempo y con equipos compuestos por menos de 10 personas. Con estas metodologías, promovemos el trabajo en equipo, nuestra propia responsabilidad, las necesidades del cliente y los objetivos de su empresa. La comunicación cara a cara entre los miembros del equipo y con el cliente es muy regular. De esta manera, los miembros del equipo comparten sus progresos y problemas, y reciben una retroalimentación rápida del cliente.

Para cumplir su propósito, el desarrollo ágil realiza pequeños incrementos del proyecto, con una planificación mínima. Cada incremento realiza una iteración completa sobre las etapas del software (requisitos, diseño, implementación, pruebas...), en un corto período de tiempo (generalmente de 1 a 4 semanas), conocido como *timebox*. De esta manera, minimizamos el riesgo general y el proyecto puede adaptarse a muchos cambios a lo largo de su desarrollo. La documentación solo se genera cuando realmente se necesita, y el objetivo es obtener un prototipo funcional después de cada iteración, aunque tenga funcionalidades realmente reducidas.

## 1. El Manifiesto Ágil
El Manifiesto Ágil es una especificación creada en 2001 que reúne los principales principios que una metodología debe tener para permitir que el equipo construya un proyecto de software de manera rápida y enfrentando los cambios que pueda tener en el futuro. Algunos de los principios más importantes son:
- Las personas son el principal factor de éxito de un proyecto. Es mejor crear un buen equipo y permitir que configure su propio entorno de trabajo, que construir el entorno y obligar al equipo a adaptarse a él.
- No debemos producir ninguna documentación a menos que sea necesaria para tomar una decisión de inmediato.
- Debe haber una interacción constante entre el cliente y el equipo de trabajo.
- La capacidad de enfrentar los cambios que el proyecto pueda tener durante el desarrollo es más importante que seguir una planificación rígida desde el principio.
- La principal prioridad es satisfacer al cliente a través de la entrega continua de software funcional.
- La conversación cara a cara es el método más eficiente para transmitir información en un equipo de trabajo.
- Simplicidad.

## 2. Algunas prácticas habituales

Además de los principios recogidos en el manifiesto ágil, algunas metodologías ágiles utilizan ciertas prácticas adicionales. Veamos algunas de ellas.

### **Programación en pareja (PP)**

La programación en pareja es una técnica que ofrece muchas ventajas. Dos programadores trabajan juntos en el mismo ordenador. Uno de ellos escribe el código (conductor) y el otro revisa lo que se escribe (observador). Ambos intercambian sus roles frecuentemente (por ejemplo, cada 30 minutos). El observador se encarga de guiar el trabajo del conductor y de aportar ideas para resolver posibles problemas futuros.

#### Las principales ventajas de esta técnica son:

- Se producen programas más cortos, con menos errores y mejor diseñados (ya que el código debe ser legible para ambos miembros del equipo).
- Es útil para el aprendizaje, si uno de los miembros tiene mucha experiencia y el otro es un novato, o si ambos tienen conocimientos diferentes que pueden intercambiarse.
- Si uno de los miembros deja el equipo, otro puede ocupar su lugar con el apoyo del anterior miembro, de modo que no es necesario modificar los plazos de entrega.
- Hay menos interrupciones durante el proceso, ya que ambos miembros intercambian sus tareas y pueden trabajar de manera más continua.

#### Sin embargo, también tiene algunos inconvenientes:

- Algunos ingenieros prefieren trabajar solos.
- Un novato puede sentirse intimidado si trabaja con alguien más experimentado, y viceversa (los trabajadores con experiencia pueden aburrirse ayudando a un novato).
- Es más costoso (hay que pagar dos salarios por un solo trabajo).
- Puede haber hábitos de trabajo molestos en el equipo.

### **Desarrollo guiado por pruebas (TDD)**

Esta es una técnica que utiliza iteraciones cortas basadas en casos de prueba previamente escritos. De esta manera, cada iteración produce el código necesario para pasar estas pruebas, y una vez que se pasan, se integra este código con el anterior y se optimiza. El proceso es el siguiente:

1. Añadimos una nueva prueba al conjunto actual.
2. Escribimos el código para pasar esta última prueba.
3. Ejecutamos nuevamente el conjunto de pruebas y verificamos que todas se pasen.
4. Refactorizamos el código final para optimizarlo.
5. Volvemos al paso 1.

Es importante tener un conjunto de pruebas unitarias que puedan ejecutarse automáticamente, de modo que podamos añadir más pruebas de vez en cuando y relanzarlas en cualquier momento. Veremos más adelante en este módulo algunas técnicas para definir casos de prueba y conjuntos de pruebas.

La idea principal es definir las pruebas que el sistema debe pasar antes de escribir el código correspondiente, asegurándonos de que la aplicación puede verificarse y definiendo pruebas para cada funcionalidad. De esta manera, evitamos escribir código innecesario (esto es, código que no está asociado a ninguna prueba).

---

## 3. Ejemplos de metodologías ágiles

A continuación vamos ver dos ejemplos de metodologías ágiles que se pueden utilizar para el desarrollo de proyectos completos:
- [Scrum](scrum.md)
- [Kanban](kanban.md)

Scrum es una metodología ágil que se puede utilizar en proyectos complejos. Utiliza procesos iterativos e incrementales, y puede aplicarse tanto a productos de software como a otros ámbitos. Su nombre proviene de la "melé" que realizan los jugadores de rugby.

### **Roles**

Los principales roles en Scrum son:

- **ScrumMaster**, equivalente a un gerente de proyecto, aunque este rol no existe implícitamente en Scrum, ya que el propio equipo de trabajo se autogestiona. Su tarea principal es asegurarse de que el método Scrum se utiliza correctamente y que no hay influencias externas que lo perturben.
- **ProductOwner**, quien representa al cliente, aunque no necesita formar parte de la empresa del cliente. Incluso puede ser alguien del propio equipo de trabajo.
- **Equipo de desarrolladores.**

### **Proceso**

Para comenzar, el equipo de trabajo debe recopilar los requisitos del usuario del cliente (tanto gerentes como empleados que van a usar la aplicación). Las características de la aplicación se recopilan a través de historias de usuario, que básicamente son un conjunto de tarjetas de papel en las que el cliente describe las funcionalidades del sistema. Cada historia debe ser comprensible y concreta, para que el equipo pueda implementarla en pocas semanas. Se les pide a los usuarios de la empresa cliente que escriban lo que esperan de la aplicación. El conjunto completo de historias se recopila en una colección llamada **backlog**. De este backlog, algunas historias formarán finalmente parte de la aplicación (el resto serán descartadas).

A partir de aquí, comenzamos el proceso de desarrollo, basado en iteraciones llamadas **sprints**. Cada iteración dura de 2 a 4 semanas y produce un prototipo o versión operativa del producto. En este incremento, se añaden algunas de las funcionalidades extraídas del backlog. El conjunto de requisitos a añadir en cada iteración se decide en una reunión de planificación, donde el Product Owner elige algunos elementos para añadir, y el equipo decide cuáles se pueden añadir en la próxima iteración. Luego, durante la iteración, el backlog se congela, es decir, no podemos cambiar ningún requisito anterior hasta que comience la siguiente iteración.

Además de la reunión al inicio de la iteración, en Scrum también hay reuniones diarias, donde se discute el estado del proyecto, lo que se ha hecho y lo que está por hacerse. También hay una reunión final al terminar la iteración para revisar la versión o prototipo obtenido.

### **Estimación de tiempo**

A cada historia de usuario en el backlog se le asigna un tiempo, generalmente en horas, días o incluso semanas. Así, el tiempo total estimado de un sprint es la suma de todas las historias de usuario seleccionadas para ese sprint.

Para determinar si el tiempo estimado total difiere mucho del tiempo real, podemos usar algunas herramientas adicionales, como los **gráficos de quemado** (*burndown charts*), que nos ayudan de manera gráfica a determinar qué medidas se pueden tomar para reducir esta diferencia.

---

## 4. Ejemplo: Kanban

Kanban es otra metodología ágil, que es realmente fácil de aplicar. Su nombre es una combinación de dos palabras japonesas: *kan* ("visual") y *ban* ("tarjeta"), por lo que podemos deducir que el componente principal de esta metodología consiste en usar tarjetas que representan las diferentes tareas que debemos completar en el proceso de desarrollo.

Los orígenes de la metodología Kanban se remontan a más de 60 años. A finales de la década de 1940, Toyota comenzó a optimizar sus procesos de ingeniería, basándose en el mismo modelo que utilizaban los supermercados para optimizar su stock. Dado que los niveles de inventario debían coincidir con los patrones de consumo, el exceso de stock podía (y debía) controlarse. De este modo, Toyota pudo alinear sus niveles de inventario con su consumo real de materiales. Los trabajadores pasaban una tarjeta entre equipos cuando un contenedor de materiales se había vaciado, indicando la cantidad exacta de material necesario. El almacén tenía listo un nuevo contenedor de material para entregar a la fábrica, y luego enviaban una nueva tarjeta Kanban al proveedor para que suministrara un nuevo contenedor.

Aplicado a los procesos de desarrollo de software, Kanban permite a los equipos ajustar la cantidad de trabajo en curso (WIP) a la capacidad del equipo. Esto da a los equipos opciones de planificación más flexibles, una salida más rápida y un enfoque más claro.

### **Proceso**

El término general para referirse a la metodología Kanban es **flujo**, ya que el trabajo fluye continuamente a través del sistema en lugar de estar organizado en bloques de tiempo, como hace Scrum con sus sprints.

Kanban utiliza mecanismos visuales, como los tableros Kanban, para que los miembros del equipo puedan ver el estado de cada tarea en cualquier momento. Estos tableros pueden ser físicos y/o virtuales.

### **Tablero Kanban**

La función principal del tablero Kanban es asegurar que el trabajo del equipo sea visualizado y que cualquier bloqueo o dependencia sea detectado inmediatamente. El tablero más básico tiene tres secciones (Por hacer, En progreso y Hecho), pero podemos añadir tantas columnas y estados como necesitemos en nuestro caso particular.

Cualquier sección o columna de un tablero Kanban puede llenarse con tarjetas Kanban. Estas reflejan información crítica sobre un elemento de trabajo particular, proporcionando al equipo información sobre quién es responsable de esa tarea, una breve descripción del trabajo a realizar y una estimación de cuánto tiempo tomará.

### **Principios**

Algunos de los principales principios de la metodología Kanban son:

- **Trabajo en progreso limitado**, o "deja de empezar y empieza a terminar", es decir, el equipo no debe empezar otra tarea hasta que la actual haya sido terminada.
- **Calidad garantizada**: todo debe salir bien a la primera, no hay margen de error. De esta manera, la velocidad no es tan importante como la calidad, ya que corregir errores puede ser costoso.
- **Reducción de desperdicio**: debemos hacer solo lo que necesitamos y hacerlo bien.
- **Flexibilidad**: el siguiente paso se decide a partir del backlog, eligiendo la siguiente tarea a completar. Así, podemos priorizar la tarea elegida según las necesidades de cada momento concreto.

---

## **Kanban vs Scrum**

Kanban tiene algunas similitudes con la metodología Scrum, ya que ambas son metodologías ágiles: ambas requieren equipos colaborativos y autogestionados, y ambas se centran en liberar software con frecuencia. Sin embargo, hay algunas diferencias importantes entre ellas:

| Kanban               | Scrum                        |
|----------------------|------------------------------|
| No tiene roles prescritos | ScrumMaster, ProductOwner... |
| Entregas continuas      | Sprints en bloques de tiempo   |
| Se pueden hacer cambios en cualquier momento | No se permiten cambios durante el sprint |

Ambas metodologías pueden aplicarse al mismo tiempo. Scrum es más adecuado para dar retroalimentación al equipo y para la planificación a corto plazo, mientras que Kanban puede usarse para el trabajo diario o en entornos con un alto grado de variabilidad en las prioridades.

### **Ejercicio 2:**

En este video tienes un ejemplo de la metodología Kanban. Intenta responder a estas preguntas después de verlo:

- ¿Cuál es la función principal de los límites de WIP? ¿Qué sucede cuando intentamos mover una tarea a una columna que excede este límite?
- ¿Cómo se pueden combinar Kanban y Scrum? ¿Cuál es el propósito principal de añadir Scrum a Kanban?
