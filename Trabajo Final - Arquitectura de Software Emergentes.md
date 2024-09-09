**Universidad Peruana de Ciencias Aplicadas**

Ingeniería de Software

Ciclo: VIII

Sección: WS82

Profesor: Royer Edelwer Rojas Malasquez

**INFORME DE TRABAJO FINAL**

**CasaFinder**

Integrantes:

* Carrillo Mainicta, Michael - U20201A924


Setiembre, 2024

---

# Registro de Versiones del Informe

| Versión | Fecha    | Autor            | Descripción de modificación                                                      |
| ------- | -------- | ---------------- | -------------------------------------------------------------------------------- |
| 1.0     | 08/09/24 | Michael Carrillo | Creación del proyecto con Markdown Introducción del proyecto Cap I, II, III y IV |

---

# Contenido
- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Contenido](#contenido)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
        - [MISIÓN](#misión)
        - [VISIÓN](#visión)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1. Antecedentes y Problemática](#121-antecedentes-y-problemática)
        - [ANTECEDENTES:](#antecedentes)
        - [PROBLEMÁTICA](#problemática)
    - [1.2.2. Lean UX Process](#122-lean-ux-process)
      - [1.2.2.1. Lean UX Problem Statements](#1221-lean-ux-problem-statements)
      - [1.2.2.2. Lean UX Assumptions](#1222-lean-ux-assumptions)
        - [CARACTERÍSTICAS](#características)
        - [BUSINESS OUTCOMES](#business-outcomes)
        - [BENEFICIOS DEL USUARIO](#beneficios-del-usuario)
        - [BUSINESS ASSUMPTIONS](#business-assumptions)
        - [USER ASSUMPTIONS](#user-assumptions)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos Objetivo](#13-segmentos-objetivo)
        - [Segmento Clientes](#segmento-clientes)
        - [Segmento Transportistas](#segmento-transportistas)
- [Capítulo II: Requirements Elicitation \& Analysis](#capítulo-ii-requirements-elicitation--analysis)
  - [2.1. Competidores](#21-competidores)
    - [2.1.1. Análisis Competitivo](#211-análisis-competitivo)
    - [2.1.2. Estrategias y tácticas frente a competidores](#212-estrategias-y-tácticas-frente-a-competidores)
  - [2.2. Entrevistas](#22-entrevistas)
    - [2.2.1. Diseño de entrevistas](#221-diseño-de-entrevistas)
    - [2.2.2. Registro de entrevistas](#222-registro-de-entrevistas)
      - [Entrevista N° 1](#entrevista-n-1)
      - [Entrevista N° 2](#entrevista-n-2)
      - [Entrevista N° 3](#entrevista-n-3)
      - [Entrevista N° 4](#entrevista-n-4)
      - [Entrevista N° 5](#entrevista-n-5)
      - [Entrevista N° 6](#entrevista-n-6)
    - [2.2.3. Análisis de entrevistas](#223-análisis-de-entrevistas)
  - [2.3 Needfinding](#23-needfinding)
    - [2.3.1 User Persona](#231-user-persona)
          - [_User Persona Manuel Segura, usuario Cliente_](#user-persona-manuel-segura-usuario-cliente)
          - [_User Persona Manuel Segura, usuario Transportista_](#user-persona-manuel-segura-usuario-transportista)
    - [2.3.2 User Task Matrix](#232-user-task-matrix)
          - [_User Task Matrix del usuario cliente_](#user-task-matrix-del-usuario-cliente)
          - [_User Task Matrix del usuario transportista_](#user-task-matrix-del-usuario-transportista)
    - [2.3.3 Empathy Mapping](#233-empathy-mapping)
          - [*Empathy Mapping del usuario cliente*](#empathy-mapping-del-usuario-cliente)
          - [*Empathy Mapping del usuario transportista*](#empathy-mapping-del-usuario-transportista)
    - [2.3.4. As-is Scenario Mapping.](#234-as-is-scenario-mapping)
          - [*As-is Scenario Mapping del usuario cliente*](#as-is-scenario-mapping-del-usuario-cliente)
          - [*As-is Scenario Mapping del usuario transportista*](#as-is-scenario-mapping-del-usuario-transportista)
  - [2.4. Ubiquitous Language.](#24-ubiquitous-language)
- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
  - [3.1. To-Be Scenario Mapping.](#31-to-be-scenario-mapping)
          - [_To-Be Scenario Mapping del usuario cliente_](#to-be-scenario-mapping-del-usuario-cliente)
          - [_To-Be Scenario Mapping del usuario transportista_](#to-be-scenario-mapping-del-usuario-transportista)
  - [3.2. User Stories.](#32-user-stories)
        - [_Desarrollo de los User Stories_](#desarrollo-de-los-user-stories)
    - [EPICS](#epics)
          - [_Desarrollo de las Epics_](#desarrollo-de-las-epics)
  - [3.3. Impact Mapping.](#33-impact-mapping)
          - [_Impact Mapping de los usuarios cliente y transportista_](#impact-mapping-de-los-usuarios-cliente-y-transportista)
  - [3.4. Product Backlog.](#34-product-backlog)
        - [_Desarrollo del Product Backlog_](#desarrollo-del-product-backlog)
- [Capítulo IV: Strategic-Level Software Design](#capítulo-iv-strategic-level-software-design)
  - [4.1. Strategic-Level Attribute-Driven Design](#41-strategic-level-attribute-driven-design)
    - [4.1.1. Design Purpose](#411-design-purpose)
    - [4.1.2. Attribute-Driven Design Inputs](#412-attribute-driven-design-inputs)
      - [4.1.2.1. Primary Functionality (Primary User Stories)](#4121-primary-functionality-primary-user-stories)
      - [4.1.2.2. Quality attribute Scenarios](#4122-quality-attribute-scenarios)
      - [4.1.2.3. Constraints](#4123-constraints)
    - [4.1.3. Architectural Drivers Backlog](#413-architectural-drivers-backlog)
    - [4.1.4. Architectural Design Decisions](#414-architectural-design-decisions)
    - [4.1.5. Quality Attribute Scenario Refinements](#415-quality-attribute-scenario-refinements)
  - [4.2. Strategic-Level Domain-Driven Design.](#42-strategic-level-domain-driven-design)
    - [4.2.1. EventStorming](#421-eventstorming)
          - [*Step 1: Unstructured Exploration*](#step-1-unstructured-exploration)
          - [*Step 2: Timelines, Step 3: Pain Points, Step 4: Pivotal Points*](#step-2-timelines-step-3-pain-points-step-4-pivotal-points)
          - [*Step 5: Commands, Step 6: Policies, Step 7: Read models, Step 8: External Systems*](#step-5-commands-step-6-policies-step-7-read-models-step-8-external-systems)
          - [*Step 9: Aggregates, Step 10: Bounded Contexts*](#step-9-aggregates-step-10-bounded-contexts)
    - [4.2.2. Candidate Context Discovery](#422-candidate-context-discovery)
    - [4.2.3. Domain Message Flows Modeling](#423-domain-message-flows-modeling)
    - [4.2.4. Bounded Context Canvases](#424-bounded-context-canvases)
    - [4.2.5. Context Mapping](#425-context-mapping)
  - [4.3. Software Architecture.](#43-software-architecture)
    - [4.3.1. Software Architecture System Landscape Diagram.](#431-software-architecture-system-landscape-diagram)
    - [4.3.2. Software Architecture Context Level Diagrams.](#432-software-architecture-context-level-diagrams)
          - [***Diagrama de Contexto de FastPorte***](#diagrama-de-contexto-de-fastporte)
    - [4.3.3. Software Architecture Container Level Diagrams.](#433-software-architecture-container-level-diagrams)
          - [*Diagrama de Contenedores de FastPort*](#diagrama-de-contenedores-de-fastport)
    - [4.3.4. Software Architecture Deployment Diagrams.](#434-software-architecture-deployment-diagrams)
          - [*Cloud Architecture Deployment Diagram*](#cloud-architecture-deployment-diagram)
- [Conclusiones](#conclusiones)
- [Recomendaciones](#recomendaciones)
- [Anexos](#anexos)
  - [Repositorio con Informe](#repositorio-con-informe)
  - [Entrega TB1](#entrega-tb1)

--- 

# Student Outcome

| Criterio específico                                                                                                                                                                    | Acciones realizadas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Conclusiones                                                                                                                                                                                                                                                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.     | **Eduardo Sebastián Lévano Cavero**<br>*TB1* <br>- Durante el video de exposición se transmitió de manera adecuada la problemática hallada en el sector de transporte de mercadería y como se solucionaría por medio de la implementación de una página web para comunicar a transportistas con personas que requieran de sus servicios. Asimismo, se detallo como esta diseñada la propuesta y su sustentación.<br><br>**Anthony Botello** <br>*TB1* <br>- En el vídeo de exposición se indicaron a los competidores, así como también se explicó la matriz DAFO de nuestra organización. Finalmente, se expusieron resultados acerca de las entrevistas realizadas.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- Durante mi exposición, comuniqué de manera clara y objetiva los resultados de mi proyecto en ingeniería, destacando la fase de Needfinding. Presenté User Personas y una matriz de tareas de usuario, usando herramientas como Empathy Mapping y As-is Scenario Mapping. Además, delineé el escenario futuro de la plataforma propuesta, detallando User Stories, Impact Mapping y un Product Backlog completo.<br><br>**Abel Angel Cierto Espiritu**<br>*TB1* <br>- Durante el desarrollo de este primer avance, comunique de manera eficaz el objetivo del diseño al desarrollar la aplicación web. También, detalle acerca de las funcionalidades primarias  que considero que son importantes y definir los atributos de calidad para una buena aplicación es necesaria. Los constraints nos sirven para tener claro las limitaciones del sistema al momento de desarrollar la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, me enfoqué en comunicar nuestros avances y resultados de manera clara y objetiva. Presenté nuestras ideas durante el proceso de Event Storming y facilité discusiones sobre el modelado de flujo de mensajes del dominio. Mi objetivo era asegurarme de que todos los miembros del equipo, independientemente de su especialidad o nivel jerárquico, comprendieran el progreso y las decisiones tomadas en el proyecto.<br><br>  | *TB1*<br>En la exposición de la presente entrega se comunico eficientemente las bases del proyecto desarrollado y el proceso que llevo a corroborar que efectivamente es una solución adecuada para la problemática encontrada. Asimismo, se presentaron las herramientas para utilizadas para las primeras fases de implementación del proyecto y su planteamiento. |
| Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.. | **Eduardo Sebastián Lévano Cavero**<br>*TB1* <br>- Se documento con éxito y de manera adecuada la introducción al proyecto, describiendo la problemática con antecedentes, ilustrando las posibles soluciones y como se busca solucionarlo de una manera más eficiente por medio del desarrollo de la presenta investigación.<br><br>**Anthony Botello** <br>*TB1* <br>- Se redactaron y documentó información y análisis de nuestros competidores y de la misma forma se evidenciaron las entrevistas realizadas y el análisis de ellas. Por otro lado, se definieron los Primary User Stories y los Quality Attribute Scenarios.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- En la elaboración de la primera entrega, me centré en comunicar de manera precisa y objetiva aspectos específicos. Utilizando el concepto de Ubiquitous Language, desarrollé un lenguaje común que facilitó la comprensión entre los miembros del equipo y los stakeholders. Además, identifiqué las limitaciones (Constraints) del proyecto y elaboré un Architectural Drivers Backlog para guiar el diseño arquitectónico. <br><br>**Abel Angel Cierto Espiritu** <br>*TB1* <br>- Los resultados de elegir drivers de arquitecturas permite un buen funcionamiento en la escalabilidad y mantenimiento del sistema. Por último los escenarios de los atributos que se requiere refinar permite una mejora continua en la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, utilicé herramientas como EventStorming para explorar y descubrir los contextos relevantes. Luego, modelé los flujos de mensajes del dominio para comprender las interacciones entre los diferentes componentes del sistema. Utilicé Bounded Context Canvases para delinear los límites y responsabilidades de cada contexto, y realicé un mapeo de contextos para visualizar las relaciones entre ellos. Finalmente, documenté nuestra arquitectura de software utilizando varios diagramas, incluidos contexto, contenedor y despliegue, para comunicar nuestra visión de manera efectiva a todas las partes interesadas. | *TB1*<br>En el informe se detalló los aspectos más importantes acerca de la base de la solución propuesta y las herramientas que se usaron para validar la misma. Por otro lado, se incluyeron los diagramas adecuados para cada sección con su respectiva descripción para brindar la mayor cantidad de información.                                                |

---

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

Somos un grupo de estudiantes de la Universidad Peruana de Ciencias Aplicadas y en conjunto identificamos una oportunidad de negocio relacionada con el sector transporte, precisando en el transporte de mercadería.

Nos dimos cuenta de que conseguir transporte de carga, mudanza, envío de paquetes, etc., cuando eres un cliente que necesita de ese servicio, no es muy práctico y sencillo, ya sea por diversas razones: no contar con ese tipo de contactos, no saber dónde buscar, confiabilidad, entre otros. Todo esto hace que la situación se complique cuando un cliente normal, un usuario del día a día que necesite servicios de este rubro, se vea limitado en opciones. Por otro lado, sabemos que existen transportistas independientes que brindan el servicio de movilidad particular ya sea para diferentes rubros y que no tienen la oportunidad de llegar a más personas que las de su propio entorno, lo que hace poco variado su lista de clientes y por ende limita su círculo de trabajo.

Por lo anterior expuesto, hemos creado FastPorte, una plataforma que conecta transportistas de los rubros de carga, mudanza, envío de paquetes, etc. con personas (clientes o personas naturales) que requieren de sus servicios. Funcionará de la siguiente manera: un transportista se registrará con sus datos personales, completará su perfil, incluyendo sus datos personales, documentación tales como: licencia y permisos, tipo de vehículo y tipo de transporte brinda, cuenta bancaria (la cual la aplicación utilizará para depositarle el porcentaje correspondiente al ser contratado por un cliente) y la región en la que labura. Finalmente, esperará a que un cliente lo contacte. Por otro lado, una persona que requiera de transporte se registrará con sus datos personales, buscará a un transportista por el rubro que necesite, podrá visualizar el tipo de transporte y el vehículo usado por dicho usuario transportista, la zona donde brinda el servicio o hasta dónde puede llegar, así como las reseñas de anteriores clientes que tuvieron el servicio con él y de elegirlo, tendrá que rellenar un formulario con los detalles del viaje y hacer el pago del servicio mediante la aplicación, que estará conectada a un servicio de pagos. Finalmente, el transportista acudirá al lugar acordado.

##### MISIÓN

Hacer la búsqueda de servicio de transporte para traslado de mercadería o paquetes, confiable y seguro para cada usuario.

##### VISIÓN

Convertirnos en el servicio de búsqueda de transportes preferido por los peruanos que cada vez supere aún más las expectativas de cada cliente.

### 1.1.2. Perfiles de integrantes del equipo

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Eduardo Sebastián Lévano Cavero                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------- |
| Mi nombre es Sebastián, tengo 21 años y soy estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Elegí esta carrera porque me fascina crear y diseñar procesos que faciliten procesos complejos. Por ello, cuando tengo un poco de tiempo libre lo uso para relajarme y para aprender más de lo que me apasiona, la programación, se puede decir que es uno de mis hobbies. Además, de la programación también disfruto de jugar vóley, fútbol o algún videojuego con mis amigos. | ![Sebastián Perfil](img/integrantes/sebastian.jpg) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                 | Carrillo Mainicta, Michael       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Estudiante de la carrera de ingeniería de software, actualmente cursando el 9no ciclo. Me considero una persona entusiasta que le gusta aprender y desarrollar nuevas habilidades, lo cual me ha ayudado a adquirir conocimientos en lenguajes como Python, C++ y C#. Así mismo, me apasiona explorar nuevas tecnologías como Realidad Virtual (VR) y Realidad Aumentada (AR) y a su vez buscar soluciones innovadoras con las mismas. | ![Michael Perfil](img/Capitulo_1/integrantes/img_Michael.jpg) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                           | Sabino Ramírez, Rodrigo Alexander              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Estudiante de sétimo ciclo de la carrera de Ingeniería de Software. Me considero una persona proactiva con pensamiento estratégico, con habilidades en el ámbito de la programación y un gran espíritu investigador. Para este proyecto puedo aportar parte de mi conocimiento adquirido en el curso. Además, de las habilidades blandas tales como el trabajo en equipo, comunicación, entre otras. | ![Rodrigo Perfil](img/integrantes/rodrigo.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Villegas Peralta, Branco Alberto             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Estudiante en el octavo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas, me destaco por mi firme compromiso con la excelencia académica, respaldado por una actitud proactiva y una comunicación efectiva. Esta combinación me capacita para abordar desafíos con determinación y encontrar soluciones eficaces de manera constante. Mi capacidad para mantener la empatía y la tolerancia en situaciones diversas me facilita trabajar de manera colaborativa en equipo y adaptarme sin dificultad a diversos entornos. En términos de habilidades técnicas, poseo sólidos fundamentos en desarrollo web, destacándome en HTML, CSS y JavaScript, lo que me permite crear interfaces atractivas y funcionales. Además, mi dominio versátil en lenguajes de programación como C++, Python, Java, SQL y C# me permite afrontar desafíos desde múltiples perspectivas y encontrar soluciones innovadoras en diferentes contextos. | ![Branco Perfil](img/integrantes/branco.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Cierto Espíritu, Abel Angel              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Estudiante en el octavo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas, me encanta la programación y durante el avance de la carrera adquirí habilidades en lenguajes de programación como C++, C#, Python, TypeScript, Java y SQL para base datos. Asimismo, aprendí acerca de frameworks como Angular, Vue y el desarrollo de aplicaciones móviles en Flutter. En síntesis, estoy dispuesto a ser parte de este equipo de desarrollo y seguir aprendiendo nuevas habilidades en torno a la arquitectura de software emergentes. | ![Abel Perfil](img/integrantes/abel.png) |

## 1.2. Solution Profile

El producto que proponemos como equipo es FastPorte una aplicación que permite conectar a transportistas con personas que requieran de su servicio. Este proceso se llevará a cabo de manera sencilla, accesible y segura, tanto para el cliente como para los transportistas.

### 1.2.1. Antecedentes y Problemática

##### ANTECEDENTES:

Con respecto a nuestra propuesta, nuestra competencia es la siguiente:

- **Trippy Perú:** Herramienta móvil desarrollada en Perú que permite a los padres registrados el poder visualizar la ubicación en tiempo real de la movilidad de sus hijos.
- **MiCargaApp:** Aplicación peruana que conecta a usuarios con clientes que requieran enviar cargas a partir de una tonelada a cualquier ciudad del país. Permite transportar todo tipo de carga, desde mudanzas hasta líquidos peligrosos.
- **MuberZ:** Es una aplicación para mudanzas pequeñas o de productos específicos como un electrodoméstico en Lima. El servicio puede incluir únicamente el traslado, así como el embalaje y el desembalaje.

##### PROBLEMÁTICA

- **What(Qué)**
  En la actualidad existen diversas aplicaciones que ofrecen el servicio de transporte, sin embargo, la mayoría de estas están enfocadas en el ámbito urbano como: Uber, Didi, Cabify, etc. Nosotros proponemos una solución para el ámbito de mercadería o transporte de carga. De esta manera, facilitaremos tanto para el transportista como el cliente la forma de contactar y gozar de un buen servicio.
- **When(Cuando)**
  La problemática surge al momento en que alguien busca un medio de transporte para el rubro de transporte de mercadería o carga. En muchas ocasiones, solo encontramos servicios de taxi que ofrecen diferentes aplicaciones. Sin embargo, no sabemos dónde buscar cuando requerimos de transporte más grande o de mayor capacidad, ya sea para transportar mercadería en cajas o cantidades mucho más grandes de carga de algún tipo.
- **Where(Dónde)**
  Nuestro servicio se dará a nivel nacional en un futuro, sin embargo, por ahora, y para comenzar, nos consolidaremos en la capital y luego iremos creciendo hacia otras regiones para cumplir con nuestra visión como startup.
- **Who(Quién)**
  **FastPorte** está dirigida a todas las personas que deseen encontrar de manera más rápida y confiable un servicio de transporte de carga según la disponibilidad. Por otra parte, también está dirigido a todos los transportistas que quieran brindar este servicio, ampliar su zona de servicio y atraer a más clientes potenciales a contratarlos para así obtener más ingresos.
- **Why(Por qué)**
  Como mencionamos anteriormente, esta propuesta se plantea por la necesidad de una plataforma en la cual los transportistas particulares ligados al rubro de transporte de carga puedan ofrecer sus servicios y que las personas o clientes puedan ver que tienen opciones y elegir el tipo de servicio que requieren. Además, porque será un espacio donde los trabajadores que se dediquen a transportar ya sean carga, mercadería, paquetes, etc., de forma particular podrán aumentar su público y por ende obtener más ganancias.
- **How(Cómo)**
  Funcionará de la siguiente manera: un transportista se registrará con sus datos personales, completará su perfil, incluyendo sus datos personales, documentación tales como: licencia y permisos, tipo de vehículo y tipo de transporte brinda, cuenta bancaria (la cual la aplicación utilizará para depositarle el porcentaje correspondiente al ser contratado por un cliente), el lugar por donde circula y hasta que trayecto puede llegar, finalmente esperará a que un cliente lo contacte. Por otro lado, una persona que requiera de transporte se registrará con sus datos personales, buscará a un transportista por el rubro que necesite, podrá visualizar el tipo de transporte y el vehículo usado por dicho usuario transportista, la zona donde brinda el servicio o hasta dónde puede llegar, así como las reseñas de anteriores clientes que tuvieron el servicio con él y de elegirlo, tendrá que rellenar un formulario con los detalles del viaje y hacer el pago del servicio mediante la aplicación, que estará conectada a una pasarela de pagos.
- **How much(Cuánto)**
  En el Perú son pocas las clientes que compiten directamente con nosotros ya que la mayoría de las aplicaciones de transporte están enfocadas solo a la mudanza o al transporte de carga pesada mayor a una tonelada. Por lo tanto, seríamos el único startup que abarque el área de transporte de carga sin limitaciones, desde solicitar un miniván para transportar un par de cajas hasta solicitar transporte de carga pesada para mercadería, encargos pesados, etc.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

El servicio de transporte es una actividad fundamental cuando eres un empresario y requieres de este medio para trasladar mercadería o productos. Sin embargo, no solo está relacionado a empresarios, pues podría ser una persona natural quien requiera de este servicio para el transporte de cajas o carga pesada. Hemos observado que existen plataformas que nos brindan información de servicio de transporte, sin embargo, están relacionadas a un sector en específico siendo más específicos en el área urbana. Además, existe una preocupación sobre la confiabilidad y seguridad de la información proporcionada. ¿Cómo podemos desarrollar una plataforma integral que abarque el sector de transporte de carga, proporcionando a empresarios, personas naturales y profesionales de diversos campos un acceso centralizado para adquirir servicios de transporte? ¿Cómo garantizamos la seguridad y confiabilidad de la información ofrecida en esta plataforma?

Los trabajadores del sector transporte son clave para distintos negocios, emprendimientos y clientes, pero es sabido que muchos de ellos suelen tener trabajos eventuales independientes como transportistas de carga, movilidad de personas, servicio de mudanza, etc. Hemos observado que no hay un lugar confiable en el que este grupo de trabajadores pueda ofrecer sus servicios y así ganar un extra o quizá aumentar su demanda y redes de contacto. ¿Cómo podemos empoderar a los trabajadores del sector transporte, que a menudo realizan trabajos independientes, para que ofrezcan sus servicios de manera confiable y generen ingresos adicionales? ¿Qué herramientas y plataformas podríamos desarrollar para facilitar la conexión entre estos trabajadores y un público más amplio, asegurando al mismo tiempo la confianza y calidad en los servicios ofrecidos?

#### 1.2.2.2. Lean UX Assumptions

##### CARACTERÍSTICAS

- Registro de usuarios identificados correctamente (transportista y cliente).
- Visualización de los perfiles de los transportistas. En este apartado deberán subir información relevante para el servicio, así como también fotos de su vehículo.
- Los clientes podrán ver la reputación del transportista que será puntuada mediante estrellas, así como también leerán comentarios recibidos por anteriores clientes que usaron su servicio.
- Para realizar el contrato, los clientes tendrán que llenar un formulario con los siguientes datos del servicio: fecha, hora, lugar, tipo de servicio, origen, destino, cantidad de personas o peso, el monto a pagar y una descripción adicional.
- Se le notificará al transportista de sus solicitudes de servicio y él decidirá si aceptarlas o no.
- Pago del servicio de forma online. (El pago lo recibirá el transportista una vez terminado el trabajo)
- Ver el historial de servicios brindados (transportista) y el historial de servicios contratados (cliente)
- Un foro para formar una comunidad.
- Ver la ubicación en tiempo real del transporte usando la tecnología GPS.
- Elegir el tipo de transporte que necesite el cliente usando filtros.

##### BUSINESS OUTCOMES

- Aumentar las opciones del cliente al elegir el transporte que solicitan.
- Dar seguridad a los usuarios en el proceso de pago y en la elección del transportista.
- Que el transportista reciba un pago seguro y disfrute de nuestro servicio.
- Fomentar el uso de nuestro servicio para conseguir más usuarios.

##### BENEFICIOS DEL USUARIO

- Para el transportista, aumentar la cantidad de personas a las que brinde su servicio y por lo tanto obtener más ganancias.
- Para el cliente, aumentar sus opciones de transporte, así como también poder elegir el servicio referenciándose de los comentarios y puntuación del transportista.
- Para el cliente, evitar la búsqueda del servicio de transporte que necesita en diferentes sitios en internet.
- Para el cliente, estar al tanto del transporte que contrató usando GPS.
- Compartir su experiencia y opinión en un foro.

##### BUSINESS ASSUMPTIONS

- Creemos que los usuarios quieren un lugar seguro donde el transportista y el cliente puedan brindar y adquirir el servicio respectivamente.
- Los transportistas quieren un lugar donde llegar a más personas y aumentar sus ingresos mediante la prestación de sus servicios.
- Nuestros usuarios quieren que la información brindada sea verídica y que el pago sea seguro.
- Estas necesidades se pueden resolver con una aplicación que conecte transportistas con clientes para que adquieran un servicio seguro y de acuerdo con sus necesidades.
- Los usuarios iniciales son transportistas que brinden sus servicios de transporte relacionado a un rubro en particular.
- El valor número 1 que una persona quiere de la aplicación es que sea rápida, confiable y que dé la suficiente seguridad cuando contrate el servicio de transporte.
- Obtendremos clientes a través de anuncios que saldrán cuando una persona busque algún servicio de transporte en internet o cuando un transportista busque en algún sitio web a personas que requieran de su servicio.
- Obtendremos ingresos a través de publicidad no invasiva dentro de la aplicación y mediante una comisión cuando haya algún pago de servicio.
- Mi competencia principal en el mercado será los startups que están relacionadas con el transporte, sin embargo, estas están dirigidas a un público en específico.
- Los venceremos debido a que abarcamos de manera completa el rubro de transporte de carga pesada y mercadería y a la publicidad establecida en sitios de internet claves.
- El mayor riesgo que le puede suceder a la aplicación es que la información sobre un transportista sea errónea o falsa y por lo tanto cause problemas con el cliente cuando se preste el servicio.
- Resolveremos esto cuidando y organizando mejor la información, así como también pidiendo pruebas de la información que un transportista proporciona.

##### USER ASSUMPTIONS

- ¿Quién es el usuario?  
  Las personas que brinden servicio de transporte relacionado a algún rubro y las personas entre 20 a 40 años que requieran de este servicio.
- ¿Dónde encaja nuestro producto en su trabajo o vida?
  Para los transportistas encaja en su trabajo y en el caso de los clientes, en su vida.
- ¿Qué problemas tiene nuestro producto y cómo se pueden resolver?
  Al ser relativamente nuevo, nuestro producto puede enfrentar problemas relacionados a la experiencia de usuario, ya que tendrá varias opciones. Sin embargo, leyendo los comentarios de la comunidad con respecto al producto se podría solucionar de tal manera que actualicemos y optimicemos estas características.
- ¿Cuándo y cómo es usado nuestro producto?
  Nuestro producto será de fácil uso y será usado cuando un cliente necesite del servicio de transporte en el ámbito de carga pesada o transporte de mercadería, siempre y cuando haya un transportista registrado que haga tal servicio.
- ¿Qué características son importantes?
  Que sea de fácil uso, que los call to action sean sencillos de entender y que sea de gran utilidad tanto para el transportista como para el cliente.
- ¿Cómo debe verse nuestro producto y cómo debe comportarse?
  Debe tener una interfaz amigable, sencilla y con los colores adecuados. Tendrá un diseño que trasmita confianza, seriedad y seguridad.

#### 1.2.2.3. Lean UX Hypothesis Statements

-	**Creemos** que proporcionar un medio donde se pueda brindar servicios de transporte, puede aumentar la solicitud de los transportistas que cuentan con poca demanda y ampliar su zona de trabajo
**Sabremos** que hemos tenido éxito
**Cuando** la demanda e ingresos generados por dichos transportistas aumentan y sobrepasan la cantidad aproximada que solían generar antes de brindar sus servicios a través de la plataforma.

-	**Creemos** que proporcionar una plataforma donde una persona, que necesite el servicio de transporte, pueda buscar ofertas de servicio mediante una amplia diversidad de vehículos ofrecidos por los transportistas registrados, y generar confianza en el servicio brindado
**Sabremos** que hemos tenido éxito
**Cuando** el porcentaje de satisfacción de los clientes se vea reflejada en las estadísticas, reseñas y calificaciones que estos brinden a los transportistas una vez recibido el servicio contratado.

-	**Creemos** que utilizar el GPS para rastrear el transporte en tiempo real mejorará la confianza y seguridad de los clientes
**Sabremos** que hemos tenido éxito
**Cuando** la calificación promedio de los transportistas aumente en un 20% en comparación con la línea de base previa a la implementación del GPS.

-	**Creemos** que mostrar la reputación, en base a reseñas y calificaciones, de los transportistas aumentará la confianza y respaldará la fiabilidad en el servicio que brindan
**Sabremos** que es cierto
**Cuando** los ingresos mensuales y la frecuencia de solicitud de servicios por parte del grupo de transportistas con mejor calificación aumenten en un 30% en comparación con los transportistas con una calificación promedio o aquellos que no cuenten con ninguna calificación.

-	**Creemos** que mostrar la reputación de los transportistas aumentará los contratos de aquellos con mejor calificación
**Sabremos** que es cierto
**Cuando** los ingresos mensuales del grupo de transportistas con mejor calificación aumenten en un 35% en comparación con la línea de base previa a la implementación de la reputación.

-	**Creemos** que nuestro producto aumentará las ganancias mensuales de los transportistas independientes
**Sabremos** que estamos en lo correcto
**Cuando** los ingresos reportados por los transportistas el segundo mes de uso aumente en 15%.

-	**Creemos** que tener anuncios en internet, aumentará el número de nuevos de usuarios
**Sabremos** que es cierto 
**Cuando** notemos un incremento mensual del 10% de nuevos usuarios

-	**Creemos** que nuestra aplicación perdurará en el mercado 
**Sabremos** que es cierto 
**Cuando** los usuarios sigan evaluando y calificando el funcionamiento de la aplicación de manera regular durante un periodo de al menos 2 años.

-	**Creemos** que la implementación de una función de seguimiento de rutas personalizadas aumentará la retención de usuarios.
**Sabremos** que es cierto 
**Cuando** observemos que el porcentaje de usuarios que utilizan esta función al menos una vez al mes aumenta en un 15% en   comparación con el mes anterior.

-	**Creemos** que simplificar el proceso de pago y ofrecer opciones de pago adicionales mejorará la satisfacción del usuario.
**Sabremos** que que hemos tenido éxito
**Cuando** la encuesta de satisfacción del usuario muestre un aumento del 20% en la puntuación de satisfacción en los dos meses siguientes a la implementación de estas mejoras.

#### 1.2.2.4. Lean UX Canvas

| **LEAN UX CANVAS**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | **Lean UX Canvas**                                                                                                                                                                                                                                                                                                                                                                                                                                | *Fecha: 04/04/2024* *Iteración: 1*                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Business problem**<br><br>Hemos identificado una necesidad en el mercado de transporte, donde los usuarios buscan opciones seguras y confiables para diferentes tipos de servicios de transporte, como transporte de carga, transporte de mercaderías, carga pesada y más. Al mismo tiempo, existe una oportunidad para trabajadores interesados en ofrecer sus servicios de transporte en una plataforma confiable y rentable.<br><br>¿Cómo podemos desarrollar una plataforma integral que abarque todos los sectores de transporte, proporcionando a empresarios, personas naturales y profesionales de diversos campos un acceso centralizado para adquirir servicios de transporte?<br>                                                                                                                                                                                                                                                                                                                      | **5.Solutions**<br><br>- Aplicación que conecta transportistas con personas que requieran de sus servicios.<br>- Un proceso riguroso de registro para transportistas, que incluye la verificación de documentos y papeles de su vehículo.<br>- Ayuda a los transportistas independientes a aumentar sus ingresos y a encontrar clientes que necesitan transporte.                                                                                 | **2.Business Outcomes**<br>- Expandir las opciones de transporte para los usuarios.<br>- Garantizar la seguridad de los usuarios en el proceso de pago.<br>- Garantizar que los transportistas reciban pagos seguros y protegidos.<br>- Fomentar el uso de nuestro servicio para conseguir más usuarios.                                                                                                                                                                      |
| **3. User**<br><br>Nuestro producto tiene dos tipos de usuarios:<br><br>- Personas con edades comprendidas entre 20 y 40 años que requieren servicios de transporte seguro para diferentes necesidades, como transporte de carga, transporte de mercadería, etc.<br>- Personas que ofrecen servicios de transporte y desean obtener ingresos adicionales utilizando la plataforma                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                                                                                                                                                                                                   | **4. User outcomes & benefits**<br><br>- Para el transportista, aumentar la cantidad de personas a las que brinde su servicio. Así podrá obtener más ganancias y mayores oportunidades de generación de ingresos a través de la plataforma.<br>- Para el cliente, aumentar sus opciones de transporte.  Para elegir entre una amplia gama de servicios de transporte seguros y confiables, informándose a través de comentarios y puntuaciones de los transportistas.<br>     |
| **6. Hypotheses**<br><br>- Creemos que proporcionar un medio donde se pueda brindar diversos servicios relacionados al transporte, puede aumentar la solicitud de los transportistas que cuentan con poca demanda y ampliar su zona de trabajo. **Sabremos** que hemos tenido éxito **cuando** la demanda e ingresos generados por dichos transportistas aumentan y sobrepasan la cantidad aproximada que solían generar antes de brindar sus servicios a través de la plataforma.<br>- **Creemos** que proporcionar una plataforma donde una persona, que necesite el servicio de transporte, pueda buscar ofertas de servicio mediante una amplia diversidad de vehículos ofrecidos por los transportistas registrados, y generar confianza en el servicio brindado. **Sabremos** que hemos tenido éxito **cuando** el porcentaje de satisfacción de los clientes se vea reflejada en las estadísticas, reseñas y calificaciones que estos brinden a los transportistas una vez recibido el servicio contratado.<br> | **7. ¿Qué es lo más importante que      necesitamos aprender primero?**<br> <br>- Necesitamos aprender a implementar métodos efectivos que garanticen de los documentos de los transportistas y evaluar su disposición para cumplir con los requisitos de registro. <br>- Necesitamos aprender a implementar métodos de pago seguros y realizar encuestas o pruebas de usuario para evaluar la disposición de los clientes para utilizarlos. <br> | **8. ¿Cuál es la menor cantidad de trabajo que debemos hacer para aprender la siguiente cosa más importante?**<br><br>- Realizar entrevistas breves con un pequeño grupo representativo de clientes para comprender si prefieren nuestro método de conectar transportistas con aquellos que necesitan sus servicios.<br>- Realizar encuestas breves a un grupo inicial de transportistas para conocer su opinión sobre la idea y si propondrían cambios en algún aspecto.<br> |

## 1.3. Segmentos Objetivo
Dentro de nuestro segmento objetivo, hemos identificado dos grupos de usuarios distintos:
##### Segmento Clientes
- Personas que residen en todo el territorio peruano, lima y provincias, y que necesitan servicios de transporte de mercadería, carga pesada, entre otros.
- Se dirige tanto a hombres como a mujeres cuyas edades están en el rango de 20 a 40 años.
**Características clave:**
- Preocupados por la seguridad y confiabilidad de los servicios de transporte.
- Buscan soluciones convenientes y eficientes para satisfacer sus necesidades de transporte.
- Buscan una amplia gama de ofertas en transporte para así poder elegir la que más se adapte a su necesidad.
**Necesidades y deseos:**
- Acceso a una amplia variedad de opciones de transporte.
- Garantía de seguridad en los servicios y transacciones.
- Facilidad en el proceso de reserva y pago.
- Información detallada sobre los transportistas y sus servicios, incluyendo calificaciones y comentarios.
##### Segmento Transportistas
- Personas mayores de 25 años que ofrecen servicios de transporte de forma independiente y cumplen con los requisitos legales para brindar estos servicios.
- Interesados en ganar ingresos adicionales y aumentar su visibilidad para atraer a más clientes.
**Características clave:**
- Poseen vehículos adecuados y cumplen con la documentación requerida para operar legalmente.
- Buscan oportunidades flexibles para generar ingresos.
- Valoran la retroalimentación positiva y la construcción de una buena reputación en el mercado.
**Necesidades y deseos:**
- Acceso a una plataforma confiable para ofrecer sus servicios de transporte.
- Oportunidades para recibir reservas y aumentar sus ingresos.
- Mecanismos para asegurar el pago oportuno por sus servicios.
- Exposición a una base de clientes más amplia y oportunidades de crecimiento.

---

# Capítulo II: Requirements Elicitation & Analysis
## 2.1. Competidores
### 2.1.1. Análisis Competitivo

![Analisis Competitivo - Tabla](img/Capitulo_2/Competidores/Imagen1.png)

### 2.1.2. Estrategias y tácticas frente a competidores

![Analisis Competitivo - Tabla](img/Capitulo_2/Competidores/Imagen2.png)

## 2.2. Entrevistas
### 2.2.1. Diseño de entrevistas
**Preguntas al segmento cliente:**
-	¿Cuál es tu nombre, qué edad tienes y a qué te dedicas?
-	¿Qué opinas de los servicios de transporte de mercadería en el Perú?
-	¿Alguna vez contactaste con un servicio de traslado de productos? ¿Por qué medio obtuviste el contacto?
    - SÍ ¿Tuviste algún problema con el servicio de traslado de productos que contactaste? ¿Qué pasó? ¿Cómo hizo para solucionarlo?
    - NO ¿Por qué razón?
-	 ¿Qué tan complicado se te hace encontrar un servicio de traslado de productos?
-	 ¿Qué tan a menudo necesitas un servicio de traslado de productos?
-	¿A quién recurres cuando necesitas el servicio de traslado de tus productos?
-	¿Qué tan importante consideras el estar pendiente de la ubicación de tu producto en tiempo real?
-	¿Considera importante conocer el modelo y el año del vehículo que va a trasladar su producto?
-	¿Qué opina acerca de una aplicación que te facilite encontrar un servicio de traslado de productos?
    - El entrevistador explica acerca de la aplicación
-	¿Estaría dispuesto a probarla? ¿Por qué?
-	¿Qué cree que podría mejorar o añadir a nuestra propuesta?

**Preguntas al segmento transportista:**
-	¿Cuál es tu nombre, qué edad tienes y a qué te dedicas?
-	¿Cuánto tiempo lleva trabajando en este empleo o de esta forma?
-	¿Qué opinas de los servicios de transporte de mercadería en el Perú? 
-	¿Qué tan frecuente recibe pedidos para transportar productos? aproximadamente 3-4 veces a la semana
-	¿Hacer servicios de transporte es tu única forma de ingresos o de qué otra forma te ganas el dinero? actualmente si
-	¿Cuánto es lo que gana normalmente en un día de trabajo? entre 100 y 150 depende de los envíos, pero hay varios días que no hay pedidos que movilizar
-	¿De qué manera haces conocer a las demás personas de tus servicios? mayormente me contactan personas que algún contacto les recomendó, también me encuentro en páginas en Facebook
-	¿Tuvo algún inconveniente con sus clientes? ¿Qué pasó? ¿Cómo solucionaron el problema? algunas veces existe el tráfico y algunos clientes no son tan pacientes como otros. pero siempre intento resolver conversando las cosas. 
-	¿Qué opinas de poder contar con una aplicación que te permita encontrar clientes que necesiten de tus servicios como transportista? muy buena ya que es un método en el cual recibiría más clientes. por ejemplo, el servicio de pedido de taxis online cambio totalmente ese rubro y lo convirtió más fácil y seguro para el taxista y el cliente.
    - El entrevistador explica acerca de la aplicación
-	¿Estaría dispuesto a probar nuestra aplicación? ¿Por qué?
-	¿Qué cree que podría mejorar o añadir a nuestra propuesta?


### 2.2.2. Registro de entrevistas
#### Entrevista N° 1
| ![Entevista 1 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista1.jpg)                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Carlos Alipio Sánchez Salazar <br>	Edad: 19 <br>	Distrito: Carabayllo <br>	Segmento: Transportista |

#### Entrevista N° 2
| ![Entevista 2 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista2.png)                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------------- |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Edgard Miranda Lloclla <br>	Distrito: Sullana, Piura <br>	Segmento: Transportista |

#### Entrevista N° 3
| ![Entevista 3 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista3.png)                                                                                           |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Diego Seminario Centeno <br> Edad: 24 años<br>	Distrito: Cercado de Lima <br>	Segmento: Transportista |

#### Entrevista N° 4
| ![Entevista 4 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista4.png)                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Teodoro Geiner Liberato Villanueva <br> Edad: 52 años<br>	Distrito: Huacho <br>	Segmento: Cliente |

#### Entrevista N° 5
| ![Entevista 5 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista5.png)                                                                                                     |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Alexandro Daniel Villarruel Mandujano <br> Edad: 24 años<br>	Distrito: Villa El Salvador <br>	Segmento: Cliente |

#### Entrevista N° 6
| ![Entevista 6 - Evidencia](img/Capitulo_2/Entrevistas/Entrevista6.png)                                                                               |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| <u>**Datos del entrevistado**</u> <br> Nombre y apellidos: Ítalo Paolo Sabino Ramírez <br> Edad: 23 años<br>	Distrito: Callao <br>	Segmento: Cliente |

### 2.2.3. Análisis de entrevistas
![Analisis de entrevistas - Tabla](img/Capitulo_2/Entrevistas/Analisis.png)

## 2.3 Needfinding

### 2.3.1 User Persona

###### _User Persona Manuel Segura, usuario Cliente_

![User Persona Cliente](img/Capitulo_2/Needfinding/1.png)

###### _User Persona Manuel Segura, usuario Transportista_

![User Persona Transportista](img/Capitulo_2/Needfinding/2.png)
### 2.3.2 User Task Matrix
###### _User Task Matrix del usuario cliente_

|                           **Tareas**                            | **Frecuencia** | **Importancia** |
| :-------------------------------------------------------------: | :------------: | :-------------: |
|  Contactar con un transportista para hacer uso de transporte.   |    Siempre     |      Alta       |
|           Saber cuál será el precio por el transporte           |    Siempre     |      Alta       |
|   Conocer los tipos de transporte que ofrece el transportista   |    Siempre     |      Alta       |
|                Hacer un seguimiento del producto                |  Casi Siempre  |      Alta       |
|  Mostrar los transportistas para brindarle opciones al usuario  |  Casi Siempre  |      Media      |
|               Calificar el servicio con estrellas               | Algunas veces  |      Media      |
| Recomendar el servicio proporcionado por medio de un comentario |   Casi nunca   |      Baja       |
###### _User Task Matrix del usuario transportista_

|                         Tareas                         | Frecuencia | Importancia |
| :----------------------------------------------------: | :--------: | :---------: |
|                Contactar con el cliente                |  A menudo  |    Alta     |
|  Acordar cuál será el producto por llevar y el tamaño  |  A menudo  |    Alta     |
|            Acordar el precio con el cliente            |  Siempre   |    Alta     |
|       Establecer el día de llegada del producto        |  Siempre   |    Alta     |
|          Pactar cuál será el lugar de destino          |  Siempre   |    Alta     |
|                Transportar el producto                 |  Siempre   |    Alta     |
| Evidenciar que el producto ha sido entregado con éxito |  A menudo  |    Media    |
|                 Cobrar por el servicio                 |  Siempre   |    Alta     |
|          Atender las solicitudes del cliente           |  Siempre   |    Alta     |
### 2.3.3 Empathy Mapping

###### *Empathy Mapping del usuario cliente*

![Empathy Mapping Cliente](img/Capitulo_2/Needfinding/3.png)

###### *Empathy Mapping del usuario transportista*

![Empathy Mapping Transportista](img/Capitulo_2/Needfinding/4.png)
### 2.3.4. As-is Scenario Mapping. 

###### *As-is Scenario Mapping del usuario cliente*

![As-is Scenario Mapping Cliente](img/Capitulo_2/Needfinding/5.png)
###### *As-is Scenario Mapping del usuario transportista*

![As-is Scenario Mapping Transportista](img/Capitulo_2/Needfinding/6.png)
## 2.4. Ubiquitous Language.

- **Carrier (Transportista)**

Individuo o empresa que proporciona servicios de transporte.

- **Client (Cliente)** 

Individuo o empresa que requiere servicios de transporte.

- **Service type (Tipo de servicio)**

Clasificación de los servicios de transporte ofrecidos, como carga, mudanza, movilidad, etc.

- **Carrier profile (Perfil de transportista)**

Información detallada proporcionada por los transportistas al registrarse, incluyendo datos personales, documentación, tipo de vehículo y servicios ofrecidos.

- **Client profile (Perfil de cliente)** 

Información proporcionada por los clientes al registrarse, incluyendo detalles personales e información de viajes anteriores.

- **Trip form (Formulario de viaje)** 

Formulario completado por el cliente con los detalles del viaje, incluyendo origen, destino, fecha, hora, tipo de carga, etc.

- **Payment (Pago del servicio)**

Proceso mediante el cual el cliente realiza el pago por el servicio de transporte a través de la plataforma FastPorte, utilizando un servicio de pago integrado.

- **Reviews (Reseñas)**

Comentarios y calificaciones dejados por clientes anteriores sobre su experiencia con un transportista específico, ayudando a otros clientes a tomar decisiones informadas.

- **Service area (Zona de servicio)**

Área geográfica donde un transportista está disponible para proporcionar servicios, especificada en su perfil.

- **Service contract (Contrato - Acuerdo de servicio)**

Acuerdo entre el cliente y el transportista cuando se confirma un viaje, estableciendo las condiciones y términos de la prestación del servicio.

- **Vehicle (Vehículo)**

Modo de transporte utilizado por los transportistas para proporcionar servicios.

- **License and permits (Licencia y permisos)**

Documentación legal requerida para que los transportistas operen sus vehículos y proporcionen servicios de transporte.

- **Rates (Tarifas)**

Precios cobrados por los transportistas por sus servicios de transporte.

- **Trip confirmation (Confirmación de viaje)**

Confirmación de una reserva de viaje realizada por el cliente con un transportista.

- **Service status (Estado del servicio)**

Estado actual del servicio de transporte, indicando si está pendiente, en progreso o completado.

- **Transportation request (Solicitud de transporte)**

Solicitud realizada por el cliente para servicios de transporte.

- **Service history provided (Historial de servicios brindados)**

Registro de servicios proporcionados por el transportista.

- **Service history contracted (Historial de servicios contratados)**

Registro de servicios contratados por el cliente.

- **Customer rating (Calificación del cliente)**

Calificación proporcionada por los transportistas para los clientes basada en su comportamiento e interacción durante el viaje.

- **Carrier rating (Calificación del transportista)**

Calificación proporcionada por los clientes para los transportistas basada en su desempeño y calidad del servicio.

- **Trip cancellation (Cancelación de viaje)**

Cancelación de un viaje reservado por el cliente con un transportista.

- **Invoicing (Facturación)**

Emisión de facturas por los servicios de transporte proporcionados.

- **Trip alerts (Alertas de viaje)**

Notificaciones sobre detalles o actualizaciones de viaje enviadas a clientes o transportistas.

- **Shipment tracking (Rastreo de envíos)**

Seguimiento de la ubicación y estado de las mercancías transportadas durante el tránsito.

- **Service tracking (Seguimiento del servicio)**

Seguimiento del progreso y estado de un servicio de transporte.

- **Customer service (Servicio de atención al cliente)**

Soporte y asistencia proporcionada a los clientes con respecto a los servicios de transporte.

- **Availability calendar (Calendario de disponibilidad)**

Calendario que muestra la disponibilidad de los transportistas para proporcionar servicios de transporte.

---

# Capítulo III: Requirements Specification 
## 3.1. To-Be Scenario Mapping. 

###### _To-Be Scenario Mapping del usuario cliente_

![To Be Scenario Mapping Cliente](img/Capitulo_2/Needfinding/7.png)
###### _To-Be Scenario Mapping del usuario transportista_

![To Be Scenario Mapping Transportista](img/Capitulo_2/Needfinding/8.jpg)

## 3.2. User Stories. 

##### _Desarrollo de los User Stories_
![HU-001](img/Capitulo_3/User_Stories/1.png)
![HU-002](img/Capitulo_3/User_Stories/2.png)
![HU-003](img/Capitulo_3/User_Stories/3.png)
![HU-004](img/Capitulo_3/User_Stories/4.png)
![HU-005](img/Capitulo_3/User_Stories/5.png)
![HU-006](img/Capitulo_3/User_Stories/6.png)
![HU-007](img/Capitulo_3/User_Stories/7.png)
![HU-008](img/Capitulo_3/User_Stories/8.png)
![HU-009](img/Capitulo_3/User_Stories/9.png)
![HU-010](img/Capitulo_3/User_Stories/10.png)
![HU-011](img/Capitulo_3/User_Stories/11.png)
![HU-012](img/Capitulo_3/User_Stories/12.png)
![HU-013](img/Capitulo_3/User_Stories/13.png)
![HU-014](img/Capitulo_3/User_Stories/14.png)
![HU-015](img/Capitulo_3/User_Stories/15.png)
![HU-016](img/Capitulo_3/User_Stories/16.png)
![HU-017](img/Capitulo_3/User_Stories/17.png)
![HU-018](img/Capitulo_3/User_Stories/18.png)
![HU-019](img/Capitulo_3/User_Stories/19.png)
![HU-020](img/Capitulo_3/User_Stories/20.png)
![HU-021](img/Capitulo_3/User_Stories/21.png)
![HU-022](img/Capitulo_3/User_Stories/22.png)
![HU-023](img/Capitulo_3/User_Stories/23.png)
![HU-024](img/Capitulo_3/User_Stories/24.png)



### EPICS
Las Epics que identificamos son las siguientes:

###### _Desarrollo de las Epics_

| Código | Título                            | Epic                                                                                                     |
| ------ | --------------------------------- | -------------------------------------------------------------------------------------------------------- |
| EP01   | Registro de información           | Como usuario deseo registrarme dentro de la aplicación para comenzar a usarla.                           |
| EP02   | Registro de información adicional | Como usuario deseo poder almacenar información adicional para recibir/brindar un servicio personalizado. |
| EP03   | Búsqueda de servicios disponibles | Como cliente deseo tener un resultado de búsqueda preciso de los servicios y vehículos disponibles.      |
| EP04   | Contrato del servicio             | Como usuario quiero rellenar la información necesaria para solicitar un servicio.                        |
| EP05   | Seguimiento del servicio          | Como cliente quiero conocer la ubicación del transporte.                                                 |
| EP06   | Informes sobre el servicio        | Como cliente deseo hacer un reporte del servicio dentro de la aplicación.                                |
| EP07   | Forma de pago                     | Como usuario quiero tener una forma de pago dentro de la aplicación.                                     |
| EP08   | Notificación de contratos         | Como usuario quiero notificaciones que me den información de los contratos.                              |
| EP09   | Visualización de perfiles         | Como usuario quiero ver la información que hay en el perfil de un cliente o transportista.               |
| EP10   | Información de contratos          | Como usuario quiero tener la información de mis contratos.                                               |

## 3.3. Impact Mapping. 

Link para una visualización más detallada: [https://drive.google.com/file/d/1Z_48YO0enDocx_Bz8IzVSlgUXCc-bnF5/view?usp=sharing](https://drive.google.com/file/d/1Z_48YO0enDocx_Bz8IzVSlgUXCc-bnF5/view?usp=sharing)

###### _Impact Mapping de los usuarios cliente y transportista_

![Impact Mapping](img/Capitulo_2/Needfinding/9.jpg)
## 3.4. Product Backlog.

##### _Desarrollo del Product Backlog_

| **User Story ID** | **Título**                                  | **Descripción**                                                                                                                                                                             | **Story Points (8/5/3/2/1)** |
| ----------------- | ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------: |
| **HU-011**        | Realizar el seguimiento por GPS             | Como cliente <br><br>Quiero seguir el transcurso del transportista     <br><br>Para sentirme seguro con el servicio                                                                         |            **8**             |
| **HU-007**        | Visualizar la información del transportista | Como cliente <br><br>Quiero observar el perfil del transportista<br><br>Para contratarlo                                                                                                    |            **5**             |
| **HU-008**        | Contratar el servicio                       | Como cliente <br><br>Quiero contratar el servicio<br><br>Para acceder a los servicios del transportista                                                                                     |            **5**             |
| **HU-009**        | Realizar el pago                            | Como cliente <br><br>Quiero realizar el pago del servicio<br><br>Para no tener deudas pendientes                                                                                            |            **5**             |
| **HU-017**        | Notificar del trabajo                       | Como transportista                      <br><br>Quiero que me notifiquen cuando un cliente requiere de mis servicios <br><br>Para no perderme de algún contrato                             |            **5**             |
| **HU-018**        | Informar del contrato propuesto             | Como transportista<br><br>Quiero leer la información del servicio propuesto   <br><br>Para decidir si aceptar el trabajo                                                                    |            **5**             |
| **HU-006**        | Buscar un vehículo                          | Como cliente <br><br>Quiero buscar el tipo de vehículo adecuado<br><br>Para así contratarlo                                                                                                 |            **5**             |
| **HU-022**        | Comentar el servicio brindado               | Como cliente<br><br>Quiero dejar un comentario acerca de mi experiencia con el conductor luego de terminar el servicio<br><br>Para ayudar a los demás usuarios en su elección de conductor. |            **5**             |
| **HU-001**        | Registrar al transportista                  | Como transportista<br><br>Quiero registrarme dentro de la aplicación<br><br>Para navegar dentro de ella                                                                                     |            **3**             |
| **HU-002**        | Registrar al cliente                        | Como cliente<br><br>Quiero registrarme dentro de la aplicación<br><br>Para navegar dentro de ella                                                                                           |            **3**             |
| **HU-023**        | Iniciar sesión como cliente                 | Como cliente<br><br>Quiero iniciar sesión en la aplicación<br><br>Para acceder a los servicios de transporte y gestionar mi perfil de usuario de manera segura y conveniente.               |            **3**             |
| **HU-024**        | Iniciar sesión como transportista           | Como cliente<br><br>Quiero iniciar sesión en la aplicación<br><br>Para acceder a los servicios de transporte y gestionar mi perfil de usuario de manera segura y conveniente.               |            **3**             |
| **HU-020**        | Ver la información del usuario              | Como usuario  <br><br>Quiero visualizar mi perfil y los datos que ingrese en el registro.<br><br>Para corroborar que los datos son correctos                                                |            **3**             |
| **HU-005**        | Editar mi perfil de usuario                 | Como usuario de la aplicación<br><br>Quiero poder editar los datos de mi perfil<br><br>Para mantener mis datos actualizados                                                                 |            **3**             |
| **HU-012**        | Ver el historial de contratos               | Como usuario<br><br>Quiero revisar el historial de contratos <br><br>Para tener un registro                                                                                                 |            **3**             |
| **HU0-013**       | Revisar el servicio                         | Como cliente  <br><br>Quiero decidir revisar el servicio brindado<br><br>Para sentirme más seguro                                                                                           |            **3**             |
| **HU-016**        | Ver el estado del contrato propuesto        | Como cliente <br><br>Quiero saber el estado de mi oferta de trabajo <br><br>Para saber si fue aceptada o rechazada                                                                          |            **3**             |
| **HU-019**        | Reportar una incidencia                     | Como cliente <br><br>Quiero reportar alguna incidencia que haya sucedido <br><br>Para mejorar el servicio dentro de la aplicación                                                           |            **3**             |
| **HU-021**        | Ver el contrato finalizado                  | Como transportista<br><br>Quiero rellenar mi información de pago<br><br>Para recibir el pago correspondiente por el servicio brindado.                                                      |            **3**             |
| **HU-003**        | Registrar un transporte                     | Como transportista <br><br>Quiero almacenar la información de mi transporte y el servicio que ofrezco <br><br>Para que el cliente tenga una noción del servicio que brindo                  |            **2**             |
| **HU-004**        | Registrar su experiencia                    | Como transportista<br><br>Quiero registrar mi experiencia de trabajo <br><br>Para generar confianza al cliente                                                                              |            **2**             |
| **HU-015**        | Guardar los datos de la tarjeta             | Como cliente <br><br>Quiero guardar los datos de mi tarjeta<br><br>Para usarla de manera más rápida en mis siguientes pagos                                                                 |            **2**             |
| **HU-010**        | Cerrar sesión en la aplicación              | Como usuario transportista<br><br>Quiero salir de la aplicación<br><br>Para iniciar sesión en otra cuenta como cliente                                                                      |            **1**             |
| **HU-014**        | Acceder a las preguntas frecuentes          | Como usuario<br><br>Quiero acceder a un banco de preguntas frecuentes sobre la aplicación<br><br>Para despejar dudas que tenga sobre algunos procesos                                       |            **1**             |

---

# Capítulo IV: Strategic-Level Software Design
## 4.1. Strategic-Level Attribute-Driven Design
En este apartado, se presenta una serie de enfoques cruciales en el proceso de Diseño Dirigido por el Dominio a nivel estratégico. Estos enfoques resultaron esenciales para crear una base sólida en la definición y modelado de dominios complejos. A través de metodologías como Event Storming, Context Mapping y la definición de la Arquitectura de Software, se alcanzó una comprensión detallada de los elementos clave necesarios para el desarrollo de sistemas efectivos y bien estructurados. A continuación, se describen los puntos más importantes tratados en esta sección.
### 4.1.1. Design Purpose
El propósito del diseño de CasaFinder es desarrollar una plataforma avanzada que facilite de manera eficiente la conexión entre propietarios de inmuebles y personas que buscan alquilar, ya sea de forma temporal o permanente. Lo que diferencia a CasaFinder es su innovadora integración de la tecnología blockchain, que garantiza la transparencia, seguridad y el cumplimiento de los contratos de alquiler, al tiempo que crea un historial de alquileres inmutable y confiable para ambas partes.
### 4.1.2. Attribute-Driven Design Inputs
Se trata de factores esenciales que orientan el diseño de un sistema o plataforma. Estos atributos son cualidades específicas consideradas cruciales para el éxito del diseño, influyendo en las decisiones tomadas a lo largo del proceso de desarrollo. Los insumos del diseño impulsado por atributos ayudan a establecer los requisitos y prioridades del diseño, además de guiar las decisiones sobre la arquitectura, las funcionalidades y las características del sistema.
#### 4.1.2.1. Primary Functionality (Primary User Stories)
En el diseño de la plataforma, se han identificado varias funcionalidades clave que son esenciales para su operación y eficiencia. Estas incluyen la verificación del historial de cumplimiento de pagos, que permite a los propietarios evaluar la fiabilidad de los inquilinos; un sistema de notificaciones de pagos para mantener a todas las partes informadas y comprometidas; un sistema de pago en línea, que asegura la facilidad y seguridad en las transacciones; y la generación automática de contratos, que facilita la creación y gestión de acuerdos legales entre propietarios e inquilinos. Cada una de estas funcionalidades tiene un impacto significativo en la arquitectura de la solución, requiriendo sistemas robustos y seguros para manejar datos sensibles y proporcionar una experiencia de usuario fluida y confiable. 
Las siguientes historias de usuario se consideran de mayor importancia.

| **Epica / User Story ID** | **Título**                      | **Descripción**                                                                                                                                                            | **Criterios de Aceptación**                                                                                                                                                                                                                                            | **Relacionado con Epica (ID)** |
|---------------------------|---------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------|
| US001                     | Verificación de historial de cumplimiento | Como propietario de una vivienda, quiero verificar el historial de cumplimiento de pagos de mis inquilinos, para asegurarme de que selecciono inquilinos confiables y con buen historial de pagos.      | 1. Dado que soy propietario y quiero verificar el historial de un inquilino, cuando consulto el perfil del inquilino, entonces puedo ver el historial de cumplimiento de pagos de los últimos 3 años. <br> 2. Dado que estoy revisando un posible contrato, cuando veo el historial del inquilino, entonces puedo decidir si acepto o no su solicitud. <br> 3. Dado que el historial de pagos está disponible, cuando veo detalles, entonces también puedo ver si hubo algún retraso en pagos pasados. | EP001                              |
| US003                     | Sistema de notificaciones  de pago      | Como usuario de la plataforma, quiero recibir notificaciones sobre pagos pendientes y confirmaciones de pagos, para estar siempre informado y gestionar mis finanzas eficazmente.                                               | 1. Dado que soy inquilino y tengo un próximo pago, cuando falten 5 días para la fecha de pago, entonces recibo una notificación por correo electrónico. <br> 2. Dado que utilizo la app web, cuando configuro mis notificaciones, entonces puedo elegir recibir recordatorios de pago. <br> 3. Dado que soy propietario, cuando el inquilino realiza el pago, entonces recibo una confirmación automática del pago.      | EP003                              |
| US008                     | Sistema de pago en línea        | Como inquilino, quiero realizar pagos de alquiler en línea de manera segura, para facilitar mis transacciones y asegurar mi comodidad.                                                                                               | 1. Dado que soy inquilino y debo realizar un pago, cuando accedo a la plataforma, entonces puedo realizar el pago en línea de manera segura. <br> 2. Dado que he completado el pago, cuando el sistema lo procesa, entonces recibo una confirmación tanto en la app como por correo electrónico. <br> 3. Dado que prefiero usar diferentes métodos de pago, cuando selecciono el método, entonces puedo elegir entre tarjeta de crédito o transferencia bancaria. | EP003                              |
| US014                     | Generación automática de contratos | Como arrendador, quiero que se generen automáticamente contratos con los términos acordados, para asegurar la legalidad y formalidad de los acuerdos.                                                                                  | 1. Dado que necesito un contrato para mi alquiler, cuando ingreso los términos acordados, entonces el sistema genera un contrato automáticamente. <br> 2. Dado que necesito un contrato legalmente válido, cuando se genera, entonces el sistema asegura que cumple con las regulaciones locales. <br> 3. Dado que quiero revisar el contrato, cuando lo recibo, entonces puedo firmarlo electrónicamente en la plataforma.      | EP002                              |



#### 4.1.2.2. Quality attribute Scenarios
Basándonos en las historias de usuario seleccionadas, hemos enfocado nuestra atención en cuatro atributos de calidad críticos que son esenciales para la arquitectura y operación de nuestra plataforma. Estos atributos son:
•	Seguridad
•	Rendimiento
•	Usabilidad
•	Disponibilidad
Cada uno de estos atributos ha sido cuidadosamente seleccionado para asegurar que nuestra plataforma no solo cumpla con las necesidades funcionales de los usuarios, sino que también brinde una experiencia robusta y segura. A continuación, presentamos la tabla de Quality Attribute Scenarios (QAS), la cual nos permite caracterizar y evaluar estos aspectos de calidad para su implementación y optimización en el diseño arquitectónico de la solución.

 | Atributo     | Fuente         | Estímulo                         | Artefacto       | Entorno              | Respuesta                                                                                                                                                       | Medida                                   |
|--------------|----------------|----------------------------------|-----------------|----------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------|
| Seguridad    | Usuario        | Realizar un pago de alquiler     | Sistema de pago | Plataforma web       | El sistema procesa el pago a través de un gateway seguro, usando encriptación.                                                                                 | Ningún dato de compromiso; transacciones seguras registradas. |
| Rendimiento  | Usuario        | Solicitar historial de cumplimiento | Base de datos   | Acceso web en horas pico | El sistema recupera y muestra el historial dentro de los 3 segundos, incluso bajo carga.                                                                     | Tiempo de respuesta no supera los 3 segundos en horas pico.   |
| Usabilidad   | Nuevo usuario  | Registrarse en la plataforma     | Proceso de registro | Interfaz de usuario web | El sistema guía al usuario a través de un proceso de registro directo.                                                                                        | Más del 90% de los usuarios se registran en < 5 minutos.      |
| Disponibilidad | Usuario      | Acceder a notificaciones         | Sistema de notificaciones | Plataforma web       | El sistema notifica de manera confiable las notificaciones cada vez que se accede al perfil.                                                                  | Disponibilidad del sistema del 90%.                           |

#### 4\.1.2.3. Constraints
En la fase de desarrollo de nuestro proyecto de software, resulta crucial identificar y especificar claramente las restricciones que impactarán en el diseño, implementación y operación del sistema. A continuación, se describirán detalladamente cada una de estas restricciones.

| **Technical Story ID** | **Título**              | **Descripción**                                               | **Criterios de Aceptación**                                                                                                       | **Epic ID** |
|------------------------|-------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|------------|
| TS01                   | Uso de Spring Boot JPA  | Se debe utilizar Spring Boot JPA para la implementación del backend.  | Escenario 1: Verificación del Uso de Spring Boot JPA <br> Dado que un desarrollador está implementando el backend, <br> Cuando revise el código, <br> Entonces debe confirmar que se utiliza Spring Boot JPA. | 1          |
| TS02                   | Implementación de PostgreSQL | PostgreSQL será la base de datos exclusiva del proyecto.      | Escenario 1: Verificación de Conexión a PostgreSQL <br> Dado que la base de datos necesita estar operativa, <br> Cuando se configure el backend, <br> Entonces se debe utilizar PostgreSQL como base de datos. | 1          |
| TS03                   | Desarrollo con React Native | El frontend debe ser desarrollado usando React Native.        | Escenario 1: Uso Exclusivo de React Native en el Frontend <br> Dado que se requiere un frontend móvil, <br> Cuando se revise el código del frontend, <br> Entonces debe confirmarse que se usa React Native.  | 1          |
| TS04                   | Límite de Tiempo de Desarrollo | El proyecto debe estar completo y desplegado en 3 meses.      | Escenario 1: Cumplimiento de los Plazos de Desarrollo <br> Dado que el proyecto comienza, <br> Cuando transcurran 3 meses, <br> Entonces el sistema debe estar completamente desplegado y operativo.          | 1          |
| TS05                   | Uso de GitHub Organization   | Se debe utilizar GitHub Organization para el manejo del repositorio. | Escenario 1: Configuración de GitHub Organization <br> Dado que se está configurando el control de versiones, <br> Cuando se cree el repositorio, <br> Entonces debe hacerse dentro de una GitHub Organization. | 1          |


<a name="_toc163118301"></a>
### 4.1.3. Architectural Drivers Backlog
Esta sección del proyecto cataloga los drivers clave que guían el diseño arquitectónico, organizados por su importancia y complejidad técnica. Este registro incluye Functional Drivers, Quality Attribute Drivers, y Constraints, estableciendo una hoja de ruta clara para priorizar el desarrollo y asegurar la alineación con las expectativas de los stakeholders. 

| **DRIVER ID** | **Título**                 | **Descripción**                                                                 | **Importancia para Stakeholders** | **Impacto en la Complejidad Técnica de la Arquitectura** | **Tipo**                   |
|---------------|----------------------------|---------------------------------------------------------------------------------|-----------------------------------|----------------------------------------------------------|---------------------------|
| DR01          | Seguridad de Transacciones | Garantizar la seguridad en todas las transacciones financieras dentro del sistema. | Alta                              | Alta                                                     | Quality Attribute Driver  |
| DR02          | Escalabilidad del Sistema  | El sistema debe soportar un aumento significativo en el número de usuarios sin degradar el rendimiento. | Alta                              | Alta                                                     | Quality Attribute Driver  |
| DR03          | Integración de Base de Datos | Integrar PostgreSQL de manera eficiente para manejar grandes volúmenes de datos.  | Media                             | Alta                                                     | Functional Driver         |
| DR04          | Interfaz de Usuario Responsive | Desarrollar una interfaz de usuario que se adapte a diferentes dispositivos y tamaños de pantalla.     | Media                             | Media                                                    | Quality Attribute Driver  |
| DR05          | Compatibilidad de Dispositivos | Asegurar que la aplicación funcione correctamente en varios dispositivos y plataformas.                 | Baja                              | Media                                                    | Quality Attribute Driver  |
| DR06          | Mantenimiento del Sistema   | Facilitar el mantenimiento y actualizaciones futuras del sistema sin interrupciones mayores.            | Baja                              | Baja                                                     | Constraint                |


### <a name="_toc163118302"></a>4.1.4. Architectural Design Decisions
El cuadro de Architectural Design Decisions facilita una comparación visual y estructurada de los patrones arquitectónicos MVC, Microservices, y Event-Driven Architecture contra los Architectural Drivers del proyecto. Sirve para evaluar los pros y contras de cada patrón, ayudando a tomar decisiones informadas sobre el diseño arquitectónico que mejor alinee con las necesidades y desafíos específicos del sistema. 

| **DRIVER ID** | **Título del Driver**       | **Pattern 1: MVC**                                                                                                 | **Pattern 2: Microservices**                                                                                                | **Pattern 3: Event-Driven Architecture**                                    |
|---------------|-----------------------------|--------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| DR01          | Seguridad de Transacciones  | **Pro:** Facilita una estructura organizada para implementar controles de seguridad específicos. <br> **Con:** La interacción entre componentes puede complicar la gestión de la seguridad. | **Pro:** Cada servicio puede tener sus propias políticas de seguridad, mejorando la seguridad en granularidad. <br> **Con:** Requiere una gestión de seguridad compleja y coordinada entre servicios. | **Pro:** Los eventos pueden ser monitorizados y gestionados para seguridad en tiempo real. <br> **Con:** La asincronía y la distribución pueden introducir puntos vulnerables si no se manejan adecuadamente. |
| DR02          | Escalabilidad del Sistema   | **Pro:** Baja dependencia entre componentes facilita la escalabilidad horizontal de la interfaz de usuario. <br> **Con:** Las operaciones backend complejas pueden ser menos escalables en MVC tradicional. | **Pro:** Escalabilidad inherente al permitir escalar servicios de manera independiente. <br> **Con:** La complejidad de manejar múltiples servicios puede afectar el rendimiento.              | **Pro:** Naturalmente apto para escalabilidad dado que los componentes reaccionan a eventos, no a peticiones directas. <br> **Con:** La coordinación de eventos a gran escala necesita infraestructura robusta y bien configurada. |
| DR03          | Integración de Base de Datos | **Pro:** Estructura clara para la integración y migración de bases de datos. <br> **Con:** Puede ser inflexible para cambios rápidos en esquemas de base de datos.                    | **Pro:** Cada microservicio puede usar su base de datos optimizada para sus necesidades. <br> **Con:** La sincronización entre diferentes bases de datos puede ser desafiante.              | **Pro:** Permite reaccionar a cambios en la base de datos en tiempo real. <br> **Con:** Requiere middleware robusto para gestionar eventos de la base de datos eficientemente. |
| DR04          | Interfaz de Usuario Responsive | **Pro:** Separación de la lógica de negocio y la presentación favorece adaptabilidad a diferentes dispositivos. <br> **Con:** Puede requerir más trabajo para asegurar la respuesta en todos los dispositivos. | **Pro:** Puede servir diferentes interfaces optimizadas para distintos dispositivos desde diferentes servicios. <br> **Con:** La consistencia de la interfaz entre servicios puede ser un desafío. | **Pro:** Interfaces pueden actualizar en tiempo real respondiendo a eventos del sistema. <br> **Con:** El diseño debe asegurar que los eventos no sobrecarguen al cliente con actualizaciones demasiado frecuentes. |
| DR05          | Compatibilidad de Dispositivos | **Pro:** Facilita la creación de interfaces que funcionan en múltiples dispositivos al separar frontend y backend. <br> **Con:** Requiere pruebas exhaustivas para garantizar la compatibilidad. | **Pro:** Independencia del dispositivo ya que cada servicio puede ser consumido por cualquier cliente compatible. <br> **Con:** Requiere más gestión de endpoints y versiones de API. | **Pro:** Los eventos pueden ser consumidos por cualquier dispositivo suscrito, facilitando la compatibilidad. <br> **Con:** Depende de la capacidad del dispositivo para manejar flujos de eventos en tiempo real. |
| DR06          | Mantenimiento del Sistema    | **Pro:** Modularidad facilita el mantenimiento y actualizaciones del sistema. <br> **Con:** Las dependencias entre modelos, vistas y controladores pueden complicar el mantenimiento. | **Pro:** Facilita el mantenimiento al permitir actualizar servicios de manera independiente. <br> **Con:** La gestión de múltiples servicios y sus interdependencias puede complicar el mantenimiento. | **Pro:** Permite actualizaciones en tiempo real y es adaptable a cambios con mínimas interrupciones. <br> **Con:** La complejidad de la arquitectura puede requerir herramientas especializadas para mantenimiento. |


### <a name="_toc163118303"></a>4.1.5. Quality Attribute Scenario Refinements
Los Quality Attribute Scenario Refinements detallan cómo el sistema debe manejar requisitos clave de seguridad, rendimiento, usabilidad y disponibilidad. Estos refinamientos son esenciales para asegurar que la arquitectura del sistema cumpla con las expectativas de los usuarios y los objetivos del negocio, facilitando decisiones de diseño informadas y centradas en los atributos más críticos para el éxito del proyecto. 

<table>
<tr>
<th colspan="3" valign="top"><b>Scenario Refinement for Scenario 1</b></th>
</tr>
<tr>
<td colspan="2" valign="top">Scenario</td>
<td colspan="1" valign="top">Como inquilino, quiero realizar pagos de alquiler de forma segura para evitar fraudes o robos de información.</td>
</tr>
<tr>
<td colspan="2" valign="top">Business Goals</td>
<td colspan="1" valign="top">Asegurar la confianza y protección de la información financiera de los usuarios.</td>
</tr>
<tr>
<td colspan="2" valign="top">Relevant Quality Attribute</td>
<td colspan="1" valign="top">Seguridad</td>
</tr>
<tr>
<td colspan="1" rowspan="6" valign="top">Scenario Components</td>
<td colspan="1" valign="top">Stimulus</td>
<td colspan="1" valign="top">Usuario realiza un pago de alquiler.</td>
</tr>
<tr>
<td colspan="1" valign="top">Stimulus Source</td>
<td colspan="1" valign="top">Interfaz de usuario en la plataforma web.</td>
</tr>
<tr>
<td colspan="1" valign="top">Environment</td>
<td colspan="1" valign="top">Sistema de pago en línea.</td>
</tr>
<tr>
<td colspan="1" valign="top">Artifact (if known)</td>
<td colspan="1" valign="top">Proceso de pago seguro.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response</td>
<td colspan="1" valign="top">El sistema procesa el pago a través de un gateway seguro, usando encriptación.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response Measure</td>
<td colspan="1" valign="top">Ningún dato de pago es comprometido; todas las transacciones se registran de manera segura.</td>
</tr>
<tr>
<td colspan="2" valign="top">Questions</td>
<td colspan="1" valign="top">¿Cómo se asegura la plataforma que los gateways de pago son seguros?</td>
</tr>
<tr>
<td colspan="2" valign="top">Issues</td>
<td colspan="1" valign="top">Revisar regularmente las normativas de seguridad para cumplir con estándares internacionales.</td>
</tr>
</table>



<table>
<tr>
<th colspan="3" valign="top"><b>Scenario Refinement for Scenario 2</b></th>
</tr>
<tr>
<td colspan="2" valign="top">Scenario</td>
<td colspan="1" valign="top">Como propietario, quiero solicitar el historial de cumplimiento de un inquilino rápidamente para tomar decisiones de arrendamiento informadas.</td>
</tr>
<tr>
<td colspan="2" valign="top">Business Goals</td>
<td colspan="1" valign="top">Mejorar la eficiencia operativa y satisfacción del cliente.</td>
</tr>
<tr>
<td colspan="2" valign="top">Relevant Quality Attribute</td>
<td colspan="1" valign="top">Rendimiento</td>
</tr>
<tr>
<td colspan="1" rowspan="6" valign="top">Scenario Components</td>
<td colspan="1" valign="top">Stimulus</td>
<td colspan="1" valign="top">Usuario solicita el historial de cumplimiento de un inquilino.</td>
</tr>
<tr>
<td colspan="1" valign="top">Stimulus Source</td>
<td colspan="1" valign="top">Interfaz de usuario en la plataforma web.</td>
</tr>
<tr>
<td colspan="1" valign="top">Environment</td>
<td colspan="1" valign="top">Base de datos de historiales en horas pico.</td>
</tr>
<tr>
<td colspan="1" valign="top">Artifact (if known)</td>
<td colspan="1" valign="top">Sistema de gestión de base de datos.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response</td>
<td colspan="1" valign="top">El sistema recupera y muestra el historial en menos de 3 segundos.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response Measure</td>
<td colspan="1" valign="top">Tiempo de respuesta no supera los 3 segundos en horas pico.</td>
</tr>
<tr>
<td colspan="2" valign="top">Questions</td>
<td colspan="1" valign="top">¿Cuáles son las tecnologías de base de datos empleadas para optimizar el rendimiento?</td>
</tr>
<tr>
<td colspan="2" valign="top">Issues</td>
<td colspan="1" valign="top">Monitorear y optimizar las consultas de base de datos durante las horas pico.</td>
</tr>
</table>

<table>
<tr>
<th colspan="3" valign="top"><b>Scenario Refinement for Scenario 3</b></th>
</tr>
<tr>
<td colspan="2" valign="top">Scenario</td>
<td colspan="1" valign="top">Como nuevo usuario, quiero registrarme en la plataforma de manera fácil y rápida para comenzar a utilizar el servicio sin complicaciones.</td>
</tr>
<tr>
<td colspan="2" valign="top">Business Goals</td>
<td colspan="1" valign="top">Aumentar la base de usuarios facilitando el acceso a la plataforma.</td>
</tr>
<tr>
<td colspan="2" valign="top">Relevant Quality Attribute</td>
<td colspan="1" valign="top">Usabilidad</td>
</tr>
<tr>
<td colspan="1" rowspan="6" valign="top">Scenario Components</td>
<td colspan="1" valign="top">Stimulus</td>
<td colspan="1" valign="top">Nuevo usuario se registra en la plataforma.</td>
</tr>
<tr>
<td colspan="1" valign="top">Stimulus Source</td>
<td colspan="1" valign="top">Página de registro en la interfaz web.</td>
</tr>
<tr>
<td colspan="1" valign="top">Environment</td>
<td colspan="1" valign="top">Proceso de registro.</td>
</tr>
<tr>
<td colspan="1" valign="top">Artifact (if known)</td>
<td colspan="1" valign="top">Formulario de registro.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response</td>
<td colspan="1" valign="top">El sistema guía al usuario a través de un proceso de registro sencillo y directo.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response Measure</td>
<td colspan="1" valign="top">Más del 90% de los usuarios completan el registro en menos de 5 minutos.</td>
</tr>
<tr>
<td colspan="2" valign="top">Questions</td>
<td colspan="1" valign="top">¿Cómo se manejan los errores de entrada durante el registro?</td>
</tr>
<tr>
<td colspan="2" valign="top">Issues</td>
<td colspan="1" valign="top">Asegurar que los mensajes de error sean claros y ayuden al usuario a corregir los problemas efectivamente.</td>
</tr>
</table>


<table>
<tr>
<th colspan="3" valign="top"><b>Scenario Refinement for Scenario 4</b></th>
</tr>
<tr>
<td colspan="2" valign="top">Scenario</td>
<td colspan="1" valign="top">Como usuario, quiero recibir notificaciones cuando haya cambios en el sistema para gestionar mis actividades de manera eficiente.</td>
</tr>
<tr>
<td colspan="2" valign="top">Business Goals</td>
<td colspan="1" valign="top">Mejorar la comunicación y la experiencia del usuario manteniéndolos informados de los cambios relevantes.</td>
</tr>
<tr>
<td colspan="2" valign="top">Relevant Quality Attribute</td>
<td colspan="1" valign="top">Disponibilidad</td>
</tr>
<tr>
<td colspan="1" rowspan="6" valign="top">Scenario Components</td>
<td colspan="1" valign="top">Stimulus</td>
<td colspan="1" valign="top">Usuario necesita ser notificado sobre cambios importantes en el sistema.</td>
</tr>
<tr>
<td colspan="1" valign="top">Stimulus Source</td>
<td colspan="1" valign="top">Interfaz de usuario en cualquier dispositivo.</td>
</tr>
<tr>
<td colspan="1" valign="top">Environment</td>
<td colspan="1" valign="top">Sistema de notificaciones.</td>
</tr>
<tr>
<td colspan="1" valign="top">Artifact (if known)</td>
<td colspan="1" valign="top">Servidor de notificaciones.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response</td>
<td colspan="1" valign="top">El sistema muestra de manera confiable las notificaciones cada vez que se accede al perfil.</td>
</tr>
<tr>
<td colspan="1" valign="top">Response Measure</td>
<td colspan="1" valign="top">Disponibilidad del sistema del 90%.</td>
</tr>
<tr>
<td colspan="2" valign="top">Questions</td>
<td colspan="1" valign="top">¿Cómo se gestionan y priorizan las notificaciones para evitar sobrecarga informativa?</td>
</tr>
<tr>
<td colspan="2" valign="top">Issues</td>
<td colspan="1" valign="top">Implementar filtros y configuraciones personalizables para que los usuarios controlen las notificaciones que desean recibir.</td>
</tr>
</table>


## 4.2. Strategic-Level Domain-Driven Design.

### 4.2.1. EventStorming

Se adoptó un método colaborativo y visual para modelar el contexto del dominio. Se investigaron las fases de Candidate Context Discovery, Domain Message Flows Modeling y la creación de Bounded Context Canvases.

###### *Step 1: Unstructured Exploration*
 Se llevó a cabo la etapa inicial donde se exploraron ideas y se profundizó en el conocimiento del dominio del negocio, estableciendo así las bases para el modelado en las etapas subsiguientes.

![driver](img/Capitulo_4/Unstructured%20Exploration.png)

###### *Step 2: Timelines, Step 3: Pain Points, Step 4: Pivotal Points*
Se identificaron tres etapas clave: "Timelines" para mapear la secuencia temporal de los eventos dentro del sistema, "Pain Points" para destacar y abordar los desafíos y dificultades dentro del proceso, y "Pivotal Points" que son momentos críticos que pueden influir significativamente en el diseño y la funcionalidad del sistema. 

![Step 2, 3, 4](img/Capitulo_4/Step2-3-4.png)

###### *Step 5: Commands, Step 6: Policies, Step 7: Read models, Step 8: External Systems*
Se delinearon cuatro componentes cruciales del diseño: Commands, que son acciones activadas por el usuario para influir en el sistema; Policies, reglas que guían las operaciones y mantienen la integridad del sistema; Read Models, estructuras que optimizan la recuperación y visualización de datos; y External Systems, que son servicios o plataformas externas integradas que amplían o soportan la funcionalidad del sistema. 

![Step 5, 6, 7, 8](img/Capitulo_4/Step5-6-7-8.png)

###### *Step 9: Aggregates, Step 10: Bounded Contexts*
Finalmente, se definieron dos elementos estructurales esenciales: Aggregates, que agrupan entidades y objetos relacionados para mantener la consistencia y las reglas de negocio, y Bounded Contexts, que delimitan claros contornos dentro del sistema donde los modelos de dominio aplican y se integran de manera coherente, asegurando que las interacciones entre diferentes partes del sistema sean gestionadas de forma eficaz.  

![Step 9,  10](img/Capitulo_4/Step9-10.png)

Enlace de Figma: [https://www.figma.com/design/Uc3NsOj4bLD0kn1V9fEQAS/EventStorming?node-id=0-1&t=yvJsImddBjaNskKb-1 ](https://www.figma.com/design/Uc3NsOj4bLD0kn1V9fEQAS/EventStorming?node-id=0-1&t=yvJsImddBjaNskKb-1 )

### 4.2.2. Candidate Context Discovery

Utilizando la metodología de eventstorming y centrados en la técnica de "start-with-simple", empleamos la línea de tiempo para identificar posibles candidatos para nuestro contexto delimitado, que incluyen los siguientes elementos. 

**Property Management:**
Este contexto gestiona todas las operaciones relacionadas con las propiedades listadas por los arrendadores. Incluye comandos como "Registrar nueva propiedad", "Actualizar detalles de propiedad", y "Retirar propiedad del mercado". Es fundamental para mantener la información de las propiedades actualizada y accesible, facilitando las operaciones de publicación y gestión de propiedades. Este contexto también interactúa con políticas internas para asegurar que todas las propiedades cumplan con los estándares requeridos antes de ser listadas. 

![Property Management Bounded Context](img/Capitulo_4/Property%20Management%20Bounded%20Context.png)

**Property Search:**
Este contexto permite a los arrendatarios buscar y filtrar propiedades según sus preferencias. Involucra comandos como "Iniciar búsqueda de propiedades" y "Aplicar filtros de búsqueda". Es crucial para proporcionar una experiencia de usuario eficiente, permitiendo a los arrendatarios encontrar rápidamente propiedades que se ajusten a sus necesidades. Este contexto podría interactuar con APIs externas que proporcionen datos adicionales de propiedades o recomendaciones personalizadas. 

![Property Search Bounded Context](img/Capitulo_4/Property%20Search%20Bounded%20Context.png)

**User:**
Este contexto se ocupa de la administración de usuarios, incluyendo su registro, autenticación, y gestión de perfiles. Los comandos clave incluyen "Registrar nuevo usuario" e "Iniciar sesión de usuario". Es esencial para la seguridad y personalización del sistema, asegurando que solo los usuarios autorizados puedan acceder y operar dentro de la plataforma. Utiliza servicios de verificación de identidad como sistemas externos para autenticar y validar la identidad de los usuarios. 

![User Bounded Context](img/Capitulo_4/User%20Bounded%20Context.png)

**Contracts:**
Este contexto abarca la gestión de contratos de alquiler entre arrendadores y arrendatarios. Incluye comandos para "Revisar y aceptar solicitudes de contrato" y "Responder a solicitudes de renovación de contrato". Este contexto se encarga de asegurar que todos los contratos cumplen con las normativas legales y las políticas de la plataforma, y utiliza sistemas externos como servicios de verificación de crédito para evaluar la solvencia de los arrendatarios.  

![Contracts Bounded Context](img/Capitulo_4/Contracts%20Bounded%20Context.png)

**Payments:**
Este contexto maneja todas las transacciones financieras relacionadas con el pago de alquileres. Incluye comandos para "Realizar pago online" y procesa eventos como "Realización de pago de alquiler en línea". Este contexto es vital para la gestión financiera dentro de la plataforma, asegurando transacciones seguras y eficientes a través de plataformas de pago externas y políticas que garantizan la conformidad con normativas de transacciones financieras.

![Payments Bounded Context](img/Capitulo_4/Payments%20Bounded%20Context.png)

### 4.2.3. Domain Message Flows Modeling

**Escenario 1: Alquiler de Vivienda para el Arrendatario**
Este flujo describe cómo un arrendatario inicia sesión en la plataforma usando su correo y contraseña, busca viviendas filtrando por ubicación y precio, solicita un contrato tras elegir una vivienda, y finaliza con la realización del pago del alquiler a través de plataformas de pago online, todo integrado con contratos inteligentes para asegurar transacciones seguras y automatizadas. 

![Escenario 1](img/Capitulo_4/Scenario01.png)

**Escenario 2: Alquiler de Vivienda para el Arrendador**
Este escenario ilustra cómo un arrendador ingresa a la plataforma utilizando su correo electrónico y contraseña, registra y publica nuevas viviendas con detalles como descripción, fotos, ubicación y precio, recibe solicitudes de alquiler de arrendatarios, y finalmente revisa y acepta dichas solicitudes de contrato, todo dentro de un sistema integrado que facilita la gestión eficiente de propiedades. 

![Escenario 2](img/Capitulo_4/Scenario02.png)

### 4.2.4. Bounded Context Canvases

**Contracts:**
En este Bounded Context de Contratos, se gestiona la creación, revisión y ejecución de acuerdos de alquiler, colaborando estrechamente con el Bounded Context de Property Search para recibir solicitudes de contrato. Este contexto es crucial para asegurar que tanto arrendadores como arrendatarios cumplan con las regulaciones y los términos establecidos, manteniendo un marco de transacciones seguras y confiables dentro de la plataforma.

![Contracts](img/Capitulo_4/BoundedCanvases-Contracts.png)

**Property Management:**
Este Bounded Context de Gestión de Propiedades se encarga de administrar todas las actividades relacionadas con las propiedades dentro de la plataforma. Coordina directamente con los arrendadores para el registro, actualización y eliminación de listados de propiedades, asegurando que cada propiedad cumpla con los estándares de calidad y políticas establecidas antes de su publicación. Este contexto juega un papel fundamental en mantener la integridad y la actualidad de las listas de propiedades disponibles para alquiler.

![Property Management](img/Capitulo_4/BoundedCanvases-Property%20Management.png)

**Property Search:**
Este Bounded Context de Búsqueda de Propiedades facilita la exploración y selección de viviendas por parte de los arrendatarios, permitiéndoles aplicar diversos filtros como ubicación, precio y características específicas. La interacción principal ocurre con el contexto de Gestión de Propiedades para obtener detalles precisos y actualizados de cada listado. Este contexto es esencial para proporcionar una experiencia de búsqueda eficiente y personalizada a los usuarios, ayudándoles a encontrar rápidamente propiedades que satisfagan sus necesidades específicas. 

![Property Search](img/Capitulo_4/BoundedCanvases-Property%20Search.png)

**Payments:**
Este Bounded Context de Pagos se encarga de gestionar todas las operaciones financieras relacionadas con los pagos de alquiler dentro de la plataforma. Esto incluye procesar pagos en línea, generar reportes detallados de las transacciones y asegurar la correcta notificación a los arrendadores sobre los pagos recibidos. Integrado con sistemas de pago externos y el contexto de Contratos, este contexto juega un papel crucial en la eficiencia y seguridad de las transacciones financieras, garantizando que todos los pagos se manejen de manera segura y conforme a las políticas establecidas. 

![Payments](img/Capitulo_4/BoundedCanvases-Payments.png)

**User:**
Este Bounded Context de Usuario se ocupa de todas las funciones relacionadas con la gestión de usuarios en la plataforma, incluyendo el registro de nuevos usuarios, la autenticación y la verificación de la identidad de los arrendatarios. Asegura que solo usuarios autenticados y verificados puedan interactuar con el sistema, garantizando la seguridad y la integridad de las transacciones dentro de la plataforma. Este contexto es fundamental para mantener un entorno seguro y de confianza para todos los usuarios, facilitando una experiencia de usuario fluida y protegida. 

![Contracts](img/Capitulo_4/BoundedCanvases-User.png)

Enlace a Miro: [Bounded Context Canvases](https://miro.com/app/board/uXjVKhk8XkA=/?share_link_id=403115287333)

### 4.2.5. Context Mapping

Tras identificar nuestros Bounded Contexts, procedimos a definir las relaciones estructurales entre ellos. Para esta tarea, evaluamos diversos diseños candidatos para el Context Mapping, basándonos en los patrones de relaciones entre Bounded Contexts propuestos en el Domain-Driven Design. Empleamos la herramienta en línea DomoRoboto para crear el Context Mapping mostrado en la imagen siguiente: 

![Context Mapping](img/Capitulo_4/ContextMapping.png)
## 4.3. Software Architecture.

### 4.3.1. Software Architecture System Landscape Diagram.

El diagrama de System Landscape que presentamos muestra el diseño central de nuestro sistema de transporte de paquetes, con el "FastPorte Platform" en su corazón. Este núcleo sirve como la central de gestión de paquetes, conectando a los "Clientes" con el "Carrier" adecuado para su transporte. La plataforma proporciona una interfaz clara y eficaz por medio de la cual los clientes pueden estimar la cantidad de paquetes a enviar y seleccionar el vehículo idóneo para su entrega. Este enfoque no solo optimiza la eficiencia del proceso, sino que también eleva la satisfacción de todos los actores involucrados, garantizando una experiencia de transporte fluida y sin contratiempos.

![Landscape Diagram](img/Capitulo_4/Software_Architecture_System_Landscape_Diagram/Imagen1.png)

### 4.3.2. Software Architecture Context Level Diagrams.

###### ***Diagrama de Contexto de FastPorte***

![Diagrama de Contexto](img/Capitulo_4/Software_Architecture_Context_Level_Diagrams/Imagen1.png)

| Elemento       | Responsabilidad                                                                |
| -------------- | ------------------------------------------------------------------------------ |
| Client         | Usuario de FastPorte el cual busca contratar servicios de transportista        |
| Carrier        | Usuario de FastPorte el cual busca promocionar sus servicios de transporte     |
| Admin          | Usuario administrador que tiene acceso a todas las funciones de FastPorte      |
| FastPorte      | El sistema que se desarrollará para FastPorte                                  |
| GoogleMaps     | API de GoogleMaps para poder utilizar los servicios de geolocalización         |
| RENIEC System  | Sistema externo para verificar los datos personales de los usuarios            |
| E-mail System  | Sistema de correo electrónico externo para validar servicios                   |
| Payment System | Sistema de pago externo para poder realizar pagos en la aplicación web / móvil |

### 4.3.3. Software Architecture Container Level Diagrams.
###### *Diagrama de Contenedores de FastPort*

![Diagrama de Contenedores](img/Capitulo_4/Software_Architecture_Container_Level_Diagrams/Imagen1.png)

### 4.3.4. Software Architecture Deployment Diagrams.

Para el desarrollo de aplicaciones en este proyecto, se optó por utilizar Azure debido a las necesidades específicas del proyecto. Se eligieron instancias que mejor se adaptaban a los requisitos de rendimiento y escalabilidad, proporcionando así un entorno óptimo para el desarrollo y despliegue de aplicaciones.

Una de las ventajas más significativas de usar Azure fue la rapidez en las peticiones, lo que resultó en un rendimiento mejorado de las aplicaciones. Esta característica fue crucial para satisfacer las demandas de alta disponibilidad y respuesta rápida del proyecto.

**Creación de Imágenes Docker**
Las imágenes Docker para los servicios y componentes del proyecto se crearon utilizando IntelliJ IDEA, Maven y Docker Compose. Este enfoque aseguró una integración y gestión fluidas del entorno de desarrollo, facilitando la creación y mantenimiento de las imágenes Docker.

**Gestión de Contenedores Docker**
Inicialmente, todas las pruebas se realizaron localmente para garantizar que los contenedores funcionaran según lo esperado. Tras corregir los errores identificados, los contenedores se subieron a Azure. Este proceso garantizó que los contenedores fueran robustos y estables antes de su implementación en el entorno de producción.
###### *Cloud Architecture Deployment Diagram*

![Cloud Architecture Deployment Diagram](img/Capitulo_4/Software_Architecture_Deployment_Diagrams/Imagen1.png)

---
# Conclusiones

- Aquí van las conclusiones

---
# Recomendaciones

- Aquí van las recomendaciones

--- 
# Anexos
## Repositorio con Informe
Enlace: [Repositorio Trabajo Final](https://github.com/SmartRenta/CasaFinder-Report)
## Entrega TB1
Enlace: [Exposición TB1 en Microsoft Stream]()