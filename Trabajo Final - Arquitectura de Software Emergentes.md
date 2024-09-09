**Universidad Peruana de Ciencias Aplicadas**

Ingeniería de Software

Ciclo: VIII

Sección: WS82

Profesor: Royer Edelwer Rojas Malasquez

**INFORME DE TRABAJO FINAL**

**CasaFinder**

Integrantes:

* Carrillo Mainicta, Michael - U20201A924
* Rondon Añaños, Cristopher  - U20201A291


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
          - [To-Be Scenario Mapping del usuario Arrendador](#to-be-scenario-mapping-del-usuario-arrendador)
          - [To-Be Scenario Mapping del usuario Inquilino](#to-be-scenario-mapping-del-usuario-inquilino)
  - [3.2. User Stories.](#32-user-stories)
        - [_Desarrollo de los User Stories_](#desarrollo-de-los-user-stories)
    - [EPICS](#epics)
          - [_Desarrollo de las Epics_](#desarrollo-de-las-epics)
  - [3.3. Impact Mapping.](#33-impact-mapping)
          - [\_Impact Mapping de los usuarios Arrendador e Inquilino](#_impact-mapping-de-los-usuarios-arrendador-e-inquilino)
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
| Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.     | **Cristopher Rondon Añaños**<br>*TB1* <br>- Durante el video de exposición se transmitió de manera adecuada la problemática hallada en el sector de transporte de mercadería y como se solucionaría por medio de la implementación de una página web para comunicar a transportistas con personas que requieran de sus servicios. Asimismo, se detallo como esta diseñada la propuesta y su sustentación.<br><br>**Anthony Botello** <br>*TB1* <br>- En el vídeo de exposición se indicaron a los competidores, así como también se explicó la matriz DAFO de nuestra organización. Finalmente, se expusieron resultados acerca de las entrevistas realizadas.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- Durante mi exposición, comuniqué de manera clara y objetiva los resultados de mi proyecto en ingeniería, destacando la fase de Needfinding. Presenté User Personas y una matriz de tareas de usuario, usando herramientas como Empathy Mapping y As-is Scenario Mapping. Además, delineé el escenario futuro de la plataforma propuesta, detallando User Stories, Impact Mapping y un Product Backlog completo.<br><br>**Abel Angel Cierto Espiritu**<br>*TB1* <br>- Durante el desarrollo de este primer avance, comunique de manera eficaz el objetivo del diseño al desarrollar la aplicación web. También, detalle acerca de las funcionalidades primarias  que considero que son importantes y definir los atributos de calidad para una buena aplicación es necesaria. Los constraints nos sirven para tener claro las limitaciones del sistema al momento de desarrollar la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, me enfoqué en comunicar nuestros avances y resultados de manera clara y objetiva. Presenté nuestras ideas durante el proceso de Event Storming y facilité discusiones sobre el modelado de flujo de mensajes del dominio. Mi objetivo era asegurarme de que todos los miembros del equipo, independientemente de su especialidad o nivel jerárquico, comprendieran el progreso y las decisiones tomadas en el proyecto.<br><br>  | *TB1*<br>En la exposición de la presente entrega se comunico eficientemente las bases del proyecto desarrollado y el proceso que llevo a corroborar que efectivamente es una solución adecuada para la problemática encontrada. Asimismo, se presentaron las herramientas para utilizadas para las primeras fases de implementación del proyecto y su planteamiento. |
| Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.. | **Cristopher Rondon Añaños**<br>*TB1* <br>- Se documento con éxito y de manera adecuada la introducción al proyecto, describiendo la problemática con antecedentes, ilustrando las posibles soluciones y como se busca solucionarlo de una manera más eficiente por medio del desarrollo de la presenta investigación.<br><br>**Anthony Botello** <br>*TB1* <br>- Se redactaron y documentó información y análisis de nuestros competidores y de la misma forma se evidenciaron las entrevistas realizadas y el análisis de ellas. Por otro lado, se definieron los Primary User Stories y los Quality Attribute Scenarios.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- En la elaboración de la primera entrega, me centré en comunicar de manera precisa y objetiva aspectos específicos. Utilizando el concepto de Ubiquitous Language, desarrollé un lenguaje común que facilitó la comprensión entre los miembros del equipo y los stakeholders. Además, identifiqué las limitaciones (Constraints) del proyecto y elaboré un Architectural Drivers Backlog para guiar el diseño arquitectónico. <br><br>**Abel Angel Cierto Espiritu** <br>*TB1* <br>- Los resultados de elegir drivers de arquitecturas permite un buen funcionamiento en la escalabilidad y mantenimiento del sistema. Por último los escenarios de los atributos que se requiere refinar permite una mejora continua en la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, utilicé herramientas como EventStorming para explorar y descubrir los contextos relevantes. Luego, modelé los flujos de mensajes del dominio para comprender las interacciones entre los diferentes componentes del sistema. Utilicé Bounded Context Canvases para delinear los límites y responsabilidades de cada contexto, y realicé un mapeo de contextos para visualizar las relaciones entre ellos. Finalmente, documenté nuestra arquitectura de software utilizando varios diagramas, incluidos contexto, contenedor y despliegue, para comunicar nuestra visión de manera efectiva a todas las partes interesadas. | *TB1*<br>En el informe se detalló los aspectos más importantes acerca de la base de la solución propuesta y las herramientas que se usaron para validar la misma. Por otro lado, se incluyeron los diagramas adecuados para cada sección con su respectiva descripción para brindar la mayor cantidad de información.                                                |

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

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                 | Botello Saldarriaga, Anthony Jean Pierre       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Tengo 21 años y soy estudiante de Ingeniería de Software con conocimientos de matemática y habilidades en programación en el lenguaje C++. Actualmente curso el sétimo ciclo de la carrera y mi meta es ser un profesional destacado el cual rija sus decisiones por sus valores y el bien de la cliente donde labore. Me interesa el desarrollo de la tecnología y los avances que existen en la inteligencia artificial. | ![Anthony Perfil](img/integrantes/anthony.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                           | Sabino Ramírez, Rodrigo Alexander              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Estudiante de sétimo ciclo de la carrera de Ingeniería de Software. Me considero una persona proactiva con pensamiento estratégico, con habilidades en el ámbito de la programación y un gran espíritu investigador. Para este proyecto puedo aportar parte de mi conocimiento adquirido en el curso. Además, de las habilidades blandas tales como el trabajo en equipo, comunicación, entre otras. | ![Rodrigo Perfil](img/integrantes/rodrigo.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Villegas Peralta, Branco Alberto             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Estudiante en el octavo ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas, me destaco por mi firme compromiso con la excelencia académica, respaldado por una actitud proactiva y una comunicación efectiva. Esta combinación me capacita para abordar desafíos con determinación y encontrar soluciones eficaces de manera constante. Mi capacidad para mantener la empatía y la tolerancia en situaciones diversas me facilita trabajar de manera colaborativa en equipo y adaptarme sin dificultad a diversos entornos. En términos de habilidades técnicas, poseo sólidos fundamentos en desarrollo web, destacándome en HTML, CSS y JavaScript, lo que me permite crear interfaces atractivas y funcionales. Además, mi dominio versátil en lenguajes de programación como C++, Python, Java, SQL y C# me permite afrontar desafíos desde múltiples perspectivas y encontrar soluciones innovadoras en diferentes contextos. | ![Branco Perfil](img/integrantes/branco.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Rondon Añaños, Cristopher              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Estudiante de la carrera de Ingeniería en Software. Soy una persona dinámica y curiosa, siempre dispuesta a adquirir nuevas habilidades y conocimientos. Esta actitud me ha permitido familiarizarme con herramientas y lenguajes como Java, JavaScript y SQL. Además, me entusiasma investigar y experimentar con tecnologías emergentes como el Internet de las Cosas (IoT) y la Inteligencia Artificial (IA), con el objetivo de desarrollar soluciones creativas e impactantes en el campo tecnológico. | ![Cristopher Perfil](img/integrantes/CristopherPerfil.JPG) |

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

###### To-Be Scenario Mapping del usuario Arrendador

![To Be Scenario Mapping Arrendador](img/Capitulo_3/To-be%20Arrendador.png)
###### To-Be Scenario Mapping del usuario Inquilino

![To Be Scenario Mapping Transportista](img/Capitulo_3/To-be%20Inquilino.png)

## 3.2. User Stories. 

##### _Desarrollo de los User Stories_
<table border="1">
  <tr>
    <th>Epic / User Story ID</th>
    <th>Título</th>
    <th>Descripción</th>
    <th>Criterios de Aceptación</th>
    <th>Relacionado con (Epic ID)</th>
  </tr>
  <tr>
    <td>US-01</td>
    <td>Registro de usuario</td>
    <td>Como nuevo usuario, quiero registrarme en la plataforma para acceder a sus servicios.</td>
    <td><b>Dado que</b> soy un nuevo usuario, <b>Cuando</b> completo el formulario de registro, <b>Entonces</b> debería recibir un correo de confirmación.</td>
    <td>EP-01</td>
  </tr>
  <tr>
    <td>US-02</td>
    <td>Inicio de sesión</td>
    <td>Como usuario registrado, quiero iniciar sesión en la plataforma para acceder a mi cuenta.</td>
    <td><b>Dado que</b> soy un usuario registrado, <b>Cuando</b> ingreso mis credenciales, <b>Entonces</b> debería poder acceder a mi cuenta.</td>
    <td>EP-01</td>
  </tr>
  <tr>
    <td>US-03</td>
    <td>Recuperación de contraseña</td>
    <td>Como usuario, quiero recuperar mi contraseña en caso de olvidarla para poder acceder a mi cuenta.</td>
    <td><b>Dado que</b> olvidé mi contraseña, <b>Cuando</b> solicito la recuperación, <b>Entonces</b> debería recibir un enlace para restablecerla.</td>
    <td>EP-01</td>
  </tr>
  <tr>
    <td>US-04</td>
    <td>Buscar propiedades</td>
    <td>Como inquilino, quiero buscar propiedades disponibles para alquilar según mis criterios.</td>
    <td><b>Dado que</b> estoy buscando una propiedad, <b>Cuando</b> ingreso mis criterios de búsqueda, <b>Entonces</b> debería ver una lista de propiedades que coincidan.</td>
    <td>EP-02</td>
  </tr>
  <tr>
    <td>US-05</td>
    <td>Filtrar resultados de búsqueda</td>
    <td>Como inquilino, quiero filtrar los resultados de búsqueda para encontrar propiedades que cumplan con mis necesidades específicas.</td>
    <td><b>Dado que</b> he realizado una búsqueda, <b>Cuando</b> aplico filtros, <b>Entonces</b> debería ver solo las propiedades que cumplan con esos filtros.</td>
    <td>EP-02</td>
  </tr>
  <tr>
    <td>US-06</td>
    <td>Ver detalles de propiedad</td>
    <td>Como inquilino, quiero ver los detalles completos de una propiedad para evaluar si me interesa.</td>
    <td><b>Dado que</b> estoy viendo una lista de propiedades, <b>Cuando</b> selecciono una, <b>Entonces</b> debería ver la descripción completa, fotos y condiciones del alquiler.</td>
    <td>EP-03</td>
  </tr>
  <tr>
    <td>US-07</td>
    <td>Agendar visita a propiedad</td>
    <td>Como inquilino, quiero agendar una visita a una propiedad directamente desde la plataforma.</td>
    <td><b>Dado que</b> estoy en la página de detalles de la propiedad, <b>Cuando</b> selecciono la opción de agendar visita, <b>Entonces</b> debería poder elegir una fecha y recibir confirmación de la cita.</td>
    <td>EP-03</td>
  </tr>
  <tr>
    <td>US-08</td>
    <td>Comunicación con el arrendador</td>
    <td>Como inquilino, quiero comunicarme con el arrendador a través de la plataforma para hacer consultas.</td>
    <td><b>Dado que</b> estoy interesado en una propiedad, <b>Cuando</b> envío un mensaje al arrendador, <b>Entonces</b> debería recibir una notificación <b>Cuando</b> el arrendador responda.</td>
    <td>EP-04</td>
  </tr>
  <tr>
    <td>US-09</td>
    <td>Verificación del historial del inquilino</td>
    <td>Como arrendador, quiero verificar el historial de pagos del inquilino antes de firmar un contrato.</td>
    <td><b>Dado que</b> estoy considerando alquilar mi propiedad, <b>Cuando</b> solicito el historial del inquilino, <b>Entonces</b> debería poder revisar su historial de cumplimiento de pagos.</td>
    <td>EP-05</td>
  </tr>
  <tr>
    <td>US-10</td>
    <td>Firma de contrato digital</td>
    <td>Como usuario, quiero firmar el contrato de alquiler digitalmente para mayor conveniencia.</td>
    <td><b>Dado que</b> estoy listo para firmar el contrato, <b>Cuando</b> lo reviso en la plataforma, <b>Entonces</b> debería poder firmarlo electrónicamente y recibir una copia para ambas partes.</td>
    <td>EP-05</td>
  </tr>
  <tr>
    <td>US-11</td>
    <td>Pago de alquiler</td>
    <td>Como inquilino, quiero realizar pagos automáticos del alquiler desde la plataforma.</td>
    <td><b>Dado que</b> se acerca la fecha de pago, <b>Cuando</b> programo el pago automático, <b>Entonces</b> debería procesarse y recibir una notificación de confirmación de pago exitoso.</td>
    <td>EP-06</td>
  </tr>
  <tr>
    <td>US-12</td>
    <td>Recordatorio de pago</td>
    <td>Como inquilino, quiero recibir recordatorios de pago para evitar retrasos en el alquiler.</td>
    <td><b>Dado que</b> la fecha de pago se aproxima, <b>Cuando</b> falten pocos días, <b>Entonces</b> debería recibir un recordatorio por correo o notificación para realizar el pago.</td>
    <td>EP-06</td>
  </tr>
  <tr>
    <td>US-13</td>
    <td>Solicitud de mantenimiento</td>
    <td>Como inquilino, quiero solicitar mantenimiento a través de la plataforma para problemas en la propiedad.</td>
    <td><b>Dado que</b> tengo un problema de mantenimiento, <b>Cuando</b> envío la solicitud en la plataforma, <b>Entonces</b> debería poder hacer seguimiento y recibir actualizaciones sobre el estado de la reparación.</td>
    <td>EP-07</td>
  </tr>
  <tr>
    <td>US-14</td>
    <td>Gestión de solicitudes de mantenimiento</td>
    <td>Como arrendador, quiero gestionar las solicitudes de mantenimiento de mis inquilinos.</td>
    <td><b>Dado que</b> he recibido una solicitud de mantenimiento, <b>Cuando</b> la reviso en la plataforma, <b>Entonces</b> debería poder asignarla a un proveedor y hacer seguimiento hasta su resolución.</td>
    <td>EP-07</td>
  </tr>
  <tr>
    <td>US-15</td>
    <td>Eliminar cuenta</td>
    <td>Como usuario, quiero eliminar mi cuenta de la plataforma si ya no deseo utilizar el servicio.</td>
    <td><b>Dado que</b> he decidido dejar de usar la plataforma, <b>Cuando</b> solicito la eliminación de mi cuenta, <b>Entonces</b> debería recibir una confirmación y la cuenta debería eliminarse correctamente.</td>
    <td>EP-01</td>
  </tr>
</table>





### EPICS
Las Epics que identificamos son las siguientes:

###### _Desarrollo de las Epics_

<table border = "1">
  <tr>
    <th>Epic ID</th>
    <th>Título de la Épica</th>
    <th>Descripción</th>
  </tr>
  <tr>
    <td>EP-01</td>
    <td>Gestión de Usuarios</td>
    <td>Esta épica cubre todas las funcionalidades relacionadas con la creación, autenticación, verificación y eliminación de usuarios en la plataforma, tanto para propietarios como para inquilinos.</td>
  </tr>
  <tr>
    <td>EP-02</td>
    <td>Gestión de Contratos</td>
    <td>Esta épica se enfoca en las funcionalidades que permiten la creación, modificación, generación automática y flexibilidad de contratos de arrendamiento entre propietarios e inquilinos.</td>
  </tr>
  <tr>
    <td>EP-03</td>
    <td>Gestión de Pagos y Notificaciones</td>
    <td>Esta épica incluye funcionalidades relacionadas con los pagos de alquiler, notificaciones de pagos pendientes, generación de reportes financieros y recordatorios de renovación de contratos.</td>
  </tr>
  <tr>
    <td>EP-04</td>
    <td>Verificación de Identidad y Antecedentes</td>
    <td>Esta épica aborda las funcionalidades relacionadas con la verificación de la identidad de los inquilinos y la revisión de sus antecedentes credit
  </tr>
  <tr>
    <td>EP-05</td>
    <td>Gestión del Mantenimiento de la Propiedad</td>
    <td>Esta épica cubre las funcionalidades que permiten a los inquilinos reportar problemas de mantenimiento, así como la gestión y seguimiento de las reparaciones por parte de los propietarios.</td>
  </tr>
</table>

## 3.3. Impact Mapping. 
###### _Impact Mapping de los usuarios Arrendador e Inquilino

![Impact Mapping](img/Capitulo_2/Needfinding/9.jpg)
## 3.4. Product Backlog.

##### _Desarrollo del Product Backlog_

<table border = "1">
  <thead>
    <tr>
      <th>#Orden</th>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción (Como... Quiero... Para...)</th>
      <th>Story Points</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>US-01</td>
      <td>Registro de usuario</td>
      <td>Como usuario, deseo registrarme en la plataforma para acceder a sus servicios.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>2</td>
      <td>US-02</td>
      <td>Login de usuario</td>
      <td>Como usuario, deseo iniciar sesión en la plataforma para acceder a mis propiedades y contratos.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>3</td>
      <td>US-05</td>
      <td>Búsqueda de propiedades</td>
      <td>Como inquilino, quiero buscar propiedades filtradas por ubicación, precio y características.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>4</td>
      <td>US-04</td>
      <td>Publicar propiedad</td>
      <td>Como arrendador, quiero publicar mi propiedad en la plataforma para atraer inquilinos potenciales.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>5</td>
      <td>US-06</td>
      <td>Ver detalles de propiedad</td>
      <td>Como inquilino, quiero ver los detalles completos de una propiedad para evaluar si me interesa.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>6</td>
      <td>US-07</td>
      <td>Agendar visita a propiedad</td>
      <td>Como inquilino, quiero agendar una visita a una propiedad directamente desde la plataforma.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>7</td>
      <td>US-10</td>
      <td>Firma de contrato digital</td>
      <td>Como usuario, quiero firmar el contrato de alquiler digitalmente para mayor conveniencia.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>8</td>
      <td>US-08</td>
      <td>Comunicación con el arrendador</td>
      <td>Como inquilino, quiero comunicarme con el arrendador a través de la plataforma para hacer consultas.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>9</td>
      <td>US-03</td>
      <td>Recuperar contraseña</td>
      <td>Como usuario, deseo recuperar mi contraseña en caso de olvidarla.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>10</td>
      <td>US-09</td>
      <td>Verificación del historial del inquilino</td>
      <td>Como arrendador, quiero verificar el historial de pagos del inquilino antes de firmar un contrato.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>11</td>
      <td>US-11</td>
      <td>Pago de alquiler</td>
      <td>Como inquilino, quiero realizar pagos automáticos del alquiler desde la plataforma.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>12</td>
      <td>US-12</td>
      <td>Recordatorio de pago</td>
      <td>Como inquilino, quiero recibir recordatorios de pago para evitar retrasos en el alquiler.</td>
      <td>2</td>
    </tr>
    <tr>
      <td>13</td>
      <td>US-13</td>
      <td>Solicitud de mantenimiento</td>
      <td>Como inquilino, quiero solicitar mantenimiento a través de la plataforma para problemas en la propiedad.</td>
      <td>3</td>
    </tr>
    <tr>
      <td>14</td>
      <td>US-14</td>
      <td>Gestión de solicitudes de mantenimiento</td>
      <td>Como arrendador, quiero gestionar las solicitudes de mantenimiento de mis inquilinos.</td>
      <td>5</td>
    </tr>
    <tr>
      <td>15</td>
      <td>US-15</td>
      <td>Eliminar cuenta</td>
      <td>Como usuario, quiero eliminar mi cuenta de la plataforma si ya no deseo utilizar el servicio.</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

---

# Capítulo IV: Strategic-Level Software Design
## 4.1. Strategic-Level Attribute-Driven Design
### 4.1.1. Design Purpose
El propósito fundamental del proceso de diseño de FastPorte es crear una aplicación web que facilite de manera eficiente la conexión entre transportistas y clientes que requieren servicios de transporte diversificados. Nuestra meta principal es crear una plataforma de vanguardia que proporcione una solución integral y eficiente para las necesidades de transporte de nuestros clientes y al mismo tiempo ofrezca oportunidades de crecimiento y desarrollo para los transportistas colaboradores. Nuestros objetivos se centran en la eficiencia, la seguridad, la escalabilidad y la experiencia del usuario, con una visión hacia la sostenibilidad en la industria del transporte.

**OBJETIVOS CLAVE:**

1. **Conexión Eficiente:** FastPorte tiene como objetivo principal proporcionar una interfaz de usuario intuitiva que permita a los clientes buscar y reservar fácilmente servicios de transporte. La aplicación debe garantizar que los transportistas adecuados estén disponibles para satisfacer las necesidades específicas de cada cliente.
1. **Seguridad y Confianza:** La seguridad de las transacciones y la confiabilidad de los transportistas son fundamentales para nuestro diseño. Nos comprometemos a verificar a fondo a los transportistas y proporcionar a los clientes información transparente y reseñas para tomar decisiones informadas.
1. **Escalabilidad:** FastPorte debe ser diseñado con la capacidad de crecer y adaptarse a medida que aumenta la demanda de servicios de transporte. Esto implica un diseño modular y escalable que permita la incorporación sencilla de nuevos transportistas y características adicionales.
1. **Eficiencia Operativa:** La aplicación debe optimizar la gestión de rutas, el tiempo de entrega y los recursos de los transportistas para garantizar que tanto los clientes como los transportistas obtengan el máximo valor de FastPorte.
1. **Experiencia del Usuario:** Buscamos proporcionar una experiencia de usuario excepcional, con una interfaz intuitiva y amigable que permita a los usuarios navegar sin problemas por la plataforma y realizar reservas de manera rápida y sencilla.
1. **Integración y Adaptabilidad:** FastPorte se diseñará para ser compatible con una variedad de dispositivos y sistemas, lo que permitirá futuras expansiones y la incorporación de nuevas características tecnológicas y de mercado.
1. **Sostenibilidad:** Si bien FastPorte se lanza en un dominio competitivo, aspiramos a ser líderes en la adopción de prácticas sostenibles en la industria del transporte, alentando la eficiencia energética y reduciendo la huella de carbono en la logística de transporte.

### 4.1.2. Attribute-Driven Design Inputs
#### 4.1.2.1. Primary Functionality (Primary User Stories)
| Epic /<br>User story ID | Título                               | Descripción                                                                                                                                                                     | Criterios de Aceptación                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Relacionado con (EpicID) |
| :---------------------- | :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------- |
| HU-006                  | Buscar un vehículo                   | Como cliente, quiero buscar el tipo de vehículo adecuado, para así contratarlo.                                                                                                 | <p>**Escenario N°1: El cliente busca el vehículo adecuado para contratarlo** </p><p>  </p><p>**Dado que** el cliente quiere buscar un vehículo adecuado para el servicio que requiere</p><p>**Y** se ubica en la sección “Buscar”. </p><p>**Y** se selecciona el tipo de vehículo que desea contratar</p><p>**Y** la cantidad/peso que va a transportar</p><p>**Cuando** presiona en “Enviar”</p><p>**Entonces** se le mostrarán los resultados de los vehículos acorde a su búsqueda</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | EP03                     |
| HU-008                  | Contratar el servicio                | Como cliente, quiero contratar el servicio, para acceder a los servicios del transportista.                                                                                     | <p>**Escenario N°1: El cliente desea contratar el servicio** </p><p>  </p><p>**Dado que** el cliente desea contratar el servicio para obtener los servicios del transportista </p><p>**Y** se encuentra en el perfil del transportista </p><p>**Cuando** presiona el botón “Contratar” en la parte inferior del perfil</p><p>**Entonces** aparece un formulario para realizar el contrato**  </p><p>**Y** si lo completa pasará a realizar el pago</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | EP04                     |
| HU-009                  | Realizar el pago                     | Como cliente, quiero realizar el pago del servicio, para no tener deudas pendientes.                                                                                            | <p>**Escenario N°1: El cliente realiza el pago de forma correcta**</p><p></p><p>**Dado que** el cliente ha iniciado sesión en la aplicación móvil<br>**Y** le llega una notificación de aceptación de su oferta de trabajo</p><p>**Cuando** presione “Ver más detalles”, le aparecerá la pantalla de pago </p><p>**Y** complete de forma correcta los datos de su tarjeta</p><p>**Y** presione “Pagar”</p><p>**Entonces** le aparecerá un cuadro de confirmación</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | EP07                     |
| HU-011                  | Realizar el seguimiento por GPS      | Como cliente, quiero seguir el transcurso del transportista, para sentirme seguro con el servicio.                                                                              | <p>**Escenario N°1: El cliente revisa el transcurso de su viaje**</p><p>  </p><p>**Dado que** el cliente desea observar la ubicación actual del transportista</p><p>**Cuando** se ubique en el servicio que se está realizando </p><p>**Entonces** podrá observar la ubicación actual del transportista**  </p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | EP05                     |
| HU-016                  | Ver el estado del contrato propuesto | Como cliente, quiero saber el estado de mi oferta de trabajo, para saber si fue aceptada o rechazada.                                                                           | <p>**Escenario N°1: El cliente recibe una notificación de aceptación** </p><p>  </p><p>**Dado que** el cliente ha iniciado sesión en la aplicación  </p><p>**Cuando** un transportista acepte su oferta de trabajo </p><p>**Entonces** se le mostrará en la pestaña de notificaciones un mensaje que diga que el transportista ha aceptado su oferta de trabajo </p><p></p><p>**Escenario N°2: El cliente recibe una notificación de rechazo** </p><p>  </p><p>**Dado que** el cliente ha iniciado sesión en la aplicación  </p><p>**Cuando** un transportista rechace la oferta de trabajo </p><p>**Entonces** se le mostrará en la pestaña de notificaciones un mensaje que diga que el transportista ha rechazado su oferta de trabajo </p>                                                                                                                                                                                                                                                                                                                                                                                                                        | EP08                     |
| HU-017                  | Notificar el trabajo                 | Como transportista, quiero que me notifiquen cuando un cliente requiera de mis servicios, para no perderme de algún contrato.                                                   | <p>**Escenario N°1: El transportista es notificado de un contrato nuevo** </p><p>  </p><p>**Dado que** el transportista ha iniciado sesión en la aplicación móvil</p><p>**Cuando** algún cliente le proponga un contrato  <br>**Entonces** le aparecerá una nueva notificación</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | EP08                     |
| HU-022                  | Comentar el servicio brindado        | Como cliente, quiero dejar un comentario acerca de mi experiencia con el conductor luego de terminar el servicio, para ayudar a los demás usuarios en su elección de conductor. | <p>**Escenario N°1:  El cliente deja un comentario exitosamente**</p><p></p><p>**Dado que** el cliente está autenticado en la aplicación</p><p>**Cuando** finalice un servicio</p><p>**Entonces** debe tener la opción de "Dejar un comentario" sobre el conductor.</p><p>**Dado que** el cliente seleccionó la opción "Dejar un comentario"</p><p>**Cuando** calificó al conductor con una calificación de 1 a 5 estrellas y escribió un comentario</p><p>**Entonces** su reseña debe ser registrada y visible públicamente para otros usuarios.</p><p></p><p>**Escenario N°2: El cliente tiene problemas al dejar un comentario**</p><p></p><p>**Dado que** el cliente está autenticado en la aplicación</p><p>C**uando** finalice un servicio, si la aplicación no permite dejar comentarios</p><p>E**ntonces** debe recibir un mensaje de error indicando que no se pueden dejar comentarios en este momento.</p><p>**Dado que** el cliente seleccionó la opción "Dejar un comentario"</p><p>**Si** no califica al conductor o no escribe un comentario</p><p>**Entonces** debe recibir un mensaje de error preguntándole si está seguro de omitir su reseña.</p> | EP06                     |

#### 4.1.2.2. Quality attribute Scenarios
Los escenarios de atributos de calidad son una parte fundamental del diseño de la arquitectura de software, ya que ayudan a definir cómo el sistema debe comportarse en situaciones específicas para cumplir con los requisitos de calidad esperados. En esta sección, se presenta la especificación inicial de los escenarios de atributos de calidad que tienen un impacto significativo en la arquitectura de la solución propuesta para FastPorte. Estos escenarios se han identificado con el objetivo de orientar el proceso de diseño hacia la creación de una plataforma que cumpla con las expectativas y necesidades de nuestros usuarios. 

Durante la fase de análisis, se han identificado varios atributos de calidad clave que son críticos para el éxito de FastPorte. Estos atributos incluyen usabilidad, fiabilidad, seguridad, portabilidad y mantenibilidad. Cada uno de estos atributos se refleja en una serie de escenarios que representan situaciones específicas en las cuales se evaluará el desempeño de la plataforma. 

Hemos identificado la facilidad de uso en acciones como la navegación y la modificación de datos personales, así como la respuesta rápida a las solicitudes de servicio y estrategias de tolerancia a fallos. Además, se prioriza la seguridad de los datos del usuario y la accesibilidad desde diversos dispositivos. Se enfatiza la necesidad de implementar cambios eficientemente para garantizar la continuidad del servicio.

A continuación, se presenta una tabla que detalla cada uno de los escenarios identificados, incluyendo el atributo de calidad correspondiente, la fuente del estímulo, la condición considerada, el componente afectado, el entorno, la respuesta esperada y la medida asociada.

|    Atributo    |    Fuente     |                                      Estímulo                                       |                Artefacto                 |                            Entorno                             |                                                       Respuesta                                                        |                                           Medida                                            |
| :------------: | :-----------: | :---------------------------------------------------------------------------------: | :--------------------------------------: | :------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------: |
|   Usabilidad   |    Cliente    |                       Accede por primera vez a la aplicación                        |       Interfaces de la aplicación        | <p>- Cliente nuevo </p><p>- Aplicación cargada y funcional</p> |     Las interfaces son intuitivas, permitiendo al cliente aprender a utilizar la aplicación en menos de 5 minutos      |       Tiempo necesario para que el cliente aprenda a usar la aplicación, ≤ 5 minutos        |
|   Usabilidad   |    Cliente    |             Intenta modificar su información personal en la aplicación              |    Interfaz de comunicación amigable     |                   - Nuevos datos personales                    |     La plataforma muestra una interfaz de comunicación amigable para realizar la modificación de datos personales      |             Tiempo necesario para completar la modificación de datos personales             |
|   Usabilidad   |    Cliente    |           Tiene la opción de dejar un comentario y calificar al conductor           | Formulario de calificación y comentarios |              - Servicio de transporte finalizado               |                  El proceso para dejar un comentario y calificar al conductor es sencillo e intuitivo                  |                 Tiempo necesario para completar el proceso de calificación                  |
|   Fiabilidad   |    Cliente    |            Solicita un servicio de transporte a través de la aplicación             |     Sistema de solicitud de servicio     |               - Cliente tiene una señal estable                |                                   La aplicación responde en un máximo de 5 segundos                                    |                       Tiempo de respuesta de la aplicación (segundos)                       |
|   Fiabilidad   | Sistema / Red |          Prevenir fallas e implementar estrategias de tolerancia a fallos           |                 Sistema                  |     - El sistema cuenta con una conexión de red inestable      | El sistema implementa estrategias de tolerancia a fallos, como el reintentar automáticamente en caso de errores de red |          Eficacia de las estrategias de tolerancia a fallos (porcentaje de éxito)           |
|   Seguridad    |    Cliente    |         Inicia sesión en su cuenta para solicitar un servicio de transporte         |        Módulo de inicio de sesión        |  - El cliente cuenta con sus credenciales de inicio de sesión  |      Si el inicio de sesión es exitoso, el cliente podrá realizar sus actividades con normalidad en la plataforma      |                     Éxito del inicio de sesión (valor booleano: sí/no)                      |
|   Seguridad    |    Sistema    | Almacena y utiliza los datos de tarjeta de crédito de los clientes de manera segura |   Base de datos de tarjetas de crédito   |                 - Sistema Base de datos segura                 |  Los datos de tarjeta de crédito se almacenan de forma segura y se utilizan para procesar los pagos de manera segura   | Seguridad en el almacenamiento y uso de datos de tarjeta de crédito (valor booleano: sí/no) |
|  Portabilidad  |    Cliente    |                Accede a la aplicación desde cualquier navegador web                 |             Navegadores web              |          - Cliente accede desde otro navegadores web           |                         La aplicación es accesible desde cualquier navegador web sin problemas                         |    Tiempo necesario para cargar la aplicación desde diferentes navegadores (en segundos)    |
| Mantenibilidad | Desarrollador |                      Agrega una nueva función en la aplicación                      |      Código fuente de la aplicación      |  - El desarrollador se encuentra en el entorno de desarrollo   |                   Los cambios se reflejan en la plataforma sin necesidad de un despliegue adicional                    |             Tiempo necesario para reflejar cambios en la plataforma (en horas)              |


#### 4\.1.2.3. Constraints
En la búsqueda por diseñar una arquitectura de software sólida y efectiva que integre los principios de microservicios y Domain-Driven Design (DDD) para nuestra propuesta, es fundamental considerar las restricciones arquitectónicas que guiarán nuestro proceso. Estas restricciones, derivadas de factores técnicos, regulatorios y empresariales, desempeñarán un papel clave en la toma de decisiones, asegurando que nuestra solución aborde de manera efectiva las necesidades y se ajuste a las limitaciones que puedan afectar su implementación.

| Technical Story ID | Título                                            | Descripción                                                                                                                                          | Criterios de Aceptación                                                                                                                                                                                                                                                                                                                                                                                                | Relacionado con (Epic ID) |
| :----------------- | :------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------ |
| CON-01             | Principios de Domain-Driven Design (DDD)          | La arquitectura de la aplicación debe seguir los principios de Domain-Driven Design (DDD) para modelar el dominio de manera efectiva.                | <p>Escenario: Cuando se realizan cambios en el modelo de dominio.</p><p>- **Dado que** la aplicación sigue los principios de Domain-Driven Design,</p><p>- **Cuando** los equipos de desarrollo actualizan el modelo de dominio,</p><p>- **Entonces** los cambios se reflejan de manera precisa en la arquitectura de la aplicación.</p><p></p>                                                                        | EP01                      |
| CON-02             | Escalabilidad Horizontal Eficiente                | La escalabilidad horizontal debe ser una consideración clave en la arquitectura, permitiendo la expansión de recursos de manera eficiente.           | <p>Escenario: Durante periodos de alta demanda de usuarios.</p><p>- **Dado que** la aplicación debe escalar horizontalmente de manera eficiente,</p><p>- **Cuando** el número de usuarios concurrentes aumenta significativamente,</p><p>- **Entonces** la aplicación es capaz de distribuir la carga de manera eficiente y mantener un rendimiento óptimo.</p><p></p>                                                 | EP03                      |
| CON-03             | Redundancia y Recuperación ante Desastres         | La aplicación debe ser diseñada con redundancia y recuperación ante desastres para garantizar la disponibilidad continua del servicio.               | <p>Escenario: En caso de fallo de un servidor principal.</p><p>- **Dado que** la aplicación se ha diseñado con redundancia y recuperación ante desastres,</p><p>- **Cuando** un servidor principal falla,</p><p>- **Entonces** la aplicación se conmuta automáticamente al servidor secundario sin pérdida de datos o interrupción del servicio.</p><p></p>                                                            | EP04                      |
| CON-04             | Uso de Servicios en la Nube y Contenedores        | Se debe utilizar un proveedor de servicios en la nube y aprovechar servicios de contenedores como Kubernetes.                                        | <p>Escenario: Durante el despliegue y escalado de la aplicación.</p><p>- **Dado que** se utilizan servicios en la nube y contenedores para desplegar la aplicación,</p><p>- **Cuando** se despliegan nuevas instancias de la aplicación o se escalan los recursos,</p><p>- **Entonces** la orquestación de contenedores asegura una distribución eficiente de la carga y una respuesta rápida a la demanda.</p><p></p> | EP02                      |
| CON-05             | Adaptabilidad y Agilidad en las Mejoras           | La plataforma debe ser altamente adaptable para incorporar nuevas características y mejoras de manera ágil y eficiente.                              | <p>Escenario: Al introducir una nueva funcionalidad.</p><p>- **Dado que** se prioriza la adaptabilidad y agilidad en el desarrollo,</p><p>- **Cuando** se introduce una nueva funcionalidad o se realiza una mejora,</p><p>- **Entonces** los usuarios pueden acceder a la nueva funcionalidad sin interrupciones en el servicio y sin necesidad de una actualización manual.</p><p></p>                               | EP06                      |
| CON-06             | Independencia y Desacoplamiento de Microservicios | Los microservicios deben ser independientes y desacoplados, lo que permite a los equipos de desarrollo trabajar de manera autónoma en cada uno.      | <p>Escenario: Cuando se actualiza un microservicio específico.</p><p>- **Dado que** los microservicios están diseñados para ser independientes y desacoplados,</p><p>- **Cuando** se actualiza un microservicio específico,</p><p>- **Entonces** los cambios en ese microservicio no afectan el funcionamiento de otros microservicios y la aplicación continúa funcionando sin problemas.</p><p></p>                  | EP09                      |
| CON-07             | Gestión de Versiones y Control de Cambios         | Debe implementarse un sistema de gestión de versiones y control de cambios para mantener la integridad del código y la colaboración efectiva.        | <p>Escenario: Durante la implementación de una nueva funcionalidad.</p><p>- **Dado que** se implementa un sistema de gestión de versiones y control de cambios,</p><p>- **Cuando** se implementa una nueva funcionalidad o se realiza un cambio en el código,</p><p>- **Entonces** todos los cambios están registrados y documentados adecuadamente en el sistema de control de versiones.</p><p></p>                  | EP08                      |
| CON-08             | Documentación Integral de Microservicios          | Los microservicios deben estar documentados de manera correcta para facilitar su comprensión y uso por parte de otros desarrolladores.               | <p>Escenario: Al integrar un nuevo microservicio.</p><p>- **Dado que** cada microservicio está completamente documentado,</p><p>- **Cuando** un desarrollador necesita integrar un nuevo microservicio en la aplicación,</p><p>- **Entonces** la documentación proporciona información clara y detallada sobre su funcionamiento y cómo se integra con el resto del sistema.</p><p></p>                                | EP10                      |
| CON-09             | Modularidad y Flexibilidad Arquitectónica         | La arquitectura debe ser altamente modular, lo que permite la sustitución o actualización de componentes individuales sin afectar a todo el sistema. | <p>Escenario: Al actualizar un componente del sistema.</p><p>- **Dado que** la arquitectura se basa en principios de modularidad y flexibilidad,</p><p>- **Cuando** se actualiza o reemplaza un componente del sistema,</p><p>- **Entonces** la implementación de los cambios se realiza de forma aislada y no afecta negativamente a otros componentes del sistema.</p><p></p>                                        | EP05                      |
| CON-10             | Seguridad de Datos y Privacidad del Usuario       | La seguridad de datos y la privacidad del usuario deben ser prioritarias, cumpliendo con las regulaciones de protección de datos aplicables.         | <p>Escenario: Al acceder a datos sensibles.</p><p>- **Dado que** la seguridad de datos y la privacidad del usuario son prioritarias,</p><p>- **Cuando** un usuario accede a datos sensibles o realiza una transacción,</p><p>- **Entonces** la información se almacena y se transmite de forma segura, protegiendo la privacidad del usuario y cumpliendo con las regulaciones de privacidad aplicables.</p><p></p>    | EP07                      |
| CON-11             | Estrategia de Respaldo y Recuperación de Datos    | Se debe implementar una estrategia de respaldo y recuperación de datos para garantizar la integridad y disponibilidad de la información crítica.     | <p>Escenario: Durante una restauración de datos de emergencia.</p><p>- **Dado que** se implementa una estrategia de respaldo y recuperación de datos,</p><p>- **Cuando** se produce una pérdida de datos o una interrupción del servicio,</p><p>- **Entonces** los datos críticos se pueden restaurar rápidamente y el servicio se restablece sin pérdida de funcionalidad.</p><p></p>                                 | EP01                      |
| CON-12             | Fechas de Entrega Inamovibles                     | Las fechas de entrega de los hitos del proyecto son inamovibles y no pueden ser pospuestas.                                                          | <p>Escenario: Durante el cumplimiento de un hito del proyecto.</p><p>- **Dado que** las fechas de entrega son inamovibles,</p><p>- **Cuando** se planifica y ejecuta el desarrollo del proyecto,</p><p>- **Entonces** los hitos del proyecto se entregan dentro del plazo establecido sin retrasos significativos.</p><p></p>                                                                                          | EP03                      |

<a name="_toc163118301"></a>
### 4.1.3. Architectural Drivers Backlog
Como equipo nos embarcamos en un proceso colaborativo para desarrollar una solución innovadora que abordara las complejidades del sector del transporte. Reconociendo las dificultades que enfrentan tanto los usuarios cotidianos como los transportistas independientes. Este proceso implicó una serie de pasos, desde la identificación de oportunidades de negocio hasta la definición de los requisitos arquitectónicos clave, que se documentaron en el Arquitectural Driver Backlog (ADB) para guiar el desarrollo futuro de la solución.

| Driver ID | Título de Driver                                     | Descripción                                                                                                                                                  | Importancia para Stakeholders (High, Medium, Low) | Impacto en Architecture Technical Complexity (High, Medium, Low) |
| :-------- | :--------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------ | :--------------------------------------------------------------- |
| D01       | Escalabilidad para el crecimiento futuro             | Permitir que la plataforma FastPorte maneje un aumento significativo en el volumen de usuarios y transacciones a medida que crece el negocio.                | High                                              | High                                                             |
| D02       | Seguridad de datos y privacidad                      | Garantizar la protección adecuada de la información confidencial de los usuarios y la integridad de los datos.                                               | High                                              | High                                                             |
| D03       | Interfaz de usuario intuitiva y amigable             | Diseñar una interfaz que sea fácil de usar y que brinde una experiencia positiva para los clientes y transportistas.                                         | High                                              | Medium                                                           |
| D04       | Integración con servicios de pago                    | Facilitar el proceso de pago para los usuarios al integrar métodos de pago seguros y confiables en la plataforma.                                            | High                                              | Medium                                                           |
| D05       | Notificaciones en tiempo real                        | Proporcionar a los usuarios actualizaciones instantáneas sobre el estado de sus viajes y transacciones.                                                      | Medium                                            | High                                                             |
| D06       | Adaptabilidad a múltiples dispositivos y plataformas | Garantizar que la plataforma sea accesible y funcione de manera óptima en una variedad de dispositivos y sistemas operativos.                                | Medium                                            | High                                                             |
| D07       | Gestión eficiente de la carga de trabajo             | Implementar herramientas y sistemas para administrar eficazmente la carga de trabajo de los transportistas y optimizar su tiempo y recursos.                 | Medium                                            | High                                                             |
| D08       | Mantenibilidad y escalabilidad del código            | Desarrollar un código limpio y modular que sea fácil de mantener y ampliar a medida que evoluciona la plataforma.                                            | Medium                                            | High                                                             |
| D09       | Análisis y generación de informes de datos           | Implementar herramientas para recopilar y analizar datos operativos y de rendimiento, y generar informes significativos para informar la toma de decisiones. | Low                                               | High                                                             |

### <a name="_toc163118302"></a>4.1.4. Architectural Design Decisions
Para crear decisiones de diseño arquitectónico basados en los drivers arquitectónicos, utilizaremos la siguiente matriz:

| Driver ID | Título de Driver                                     | Pattern 1                        | Pattern 2                                     | Pattern 3                                    |
| :-------- | :--------------------------------------------------- | :------------------------------- | :-------------------------------------------- | :------------------------------------------- |
| D01       | Escalabilidad para el crecimiento futuro             | Microservicios                   | Autoescalado                                  | Colas de mensajes                            |
| D02       | Seguridad de datos y privacidad                      | Gateway de API segura            | Encriptación de datos en reposo y en tránsito | Autenticación y autorización basada en roles |
| D03       | Interfaz de usuario intuitiva y amigable             | Diseño responsive                | Arquitectura micro fronted                    | Patrones de diseño de UI/UX                  |
| D04       | Integración con servicios de pago                    | Pasarela de pago de terceros     | API de pagos unificada                        | Servicios web seguros                        |
| D05       | Notificaciones en tiempo real                        | Event Sourcing                   | WebSockets                                    | Sistema de colas de mensajes                 |
| D06       | Adaptabilidad a múltiples dispositivos y plataformas | Diseño responsive                | PWA (Progressive Web Apps)                    | Cross-Platform Development Frameworks        |
| D07       | Gestión eficiente de la carga de trabajo             | Orquestación de contenedores     | Colas de trabajo                              | Escalado automático                          |
| D08       | Mantenibilidad y escalabilidad del código            | Código limpio y principios SOLID | Arquitectura basada en componentes            | Integración y entrega continua (CI/CD)       |
| D09       | Análisis y generación de informes de datos           | Almacenes de datos               | Procesamiento de eventos en tiempo real       | Herramientas BI (Business Intelligence)      |

### <a name="_toc163118303"></a>4.1.5. Quality Attribute Scenario Refinements

<table><tr><th colspan="3" valign="top"><b>Scenario Refinement for Scenario 1</b></th></tr>
<tr><td colspan="2" valign="top">Scenario(s):</td><td colspan="1" valign="top">Escalabilidad para el crecimiento Futuro</td></tr>
<tr><td colspan="2" valign="top">Business Goals</td><td colspan="1" valign="top">Asegurar la expansión sostenible y la competitividad en el mercado</td></tr>
<tr><td colspan="2" valign="top">Relevant Quality Attributes</td><td colspan="1" valign="top">Tiempo de respuesta para la implementación de capacidad adicional no superior a 3 min después de detectar aumentos en la demanda</td></tr>
<tr><td colspan="1" rowspan="6" valign="top">Scenario Components</td><td colspan="1" valign="top">Stimulus</td><td colspan="1" valign="top">La plataforma FastPorte experimenta un aumento del 300% en el volumen de usuarios y transacciones en un periodo de 4 semanas</td></tr>
<tr><td colspan="1" valign="top">Stimulus Source</td><td colspan="1" valign="top">Incremento significativo en el número de usuarios activos y transacciones simultáneas</td></tr>
<tr><td colspan="1" valign="top">Environment</td><td colspan="1" valign="top">En operación normal bajo condiciones de carga de trabajo aumentadas</td></tr>
<tr><td colspan="1" valign="top">Artifact (if known)</td><td colspan="1" valign="top">Los servidores ejecutan la lógica de negocio y manejan las solicitudes de los usuarios. Componentes como balanceadores de carga.</td></tr>
<tr><td colspan="1" valign="top">Response</td><td colspan="1" valign="top">El sistema debe escalar de manera automática para manejar el aumento de carga, manteniendo los tiempos de respuesta dentro de los parámetros aceptables y sin degradar la experiencia del usuario ni la integridad de los datos.</td></tr>
<tr><td colspan="1" valign="top">Response Measure</td><td colspan="1" valign="top">El tiempo de respuesta para transacciones críticas no debe exceder los 2 segundos, y el sistema debe ser capaz de aumentar su capacidad (ya sea mediante escalado horizontal o vertical) dentro de los 3 minutos siguientes a la detección del incremento en la carga de trabajo.</td></tr>
<tr><td colspan="2" valign="top">Questions</td><td colspan="1" valign="top">¿Existen proyecciones o estimaciones del crecimiento esperado en el volumen de usuarios y transacciones a lo largo del tiempo?</td></tr>
<tr><td colspan="2" valign="top">Issues</td><td colspan="1" valign="top">A medida que un sistema se escala, su complejidad operativa puede aumentar significativamente. ¿Cómo se planea manejar esta complejidad adicional?</td></tr>
</table>


<table><tr><th colspan="3" valign="top">Scenario Refinement for Scenario 2</th></tr>
<tr><td colspan="2" valign="top">Scenario(s):</td><td colspan="1" valign="top">Mantenibilidad y escalabilidad del código</td></tr>
<tr><td colspan="2" valign="top">Business Goals</td><td colspan="1" valign="top">Acelerar el tiempo de lanzamiento al mercado de nuevas funcionalidades, manteniendo o mejorando la calidad del software.</td></tr>
<tr><td colspan="2" valign="top">Relevant Quality Attributes</td><td colspan="1" valign="top">Mantenibilidad y Escalabilidad</td></tr>
<tr><td colspan="1" rowspan="6" valign="top">Scenario Components</td><td colspan="1" valign="top">Stimulus</td><td colspan="1" valign="top">La necesidad de modificar, extender, o escalar componentes del sistema para introducir nuevas funcionalidades, mejorar el rendimiento, o adaptarse a cambios en el entorno tecnológico o del negocio.</td></tr>
<tr><td colspan="1" valign="top">Stimulus Source</td><td colspan="1" valign="top">Equipo de desarrollo, cambios en requisitos del negocio, actualizaciones tecnológicas.</td></tr>
<tr><td colspan="1" valign="top">Environment</td><td colspan="1" valign="top">Desarrollo y mantenimiento post-lanzamiento.</td></tr>
<tr><td colspan="1" valign="top">Artifact (if known)</td><td colspan="1" valign="top">Código fuente, documentación del sistema, tests automatizados.</td></tr>
<tr><td colspan="1" valign="top">Response</td><td colspan="1" valign="top">El sistema facilita las modificaciones, extensiones y escalado con un mínimo impacto en los componentes existentes y sin degradar la calidad general o el rendimiento.</td></tr>
<tr><td colspan="1" valign="top">Response Measure</td><td colspan="1" valign="top">El tiempo requerido para implementar una nueva funcionalidad o modificar una existente no debe aumentar de manera significativa a medida que el sistema crece.</td></tr>
<tr><td colspan="2" valign="top">Questions</td><td colspan="1" valign="top">¿Cómo se estructurará el código para facilitar su comprensión y modificación?</td></tr>
<tr><td colspan="2" valign="top">Issues</td><td colspan="1" valign="top">Asegurar que el sistema escale de manera efectiva sin comprometer el rendimiento bajo cargas de trabajo elevadas.</td></tr>
</table>
## 4.2. Strategic-Level Domain-Driven Design.

### 4.2.1. EventStorming

###### *Step 1: Unstructured Exploration*
![driver](img/Capitulo_4/Event_Storming/Imagen1.png)
###### *Step 2: Timelines, Step 3: Pain Points, Step 4: Pivotal Points*
![Step 2 Part 1](img/Capitulo_4/Event_Storming/Imagen2.png)
![Step 2 Part 2](img/Capitulo_4/Event_Storming/Imagen3.png)
![Step 2 Part 3](img/Capitulo_4/Event_Storming/Imagen4.png)

###### *Step 5: Commands, Step 6: Policies, Step 7: Read models, Step 8: External Systems*

![Step 5, 6, 7, 8,  Part 1](img/Capitulo_4/Event_Storming/Imagen5.png)
![Step 5, 6, 7, 8,  Part 2](img/Capitulo_4/Event_Storming/Imagen6.png)
![Step 5, 6, 7, 8,  Part 3](img/Capitulo_4/Event_Storming/Imagen7.png)

###### *Step 9: Aggregates, Step 10: Bounded Contexts*

![Step 9,  10](img/Capitulo_4/Event_Storming/Imagen8.png)
Enlace de Figma para una mejor visualización: [https://www.figma.com/file/RqNZH8CXgzb4YsO1sjOR7v/Event-Storming---FastPorte?type=whiteboard&node-id=0%3A1&t=PA6eDILnRHf7lfWC-1](https://www.figma.com/file/RqNZH8CXgzb4YsO1sjOR7v/Event-Storming---FastPorte?type=whiteboard&node-id=0%3A1&t=PA6eDILnRHf7lfWC-1)

### 4.2.2. Candidate Context Discovery

Utilizando la metodología de eventstorming y adoptando el enfoque de "start-with-simple", empleamos una línea de tiempo como herramienta para discernir potenciales candidatos dentro de nuestro contexto definido. Estos candidatos identificados son los siguientes:

**Búsqueda de Vehículos**
Este bounded context se centra en la búsqueda de vehículos, integrando eventos como la inspección de perfiles de transportistas, la reconsideración de opciones por parte de los usuarios, y el regreso a la sección principal. Utiliza comandos para elegir vehículos, aplicar filtros, y aprovechar una API de inteligencia artificial, junto con políticas para manejar usuarios fuera de cobertura y ofrecer recomendaciones personalizadas. Su objetivo es optimizar la selección de transporte, haciéndola eficiente y adaptada a las necesidades del usuario.

![Búsqueda de vehículos Bounded Context](img/Capitulo_4/Candidate_Context_Discovery/Imagen1.png)
**Servicios**
Este Bounded Context aborda servicios de transporte, enfocándose en eventos clave como el retorno de usuarios a la página principal, accesos al soporte, aceptaciones de ofertas por transportistas, seguimientos GPS, y servicios concluidos. Los comandos gestionan ofertas y el estado de registro de vehículos, mientras que la política de GPS activado mejora la transparencia y la experiencia de seguimiento. Su propósito es optimizar las interacciones entre clientes y transportistas, asegurando una comunicación efectiva y una mayor satisfacción en el servicio.

![Servicios Bounded Context](img/Capitulo_4/Candidate_Context_Discovery/Imagen2.png)

**Cliente**
Este Bounded Context se centra en la experiencia del cliente dentro de una aplicación de servicios de transporte, abarcando eventos desde el registro en la aplicación hasta la realización de ofertas por servicios. Los eventos clave incluyen la búsqueda de transportistas que se ajusten a las necesidades específicas del cliente, la visualización de perfiles de transportistas y sus vehículos, y la elección de una opción de transporte. Los comandos disponibles permiten el registro de usuarios y la selección de vehículos, mientras que las políticas garantizan que los usuarios operen dentro de la cobertura y con datos ingresados correctamente. Este contexto busca facilitar la conexión entre clientes y transportistas, asegurando un proceso de selección eficiente y satisfactorio.

![Cliente Bounded Context](img/Capitulo_4/Candidate_Context_Discovery/Imagen3.png)

**Transportista**
Este Bounded Context se centra en los transportistas, desde su registro en la aplicación hasta el registro de nuevos vehículos, incluyendo el acceso a sus perfiles y el llenado de información vehicular. Los comandos principales son para registrar tanto al usuario como al vehículo, con políticas que aseguran la correcta o incorrecta entrada de datos. Este contexto apunta a facilitar la gestión de transportistas y sus vehículos, promoviendo la precisión en el registro de información.

![Transportista Bounded Context](img/Capitulo_4/Candidate_Context_Discovery/Imagen4.png)

### 4.2.3. Domain Message Flows Modeling

**Escenario 1: Cliente Solicita Servicio de Transporte**
En este escenario, un cliente utiliza una aplicación de servicios de transporte para solicitar un servicio de transporte de sus paquetes desde un lugar de recogida hasta un destino. El cliente inicia sesión en la aplicación. Luego, toma una foto de los paquetes para adjuntarla a la solicitud de transporte. La aplicación envía la solicitud junto con la foto al sistema de búsqueda de vehículos, que utiliza una API de inteligencia artificial para encontrar el transporte adecuado. Una vez encontrado, el sistema notifica al cliente sobre la asignación del transporte, proporcionando detalles adicionales

![Escenario 1](img/Capitulo_4/Domain_Message_Flows_Modeling/Imagen1.png)

**Escenario 2: Transportista Realiza el Servicio de Transporte**
En este escenario, un transportista utiliza una aplicación de servicios de transporte para llevar a cabo un servicio de transporte de paquetes. El transportista inicia sesión en la aplicación, revisa las solicitudes de transporte disponibles y acepta una de ellas. Luego, se dirige al lugar de recogida donde recoge los paquetes del cliente. Una vez recogidos, inicia el servicio de transporte y se dirige al destino. Durante el viaje, el sistema realiza un seguimiento GPS del transporte. Una vez que llega al destino y entrega los paquetes, se registra la finalización del servicio y se notifica al cliente sobre la entrega exitosa.

![Escenario 2](img/Capitulo_4/Domain_Message_Flows_Modeling/Imagen2.png)

### 4.2.4. Bounded Context Canvases

**Búsqueda de Vehículos**
Este bounded context se centra en el problema del dominio y es la búsqueda de vehículos, con el objetivo de optimizar la selección de opciones de transporte para los usuarios. En cuando a los subdominios se encuentra la inspección de los perfiles de transportistas y reconsideración de opciones, selección y filtrado de vehículos.

![Búsqueda de vehículos Canvas](img/Capitulo_4/Bounded_Context_Canvases/Imagen1.png)

**Servicios**
El Bounded Context Canvas para servicios de transporte es una herramienta estratégica diseñada para definir y delinear las características clave de este dominio específico dentro de un sistema de software. Proporciona una visión integral de cómo este contexto interactúa con los usuarios, gestiona datos y se comunica con otros contextos o sistemas.

![Servicios Canvas](img/Capitulo_4/Bounded_Context_Canvases/Imagen2.png)

**Transportista**
Este Bounded Context se centra en la gestión integral de los transportistas y sus vehículos, desde el registro inicial en la aplicación hasta la actualización continua de su información vehicular y personal. Este contexto define cómo los transportistas interactúan con la plataforma, estableciendo procesos y políticas claras para el registro de usuarios y vehículos, la validación de datos, y la comunicación entre la plataforma y los transportistas.

![Transportista Canvas](img/Capitulo_4/Bounded_Context_Canvases/Imagen3.png)

### 4.2.5. Context Mapping

Después de obtener cuáles serían nuestros Bounded Contexts, se realizó la elaboración de las relaciones estructurales entre estos. Para ello, se tomó en cuenta posibles diseños candidatos para el Context Mapping, el cual se desarrolló considerando los patrones de relaciones entre Bounden Contexts establecidos en Domain-Driven Desgin. Se utilizó la herramienta online DomoRoboto para elaborar el Context Mapping de la siguiente imagen:

![Context Mapping](img/Capitulo_4/Context_Mapping/Imagen1.png)
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

- El desarrollo del Lean UX Process ayudó a comprender mejor y aplicar efectivamente las herramientas en nuestra propuesta enfocada al servicio de transportistas hacia clientes. De la misma forma, contribuyó a definir de manera más clara nuestro público objetivo o llámese segmento hacia el cual va enfocada nuestra aplicación.
- Después de culminar la primera parte de nuestro proyecto e identificar los principales problemas que tienen nuestros segmentos, concluimos que sería de mucha ayuda el desarrollo de FastPorte con el fin de mejorar la experiencia de los transportistas al momento de ofrecer sus servicios, al igual que a los clientes sería una herramienta eficiente en su trabajo.
- El desarrollo de entrevistas nos ayudó a esclarecer la visión del proyecto, en cuanto a la perspectiva del usuario y por lo tanto fue importante para mejorar los aspectos de las funcionalidades de la aplicación.
- La transición a microservicios y la contenerización con Docker ha mejorado significativamente la modularidad del sistema. Cada microservicio puede desarrollarse, probarse e implementarse de manera independiente, lo que facilita la escalabilidad y el mantenimiento a largo plazo. Esta arquitectura modular también permite la adopción de tecnologías específicas para cada servicio.
- La contenerización y el uso de orquestadores como Kubernetes han proporcionado un entorno de despliegue más consistente y predecible. Ahora podemos implementar actualizaciones y mejoras de manera más rápida y eficiente, reduciendo el tiempo de inactividad y mejorando la experiencia del usuario. La capacidad de realizar implementaciones continuas se ha vuelto más factible.
- Aunque la arquitectura de microservicios ofrece ventajas claras, también presenta desafíos en la gestión de la complejidad. La coordinación entre microservicios, la configuración adecuada de las relaciones entre ellos y la gestión de versiones son aspectos críticos que requieren atención constante. Además, es esencial tener un equipo bien capacitado y una documentación completa para abordar estos desafíos de manera efectiva.

---
# Recomendaciones

- Se recomienda realizar los diagramas C4 con el lenguaje de programación C# y usando el módulo de Structurizr.Client en Nuget. Esto con el fin de poder gestionar las versiones de la arquitectura realizada. Asimismo, para poder realizar una mejor documentación de cada uno de los servicios implementados.
- Asegurarse de tener una documentación clara y accesible para cada microservicio. Esto facilitará la comprensión y colaboración del equipo, así como la integración de nuevos miembros. Utiliza un formato fácil de seguir, destacando los puntos clave sobre la funcionalidad, API y dependencias.
- Implementar pruebas rigurosas para cada microservicio antes y después de la contenerización. Las pruebas unitarias, de integración y funcionales son fundamentales. Garantizar la estabilidad y la funcionalidad adecuada en un entorno contenerizado minimizará problemas en el despliegue y mejorará la confianza en el sistema.
- Implementar un sólido plan de respaldo y recuperación para los datos de los microservicios. Utilizar soluciones automatizadas para realizar copias de seguridad periódicas y verificar regularmente la capacidad de restauración. Y así lograr un enfoque proactivo hacia la gestión de datos garantizará la integridad y disponibilidad del sistema en caso de fallos inesperados.

--- 
# Anexos
## Repositorio con Informe
Enlace: [Repositorio Trabajo Final](https://github.com/Arquitectura-WS82/TrabajoFinal)
## Entrega TB1
Enlace: [Exposición TB1 en Microsoft Stream](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201c172_upc_edu_pe/Ec1gj2b9GwhMiIeeW4ZbOQUBjR8V_vwBKCj4ByvhRvIVLg?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=mEYRo9)