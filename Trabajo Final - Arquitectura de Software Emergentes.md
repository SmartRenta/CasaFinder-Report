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
* Vara Quispe, José Carlos - U202125116



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
        - [Business Assumptions](#business-assumptions)
        - [User Assumptions](#user-assumptions)
        - [Features](#features)
        - [Business Outcomes](#business-outcomes)
        - [User Outcomes](#user-outcomes)
      - [1.2.2.3. Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)
      - [1.2.2.4. Lean UX Canvas](#1224-lean-ux-canvas)
  - [1.3. Segmentos Objetivo](#13-segmentos-objetivo)
        - [Segmento Propietarios de Viviendas](#segmento-propietarios-de-viviendas)
        - [Segmento Inquilinos](#segmento-inquilinos)
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
  - [2.3. Needfinding](#23-needfinding)
    - [2.3.1. User Personas](#231-user-personas)
    - [2.3.2. User Task Matrix](#232-user-task-matrix)
    - [Propietarios](#propietarios)
    - [Inquilinos](#inquilinos)
    - [2.3.3. User Journey Mapping](#233-user-journey-mapping)
    - [2.3.4. Empathy Mapping](#234-empathy-mapping)
    - [2.3.5. As-is Scenario Mapping](#235-as-is-scenario-mapping)
  - [2.4. Ubiquitous Language](#24-ubiquitous-language)
    - [Blockchain](#blockchain)
    - [Contrato Inteligente (Smart Contract)](#contrato-inteligente-smart-contract)
    - [Descentralización](#descentralización)
    - [Inmutabilidad](#inmutabilidad)
    - [Oráculos](#oráculos)
    - [Tokenización del Alquiler](#tokenización-del-alquiler)
    - [Automatización de Pagos](#automatización-de-pagos)
    - [Depósito de Garantía en Blockchain](#depósito-de-garantía-en-blockchain)
    - [Resolución de Disputas Automatizada](#resolución-de-disputas-automatizada)
    - [Auditoría Transparente](#auditoría-transparente)
    - [Plataforma de Alquiler Descentralizada](#plataforma-de-alquiler-descentralizada)
    - [Wallet Digital](#wallet-digital)
    - [Identidad Digital Descentralizada](#identidad-digital-descentralizada)
    - [Penalizaciones Automáticas](#penalizaciones-automáticas)
    - [Rentabilidad Tokenizada](#rentabilidad-tokenizada)
    - [2.3.1 User Persona](#231-user-persona)
          - [_User Persona Manuel Segura, usuario Cliente_](#user-persona-manuel-segura-usuario-cliente)
          - [_User Persona Manuel Segura, usuario Transportista_](#user-persona-manuel-segura-usuario-transportista)
    - [2.3.2 User Task Matrix](#232-user-task-matrix-1)
          - [_User Task Matrix del usuario cliente_](#user-task-matrix-del-usuario-cliente)
          - [_User Task Matrix del usuario transportista_](#user-task-matrix-del-usuario-transportista)
    - [2.3.3 Empathy Mapping](#233-empathy-mapping)
          - [*Empathy Mapping del usuario cliente*](#empathy-mapping-del-usuario-cliente)
          - [*Empathy Mapping del usuario transportista*](#empathy-mapping-del-usuario-transportista)
    - [2.3.4. As-is Scenario Mapping.](#234-as-is-scenario-mapping)
          - [*As-is Scenario Mapping del usuario cliente*](#as-is-scenario-mapping-del-usuario-cliente)
          - [*As-is Scenario Mapping del usuario transportista*](#as-is-scenario-mapping-del-usuario-transportista)
  - [2.4. Ubiquitous Language.](#24-ubiquitous-language-1)
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
| Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.     | **José Carlos Vara**<br>*TB1* <br>-Desarrollé y presenté los puntos clave del perfil de la startup y la solución propuesta, incluyendo los antecedentes, la problemática y el proceso Lean UX, adaptando la comunicación para un público de diversas especialidades y niveles jerárquicos. Utilicé un enfoque claro y estructurado para asegurar que los conceptos de ingeniería fueran comprensibles para todos los asistentes.<br><br>**Anthony Botello** <br>*TB1* <br>- En el vídeo de exposición se indicaron a los competidores, así como también se explicó la matriz DAFO de nuestra organización. Finalmente, se expusieron resultados acerca de las entrevistas realizadas.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- Durante mi exposición, comuniqué de manera clara y objetiva los resultados de mi proyecto en ingeniería, destacando la fase de Needfinding. Presenté User Personas y una matriz de tareas de usuario, usando herramientas como Empathy Mapping y As-is Scenario Mapping. Además, delineé el escenario futuro de la plataforma propuesta, detallando User Stories, Impact Mapping y un Product Backlog completo.<br><br>**Abel Angel Cierto Espiritu**<br>*TB1* <br>- Durante el desarrollo de este primer avance, comunique de manera eficaz el objetivo del diseño al desarrollar la aplicación web. También, detalle acerca de las funcionalidades primarias  que considero que son importantes y definir los atributos de calidad para una buena aplicación es necesaria. Los constraints nos sirven para tener claro las limitaciones del sistema al momento de desarrollar la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, me enfoqué en comunicar nuestros avances y resultados de manera clara y objetiva. Presenté nuestras ideas durante el proceso de Event Storming y facilité discusiones sobre el modelado de flujo de mensajes del dominio. Mi objetivo era asegurarme de que todos los miembros del equipo, independientemente de su especialidad o nivel jerárquico, comprendieran el progreso y las decisiones tomadas en el proyecto.<br><br>  | *TB1*<br>En la exposición de la presente entrega se comunico eficientemente las bases del proyecto desarrollado y el proceso que llevo a corroborar que efectivamente es una solución adecuada para la problemática encontrada. Asimismo, se presentaron las herramientas para utilizadas para las primeras fases de implementación del proyecto y su planteamiento. |
| Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.. | **José Carlos Vara**<br>*TB1* <br>- Redacté de manera clara y precisa los puntos del perfil de la startup y la solución propuesta, incluyendo antecedentes, problemática y el proceso Lean UX. Adapté el lenguaje técnico para que fuera accesible a un público de distintas especialidades y niveles jerárquicos, asegurando que la información se presentara de forma objetiva y comprensible para todos los involucrados en el proyecto.<br><br>**Anthony Botello** <br>*TB1* <br>- Se redactaron y documentó información y análisis de nuestros competidores y de la misma forma se evidenciaron las entrevistas realizadas y el análisis de ellas. Por otro lado, se definieron los Primary User Stories y los Quality Attribute Scenarios.<br><br>**Rodrigo Alexander Sabino Ramirez** <br>*TB1* <br>- En la elaboración de la primera entrega, me centré en comunicar de manera precisa y objetiva aspectos específicos. Utilizando el concepto de Ubiquitous Language, desarrollé un lenguaje común que facilitó la comprensión entre los miembros del equipo y los stakeholders. Además, identifiqué las limitaciones (Constraints) del proyecto y elaboré un Architectural Drivers Backlog para guiar el diseño arquitectónico. <br><br>**Abel Angel Cierto Espiritu** <br>*TB1* <br>- Los resultados de elegir drivers de arquitecturas permite un buen funcionamiento en la escalabilidad y mantenimiento del sistema. Por último los escenarios de los atributos que se requiere refinar permite una mejora continua en la aplicación web.<br><br>**Branco Alberto Villegas Peralta**<br>*TB1*<br>- Durante el proyecto, utilicé herramientas como EventStorming para explorar y descubrir los contextos relevantes. Luego, modelé los flujos de mensajes del dominio para comprender las interacciones entre los diferentes componentes del sistema. Utilicé Bounded Context Canvases para delinear los límites y responsabilidades de cada contexto, y realicé un mapeo de contextos para visualizar las relaciones entre ellos. Finalmente, documenté nuestra arquitectura de software utilizando varios diagramas, incluidos contexto, contenedor y despliegue, para comunicar nuestra visión de manera efectiva a todas las partes interesadas. | *TB1*<br>En el informe se detalló los aspectos más importantes acerca de la base de la solución propuesta y las herramientas que se usaron para validar la misma. Por otro lado, se incluyeron los diagramas adecuados para cada sección con su respectiva descripción para brindar la mayor cantidad de información.                                                |

---

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

SmartRent es una innovadora startup tecnológica enfocada en revolucionar el mercado del alquiler de viviendas a través de la integración de tecnologías emergentes. Su producto principal, CasaFinder, es una plataforma web diseñada para conectar de manera eficiente a propietarios de inmuebles interesados en alquilar sus propiedades con personas que buscan un hogar temporal o permanente. Lo que distingue a CasaFinder es su uso pionero de la tecnología blockchain, que garantiza la transparencia, seguridad y cumplimiento de los contratos de alquiler, al tiempo que crea un historial de cumplimiento de alquileres inmutable y confiable para ambas partes.

##### MISIÓN

Nuestra misión en SmartRent es simplificar y asegurar el proceso de alquiler de viviendas mediante la tecnología, ofreciendo una plataforma que garantice la confianza y la transparencia para propietarios e inquilinos por igual. Nos esforzamos por transformar la experiencia del alquiler en una transacción más accesible, eficiente y justa, aprovechando el poder de la tecnología blockchain para garantizar el cumplimiento de los acuerdos y la creación de un historial de arrendamientos confiable.

##### VISIÓN

Nuestra visión es convertirnos en la plataforma líder mundial en alquiler de viviendas, redefiniendo los estándares de confianza y eficiencia en el mercado inmobiliario. Aspiramos a que CasaFinder sea el estándar global para el alquiler de viviendas, ofreciendo una solución innovadora y segura que transforme la manera en que las personas encuentran y alquilan sus hogares, impulsando un futuro donde el proceso de arrendamiento sea tan simple y confiable como hacer una compra en línea.

### 1.1.2. Perfiles de integrantes del equipo

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |  José Carlos Vara Quispe                   |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------- |
| Soy José Carlos Vara Quispe,tengo 26 años, nací en Lima. Entre este ciclo a la UPC en la carrera de ingeniería de sistemas. Me gusta escuchar música, jugar videojuegos y salir con mis amigos. Me considero una persona puntual, respetuosa y responsable.
 | ![Jose Perfil](img/integrantes/jose.jpg) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                 | Grecia Carolina Guerrero Alegría       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Tengo 21 años y soy estudiante de Ingeniería de Software con conocimientos de matemática y habilidades en programación en el lenguaje C++. Actualmente curso el sétimo ciclo de la carrera y mi meta es ser un profesional destacado el cual rija sus decisiones por sus valores y el bien de la cliente donde labore. Me interesa el desarrollo de la tecnología y los avances que existen en la inteligencia artificial. | ![Anthony Perfil](img/integrantes/anthony.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                           | Michael Carrillo Mainicta              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Estudiante de la carrera de ingeniería de software, actualmente cursando el 9no ciclo. Me considero una persona entusiasta que le gusta aprender y desarrollar nuevas habilidades, lo cual me ha ayudado a adquirir conocimientos en lenguajes como Python, C++ y C#. Así mismo, me apasiona explorar nuevas tecnologías como Realidad Virtual (VR) y Realidad Aumentada (AR) y a su vez buscar soluciones innovadoras con las mismas. | ![Michael Perfil](img/integrantes/Michael.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Farid Hinostroza Mavila             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Estudiante de Ingeniería de Software con un interés particular en la inteligencia artificial y la gestión de bases de datos. Mi enfoque es la mejora continua y la implementación de soluciones innovadoras que resuelvan problemas reales. Además, soy proactivo y colaborativo, lo que me permite trabajar eficazmente en equipo para alcanzar los objetivos propuestos, siempre con la vista puesta en la excelencia y la eficiencia del proyecto.
| ![Farid Perfil](img/integrantes/Farid.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Rondon Añaños, Cristopher              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Estudiante de la carrera de Ingeniería en Software. Soy una persona dinámica y curiosa, siempre dispuesta a adquirir nuevas habilidades y conocimientos. Esta actitud me ha permitido familiarizarme con herramientas y lenguajes como Java, JavaScript y SQL. Además, me entusiasma investigar y experimentar con tecnologías emergentes como el Internet de las Cosas (IoT) y la Inteligencia Artificial (IA), con el objetivo de desarrollar soluciones creativas e impactantes en el campo tecnológico. | ![Cristopher Perfil](img/integrantes/CristopherPerfil.JPG) |

## 1.2. Solution Profile

Nombre del Producto: CasaFinder 

Tipo de Producto: Aplicación web para el alquiler de viviendas

### 1.2.1. Antecedentes y Problemática

##### ANTECEDENTES:

CEl mercado de alquiler de viviendas ha mostrado un crecimiento sostenido en las últimas décadas, influenciado por tendencias como la urbanización, la movilidad laboral y los cambios en las preferencias generacionales. La urbanización ha intensificado la demanda de viviendas en áreas urbanas, donde las personas buscan oportunidades económicas y experiencias culturales. Además, las nuevas generaciones, como los millennials y la Generación Z, tienden a priorizar la flexibilidad sobre la propiedad, prefiriendo opciones de alquiler que les permitan adaptarse a cambios rápidos en sus vidas personales y profesionales. Sin embargo, este crecimiento también ha expuesto problemas persistentes, como la falta de claridad en los contratos y el incumplimiento de pagos, que complican las transacciones entre propietarios e inquilinos y dificultan la construcción de relaciones de largo plazo en el mercado de alquiler.
Estas cuestiones se ven exacerbadas por la falta de un sistema estandarizado que permita a ambas partes verificar de manera confiable el historial de cumplimiento de los acuerdos, lo que genera desconfianza y aumenta la incidencia de disputas legales (Realty Boris, 2023; Virginia REALTORS®, 2023).

##### PROBLEMÁTICA

- **What(Qué)**
  CasaFinder aborda la falta de transparencia, seguridad y confianza en el proceso de alquiler de viviendas. Actualmente, no existe un sistema estandarizado que garantice el cumplimiento de los contratos de alquiler ni un historial confiable que documente el comportamiento de las partes involucradas.
- **When(Cuando)**
  El problema se manifiesta en todas las etapas del proceso de alquiler: desde la búsqueda de propiedades, la negociación y firma del contrato, hasta el seguimiento del cumplimiento del mismo.
- **Where(Dónde)**
  Este problema es global y afecta a todos los mercados de alquiler de viviendas, pero es particularmente grave en zonas urbanas con alta demanda y en mercados con regulaciones laxas o inexistentes.
- **Who(Quién)**
  Propietarios de viviendas: Que enfrentan riesgos financieros y legales debido al incumplimiento de los contratos y la falta de un sistema confiable que garantice el pago del alquiler.

  Inquilinos: Que experimentan inseguridad y desconfianza debido a la falta de transparencia en los contratos y a la dificultad para encontrar propietarios confiables.
- **Why(Por qué)**
  Resolver este problema es esencial para mejorar la confianza y seguridad en el mercado de alquiler de viviendas, reduciendo el riesgo de disputas legales, incumplimientos de contrato y pérdidas financieras, lo que resultará en un mercado más eficiente y justo para todas las partes.
- **How(Cómo)**
  CasaFinder utiliza la tecnología blockchain para crear contratos inteligentes, seguros y transparentes, que garantizan el cumplimiento de los términos acordados. Además, la plataforma genera un historial inmutable de cumplimiento de alquileres que permite evaluar la confiabilidad de propietarios e inquilinos.
- **How much(Cuánto)**
  El impacto del problema es significativo, afectando la estabilidad y eficiencia del mercado de alquiler de viviendas. Con CasaFinder, se espera una reducción sustancial en las disputas legales y en los riesgos financieros para ambas partes, así como una mejora considerable en la confianza mutua, lo que puede transformar positivamente el mercado de alquiler a nivel global.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

El mercado de alquiler de viviendas ha estado en constante crecimiento, impulsado por tendencias como la urbanización y el aumento de la movilidad laboral. Sin embargo, sigue enfrentando problemas significativos relacionados con la falta de transparencia, confianza y seguridad en las transacciones entre propietarios e inquilinos (Realty Boris, 2023; Virginia REALTORS®, 2023). Este dominio abarca todas las etapas del proceso de alquiler, desde la búsqueda de propiedades y la negociación de contratos hasta la firma y la gestión de la relación de alquiler. Los desafíos persisten, afectando tanto a los propietarios como a los inquilinos, y creando una necesidad urgente de una solución más confiable y eficiente (Gyourko et al., 2022).

Por un lado, los propietarios de viviendas enfrentan dificultades para encontrar inquilinos confiables y asegurar el cumplimiento de los contratos. Están constantemente expuestos al riesgo de incumplimiento de pago y carecen de herramientas efectivas para gestionar disputas legales de manera eficiente (Molloy et al., 2022). Por otro lado, los inquilinos sufren por la falta de transparencia en los términos de los contratos y la dificultad de encontrar propietarios que les ofrezcan seguridad y cumplimiento de los acuerdos. Esta inseguridad puede dejarlos en situaciones de vulnerabilidad, especialmente cuando se encuentran con propietarios que no respetan los términos acordados (Realty Boris, 2023).

Existe una brecha significativa en el mercado para una plataforma que integre tecnología avanzada, como blockchain, que pueda ofrecer contratos seguros y transparentes, al mismo tiempo que proporciona un historial de cumplimiento de alquileres que fortalezca la confianza entre las partes. Actualmente, no hay una solución en el mercado que aborde de manera integral la necesidad de seguridad y transparencia en las transacciones de alquiler, lo que deja una gran oportunidad para una innovación que responda a estas necesidades críticas (Virginia REALTORS®, 2023).


#### 1.2.2.2. Lean UX Assumptions

##### Business Assumptions

- Creemos que nuestros clientes tienen la necesidad de: Encontrar una manera segura y transparente de alquilar viviendas que garantice el cumplimiento de los contratos y genere confianza entre propietarios e inquilinos.
- Estas necesidades se pueden resolver con: Una plataforma que utilice tecnología blockchain para crear contratos inteligentes, transparentes y seguros, además de ofrecer un historial de cumplimiento de alquileres verificable.
- Nuestros clientes principales son: Propietarios de viviendas que desean alquilar sus propiedades de manera confiable y segura, e inquilinos que buscan viviendas con la certeza de que sus derechos serán respetados y los términos del contrato serán cumplidos.
- El valor #1 que un cliente quiere de nuestros servicios: Es la seguridad en las transacciones y la confianza que genera un contrato respaldado por tecnología blockchain.
- El cliente también puede obtener estos beneficios adicionales: Un historial de cumplimiento de alquileres que les permite verificar la reputación de las partes involucradas, y herramientas para facilitar la gestión de contratos y pagos.
- Voy a adquirir la mayoría de mis clientes a través de: Campañas de marketing digital enfocadas en redes sociales, así como asociaciones estratégicas con inmobiliarias y plataformas de alquiler.
- Hare dinero a través de: Pagos por suscripción mensual o anual, así como comisiones por cada contrato de alquiler gestionado a través de la plataforma.
- Mis competencias principales en el mercado serán: Airbnb, Zillow y otros servicios de alquiler de viviendas que no ofrecen la misma seguridad en los contratos y confianza entre las partes.
- Los venceremos con: Una experiencia de usuario superior, respaldada por la seguridad y transparencia que ofrece la tecnología blockchain, además de un enfoque en la creación de un historial de cumplimiento de alquileres confiable.
- Mi mayor riesgo de producto es: No lograr que suficientes propietarios e inquilinos adopten la plataforma debido a la complejidad percibida de la tecnología blockchain o la falta de confianza inicial en un nuevo servicio.
- Resolveremos esto a través de: Una campaña de educación y marketing que explique claramente los beneficios de blockchain y cómo CasaFinder ofrece una solución más segura y confiable en comparación con las plataformas tradicionales.

##### User Assumptions

- ¿Quién es el usuario?: Usuarios mayores de edad con acceso a internet que necesitan alquilar una vivienda o propietarios que desean alquilar sus propiedades de manera segura y confiable.
- ¿Dónde encaja nuestro producto en su vida?: CasaFinder se integra en la vida de los usuarios en el momento en que necesitan asegurar una transacción de alquiler confiable, ya sea para alquilar una vivienda o para garantizar que su propiedad sea arrendada sin problemas.
- ¿Qué problemas resuelve nuestro producto?: CasaFinder resuelve la falta de transparencia y seguridad en los contratos de alquiler, reduciendo la posibilidad de incumplimiento y conflictos legales, y creando un entorno de confianza mutua entre propietarios e inquilinos.
- ¿Cuándo y cómo es usado nuestro producto?: CasaFinder se utiliza durante todo el proceso de alquiler, desde la búsqueda de propiedades, la negociación y firma de contratos, hasta la gestión continua de la relación de alquiler. La plataforma es accesible a través de una aplicación web, permitiendo a los usuarios gestionar sus alquileres de manera conveniente y segura.
- ¿Qué características son importantes?: Es crucial que CasaFinder ofrezca seguridad en las transacciones, autenticación confiable, persistencia de datos, y una experiencia de usuario intuitiva que facilite la gestión de alquileres y el cumplimiento de contratos.
- ¿Cómo debe verse nuestro producto y comportarse?: CasaFinder debe ser estéticamente atractivo, intuitivo de usar, y confiable en todas sus funciones. La plataforma debe inspirar confianza y ser percibida como una solución moderna y segura para el alquiler de viviendas.

##### Features

- La aplicación permitirá a los usuarios visualizar propiedades disponibles y verificar el historial de cumplimiento de alquileres de propietarios e inquilinos.
- CasaFinder ofrecerá contratos inteligentes basados en blockchain que se ejecutan automáticamente cuando se cumplen los términos acordados.
- Los usuarios podrán comunicarse directamente a través de la plataforma para negociar términos y resolver cualquier duda.
- CasaFinder proporcionará una autenticación segura y un proceso de pago confiable para todas las transacciones de alquiler.
- La plataforma reducirá la complejidad y los riesgos asociados con las transacciones de alquiler al ofrecer herramientas para gestionar contratos y realizar pagos de manera segura y eficiente.

##### Business Outcomes

- Ser reconocidos como la plataforma más segura y confiable para el alquiler de viviendas.
- Desarrollar una aplicación que ofrezca una excelente experiencia de usuario, mejorando continuamente con el feedback recibido.
- Incrementar la cantidad de usuarios registrados y activos mediante estrategias de marketing digital y asociaciones estratégicas.
- Lograr que la mayoría de los alquileres realizados a través de CasaFinder se completen sin problemas, con altos niveles de satisfacción entre propietarios e inquilinos.

##### User Outcomes

Para Propietarios:

- Satisfacer su necesidad de alquilar propiedades de manera segura y confiable.
- Reducir riesgos asociados con el incumplimiento de contratos y gestionar fácilmente los términos de alquiler.
- Sentir mayor seguridad al autenticarse o realizar transacciones mediante CasaFinder.

Para Inquilinos:

- Encontrar viviendas que se ajusten a sus necesidades con la certeza de que los términos del contrato serán respetados.
- Acceder fácilmente a un historial verificable de cumplimiento de alquileres para tomar decisiones informadas.
- Realizar pagos de alquiler de manera rápida y segura a través de la plataforma.

#### 1.2.2.3. Lean UX Hypothesis Statements

-	**Creemos** los propietarios de viviendas valoran la seguridad y transparencia en las transacciones de alquiler y estarán dispuestos a utilizar una plataforma que ofrezca contratos inteligentes respaldados por blockchain.
**Sabremos** que hemos tenido éxito
**Cuando** al menos el 40% de los propietarios registrados en CasaFinder crean contratos a través de la plataforma y un 60% de ellos continúan utilizando el servicio para futuros alquileres dentro de los primeros seis meses.

-	**Creemos** los inquilinos buscan una manera confiable y segura de alquilar viviendas y estarán motivados a usar CasaFinder para evitar riesgos asociados con contratos tradicionales. 
**Sabremos** que hemos tenido éxito
**Cuando** al menos el 50% de los inquilinos que utilizan CasaFinder completan su alquiler a través de la plataforma y un 70% de ellos recomiendan el servicio a otros, reflejado en un aumento del 20% en nuevos registros basados en referencias.

-	**Creemos** la tecnología blockchain aumentará la confianza de los usuarios en la plataforma, al proporcionar un historial inmutable de cumplimiento de alquileres.
**Sabremos** que hemos tenido éxito
**Cuando** un 80% de los usuarios confían en el historial de cumplimiento de alquileres al tomar decisiones, con una reducción del 25% en disputas legales y problemas relacionados con el incumplimiento de contratos en comparación con el método tradicional.

-	**Creemos** una interfaz de usuario intuitiva y un proceso de autenticación seguro atraerán y retendrán tanto a propietarios como a inquilinos.
**Sabremos** que es cierto
**Cuando** al menos el 85% de los usuarios completan el proceso de registro sin dificultades, con un índice de abandono inferior al 10% durante el registro y un 75% de usuarios activos después de tres meses de uso. al menos el 85% de los usuarios completan el proceso de registro sin dificultades, con un índice de abandono inferior al 10% durante el registro y un 75% de usuarios activos después de tres meses de uso.


-	**Creemos** la publicidad en redes sociales y las asociaciones estratégicas con inmobiliarias atraerán a un número creciente de usuarios a la plataforma.
**Sabremos** que es cierto
**Cuando** el número de nuevos registros aumenta en un 30% mes a mes durante los primeros seis meses, alcanzando el objetivo de 10,000 usuarios activos al final de este período.

-	**Creemos** ofrecer beneficios adicionales, como herramientas de gestión de contratos y pagos, aumentará el valor percibido de la plataforma y la satisfacción del usuario.
**Sabremos** que estamos en lo correcto
**Cuando** veamos que al menos el 50% de los usuarios utilizan estas herramientas regularmente, y un 70% reportan una mayor satisfacción general, con un índice de renovación de suscripciones del 60% al término del primer año.

#### 1.2.2.4. Lean UX Canvas

| **LEAN UX CANVAS**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | **Lean UX Canvas**                                                                                                                                                                                                                                                                                                                                                                                                                                | *Fecha: 08/09/2024* *Iteración: 1*                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Business problem**<br><br>Falta de seguridad y transparencia en las transacciones de alquiler. Desconfianza entre propietarios e inquilinos al firmar contratos. Dificultad para verificar el historial de cumplimiento de alquileres. Riesgo de disputas legales debido a contratos tradicionales mal gestionados. Adopción lenta de nuevas tecnologías como blockchain en el mercado de alquiler.<br><br>                                                                                                                                                                                                                                                        | **5.Solutions**<br><br>Contratos inteligentes: Basados en blockchain para asegurar transparencia y cumplimiento automático. Historial de cumplimiento: Registro inmutable de comportamiento en alquileres para evaluar la confiabilidad. Interfaz intuitiva: Fácil de usar, con procesos de autenticación seguros. Herramientas de gestión: Para facilitar la administración de contratos y pagos. Marketing digital: Estrategias en redes sociales y asociaciones con inmobiliarias para atraer usuarios.                                                                                 | **2.Business Outcomes**<br>Incremento del 40% en contratos de alquiler creados en la plataforma. Retención del 60% de propietarios y 70% de inquilinos satisfechos. Reducción del 25% en disputas legales relacionadas con contratos. Crecimiento mensual del 30% en nuevos registros, alcanzando 10,000 usuarios activos en 6 meses. Renovación del 60% de suscripciones al finalizar el primer año.                                                                                                                                                                       |
| **3. User**<br><br>Propietarios de viviendas que buscan alquilar de manera segura y confiable. Inquilinos que necesitan una plataforma transparente y confiable para encontrar y alquilar viviendas.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                   | **4. User outcomes & benefits**<br><br>Propietarios: Alquiler seguro, con contratos claros y reducción de riesgos de incumplimiento. Inquilinos: Transparencia en los términos de alquiler y confianza en la relación con el propietario. Ambos: Acceso a un historial de cumplimiento que facilita decisiones informadas y reduce disputas.      |
| **6. Hypotheses**<br><br>Creemos que los propietarios valoran la seguridad y transparencia, y usarán contratos blockchain en CasaFinder. Éxito cuando: El 40% de los propietarios crean contratos y el 60% repiten en 6 meses. Creemos que los inquilinos buscan una plataforma confiable y segura para alquilar viviendas. Éxito cuando: El 50% completa su alquiler y el 70% recomienda CasaFinder. Creemos que blockchain aumentará la confianza en la plataforma. Éxito cuando: El 80% confía en el historial de cumplimiento y las disputas se reducen en un 25%.  | **7. ¿Qué es lo más importante que      necesitamos aprender primero?**<br> <br> Validación del interés en contratos blockchain: ¿Propietarios e inquilinos valoran y adoptarán la tecnología blockchain para alquileres? Aceptación de la plataforma: ¿Los usuarios encuentran la plataforma intuitiva y confiable? Demanda real: ¿Existe un mercado significativo dispuesto a usar CasaFinder para sus alquileres?  | **8. ¿Cuál es la menor cantidad de trabajo que debemos hacer para aprender la siguiente cosa más importante?**<br><br>Prototipo funcional de contratos inteligentes: Crear y probar un prototipo que muestre cómo funcionarán los contratos blockchain en la plataforma. Pruebas de usabilidad: Desarrollar una versión básica de la interfaz y realizar pruebas de usabilidad con un grupo reducido de usuarios. Campaña de marketing inicial: Lanzar una campaña piloto en redes sociales para medir el interés y obtener retroalimentación inicial sobre CasaFinder. |

## 1.3. Segmentos Objetivo
Dentro de nuestro segmento objetivo, hemos identificado dos grupos de usuarios distintos:
##### Segmento Propietarios de Viviendas
Este grupo incluye tanto a individuos que poseen propiedades residenciales como a pequeños y medianos inversionistas que manejan varios inmuebles destinados al alquiler. Los propietarios en Perú suelen estar entre los 35 y 60 años, y muchos de ellos ven el alquiler de inmuebles como una fuente de ingresos adicional. Según el Instituto Nacional de Estadística e Informática (INEI) de Perú, el 16% de los propietarios en el país alquilan al menos una propiedad (INEI, 2021), y este porcentaje es más alto en áreas urbanas como Lima, donde la demanda de alquileres es más alta.
CasaFinder ofrece una plataforma que no solo facilita la búsqueda de inquilinos confiables, sino que también asegura el cumplimiento de los contratos mediante el uso de tecnología blockchain. Esto les brinda una mayor tranquilidad y reduce los riesgos asociados con el alquiler, proporcionando herramientas para gestionar contratos y pagos de manera eficiente y segura. Según un reporte de Credicorp Capital, el valor promedio de la renta de departamentos en Lima alcanzó un precio histórico de S/2.900 mensual en marzo de 2023, lo que refleja una alta demanda en el mercado (Montoro, 2023).

##### Segmento Inquilinos
El segmento de inquilinos en Perú incluye a personas que buscan vivienda por motivos laborales, educativos o familiares. A nivel demográfico, los inquilinos suelen estar en el rango de edad de 18 a 45 años, con una gran proporción concentrada en áreas urbanas como Lima, Trujillo y Arequipa. Según el INEI, el 25% de los hogares en Lima Metropolitana están ocupados por inquilinos (INEI, 2021), debido a factores como la migración interna y el aumento de precios en el mercado inmobiliario.
CasaFinder ofrece a los inquilinos la posibilidad de acceder a contratos claros y protegidos por la tecnología blockchain, lo que asegura que los términos acordados se cumplirán y que sus derechos estarán protegidos. Además, el acceso a un historial verificable de cumplimiento de alquileres les permite tomar decisiones informadas sobre a quién alquilar, reduciendo el riesgo de acuerdos desfavorables. En cuanto a la demanda de alquileres, distritos como Miraflores, Santiago de Surco y San Isidro lideran las búsquedas de departamentos en Lima, según Properati, con más de un millón de visitas en los primeros meses de 2023 (Montoro, 2023).


---

# Capítulo II: Requirements Elicitation & Analysis
## 2.1. Competidores
### 2.1.1. Análisis Competitivo

![Analisis Competitivo - Tabla](img/Capitulo_2/Competidores/Imagen1.png)

### 2.1.2. Estrategias y tácticas frente a competidores

Para enfrentar a la competencia y maximizar el éxito de CasaFinder, se implementarán varias estrategias y tácticas clave. En primer lugar, CasaFinder se diferenciará al utilizar tecnología blockchain para crear contratos inteligentes, ofreciendo una solución única en el mercado que garantiza seguridad y transparencia. Para apoyar esta estrategia, se llevarán a cabo campañas educativas que informen a los usuarios sobre los beneficios de blockchain, incluyendo seminarios web, talleres y la presentación de casos de éxito que demuestren la efectividad de esta tecnología en la reducción de disputas legales.

Además, CasaFinder se enfocará en expandirse rápidamente en mercados emergentes y áreas urbanas con alta demanda de alquileres, donde la competencia es menos intensa. La estrategia incluirá campañas de marketing localizadas, asociaciones con inmobiliarias locales y desarrolladores de propiedades, así como incentivos para atraer a los primeros usuarios. Esto permitirá a CasaFinder establecer una fuerte presencia en estos mercados desde el principio.

Otra táctica clave será la optimización de la experiencia del usuario, asegurando que CasaFinder ofrezca una interfaz intuitiva y moderna que haga que la gestión de alquileres sea sencilla y accesible para todos los usuarios. Se realizarán pruebas de usabilidad constantes y se incorporará retroalimentación de los usuarios para mejorar la plataforma continuamente y adaptarla a sus necesidades cambiantes.

En cuanto a la visibilidad y captación de usuarios, CasaFinder aprovechará alianzas estratégicas y una fuerte presencia en marketing digital. Esto incluirá asociaciones con empresas de tecnología financiera para integrar soluciones de pago seguras, publicidad segmentada en redes sociales, y un programa de referidos que incentive a los usuarios actuales a invitar a otros, generando un efecto de red que aumente rápidamente la base de usuarios.

Finalmente, CasaFinder mantendrá la flexibilidad operativa para adaptarse rápidamente a las regulaciones y cambios en el mercado. Se monitorearán activamente las regulaciones que puedan impactar el uso de blockchain, y se desarrollarán políticas de cumplimiento que aseguren que la plataforma siempre opere dentro de los marcos legales. Un equipo de respuesta rápida estará preparado para modificar características de la plataforma según sea necesario, asegurando que CasaFinder siga siendo competitiva y relevante en un entorno de mercado en constante evolución.

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

## 2.3. Needfinding

Los User Personas son fundamentales para el éxito del proyecto, ya que brindan una comprensión profunda y concreta de las necesidades, deseos, frustraciones y comportamientos de los usuarios clave. Estos perfiles detallados permiten a la startup diseñar una plataforma y experiencia de aprendizaje altamente enfocada y personalizada, abordando de manera efectiva los desafíos específicos de cada segmento objetivo: desde brindar recursos claros y accesibles a aficionados, hasta ofrecer herramientas para que los expertos compartan su conocimiento.

### 2.3.1. User Personas

Para comprender mejor a los usuarios a los que está dirigida nuestra solución, hemos identificado y perfilado dos grupos clave de usuarios: el Propietario de Viviendas y el Inquilino en Búsqueda de Alquiler. Estos perfiles de User Persona nos permiten visualizar sus necesidades, comportamientos y desafíos específicos, ayudándonos a diseñar una solución que realmente responda a sus expectativas y resuelva sus problemas de manera efectiva. De esta forma, podemos asegurarnos de que CasaFinder ofrezca una experiencia óptima tanto para los propietarios que buscan gestionar sus propiedades, como para los inquilinos que buscan un proceso de alquiler transparente y sin complicaciones.

- **Arrendador:** Poseen propiedades y desean alquilarlas de manera eficiente y segura. Buscan una plataforma que les permita gestionar los pagos, contratos y verificación de inquilinos de manera sencilla, minimizando los riesgos de retrasos o conflictos legales.


<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282503193598754969/userArrendador.png?ex=66df97ad&is=66de462d&hm=f967a5e30adef234110a58c615439f5f3feefba169c6880681902ddaf6b68f03&=&format=webp&quality=lossless&width=656&height=1034" alt="arrendador"/>
</div>

<br>

- **Inquilino:** Personas jóvenes, entre 25 y 35 años, que buscan alquilar una vivienda sin complicaciones. Prefieren una solución confiable, transparente y que automatice procesos como los pagos, garantizando que el alquiler se realice de manera fluida y sin sorpresas.

<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282503239677247561/userInquilino.png?ex=66df97b8&is=66de4638&hm=31615c635e1aabbe94752c8038710ae36b6f72486419cb5640ba4e71c4d2013f&=&format=webp&quality=lossless&width=708&height=1034"/>
</div>

<br>

### 2.3.2. User Task Matrix

El User Task Matrix es una herramienta clave que recopila y analiza las tareas fundamentales que los usuarios de CasaFinder realizan, tanto Propietarios como Inquilinos. Este cuadro se enfoca en evaluar con qué frecuencia los usuarios llevan a cabo cada una de estas tareas y el impacto que estas tienen en su éxito. 
Al identificar estas áreas clave, CasaFinder podrá desarrollar soluciones que faciliten la vida de los usuarios y maximicen la eficiencia en el proceso de alquiler. Esto permite priorizar las necesidades más críticas de los usuarios y ofrecerles herramientas que realmente les ayuden a alcanzar sus objetivos de manera óptima.

### Propietarios

| **Tareas (Tasks)**                    | **Descripción de la Tarea**                                                                                         | **Objetivo Relacionado**                                             |
|---------------------------------------|---------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------|
| Publicar una propiedad en la plataforma | Subir fotos, descripción, precio y condiciones de alquiler de la propiedad en CasaFinder.                           | Aumentar la visibilidad de las propiedades y atraer más inquilinos potenciales. |
| Gestionar contratos de alquiler        | Crear, enviar y almacenar contratos de alquiler digitalmente a través de CasaFinder.                                | Simplificar la administración de contratos y asegurar cumplimiento legal. |
| Verificar el historial de inquilinos    | Acceder a la información y antecedentes de los inquilinos potenciales mediante la plataforma.                        | Seleccionar inquilinos confiables y minimizar riesgos de impago o conflictos. |
| Automatizar pagos de alquiler          | Configurar pagos automáticos de los inquilinos a través de CasaFinder.                                              | Asegurar la puntualidad en la recepción de pagos y reducir la carga administrativa. |
| Comunicar con inquilinos                | Utilizar herramientas de mensajería integradas en CasaFinder para comunicarse con los inquilinos.                     | Mantener una comunicación efectiva y rápida con los inquilinos.      |
| Supervisar el estado de las propiedades | Monitorear el mantenimiento y estado general de las propiedades alquiladas a través de informes y notificaciones.      | Garantizar que las propiedades se mantengan en buenas condiciones y resolver problemas a tiempo. |
| Renovar o finalizar contratos           | Gestionar la renovación de contratos existentes o finalizar acuerdos de alquiler cuando sea necesario.                | Mantener la ocupación de las propiedades y gestionar adecuadamente los ciclos de alquiler. |

---

### Inquilinos

| **Tareas (Tasks)**                        | **Descripción de la Tarea**                                                                                                   | **Objetivo Relacionado**                                              |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|
| Buscar y filtrar propiedades disponibles  | Utilizar los filtros de CasaFinder para encontrar propiedades que se ajusten a sus necesidades y presupuesto.                   | Facilitar la búsqueda de viviendas adecuadas y ahorrar tiempo.       |
| Revisar información detallada de las propiedades | Consultar fotos, descripciones, precios y condiciones de alquiler de las propiedades listadas.                                 | Tomar decisiones informadas sobre qué propiedades visitar o alquilar.|
| Contactar a los propietarios              | Enviar mensajes o solicitudes a los propietarios para obtener más información o programar visitas a las propiedades.            | Establecer comunicación rápida y efectiva con los propietarios.      |
| Firmar contratos de alquiler              | Completar y firmar contratos de alquiler digitalmente a través de CasaFinder.                                                 | Simplificar el proceso de formalización del alquiler y asegurar la legalidad del acuerdo. |
| Realizar pagos de alquiler automáticos    | Configurar pagos recurrentes de alquiler mediante métodos de pago integrados en CasaFinder.                                    | Evitar retrasos en pagos y gestionar el alquiler de manera eficiente.|
| Gestionar solicitudes de mantenimiento    | Reportar problemas o solicitar mantenimiento a través de la plataforma CasaFinder.                                              | Asegurar el buen estado de la vivienda y resolver inconvenientes rápidamente. |
| Evaluar y dejar comentarios sobre la propiedad | Proporcionar retroalimentación y calificaciones sobre su experiencia con la propiedad y el propietario.                          | Ayudar a otros usuarios a tomar decisiones informadas y mejorar la calidad del servicio de CasaFinder. |


### 2.3.3. User Journey Mapping

El User Journey Mapping del Arrendador detalla el recorrido que realiza un propietario desde el momento en que se da cuenta de la necesidad de una plataforma para gestionar sus propiedades, hasta la evaluación final del impacto que esta tiene en la administración de su negocio de alquileres. A lo largo de este proceso, se identifican los pasos clave que el propietario sigue, sus emociones y desafíos, como la búsqueda de inquilinos confiables, la gestión de contratos y pagos, y la automatización de tareas administrativas. Este análisis nos permite detectar áreas de mejora y oportunidades para ofrecer una experiencia más fluida y eficiente, ayudando al propietario a maximizar el control y rentabilidad de sus propiedades.
Arrendador:


<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282503820546408609/JourneyArrendador.png?ex=66df9842&is=66de46c2&hm=7538e272d0b9008a09167fcb9811d2877eab9dadb33871d58fd0791fb75ed568&=&format=webp&quality=lossless&width=1208&height=1034"/>
</div>

<br>

El User Journey Mapping del Inquilino explora el camino que sigue un inquilino desde que comienza la búsqueda de una propiedad para alquilar, hasta la gestión del contrato y la evaluación del servicio. Este mapeo captura las etapas clave que el inquilino enfrenta, como la búsqueda de propiedades adecuadas, el contacto con propietarios, la firma de contratos y la gestión de pagos. Se analizan las emociones y desafíos a lo largo del proceso, como la frustración por falta de respuesta o propiedades desactualizadas, y se identifican oportunidades para mejorar la experiencia, ofreciendo soluciones más rápidas y automáticas para una gestión 

<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282503820227776512/JourneyInquilino.png?ex=66df9842&is=66de46c2&hm=4a14972ca9148c38f6004cfbea48b071f9b3852239e90078981f32ff62857434&=&format=webp&quality=lossless&width=1260&height=1034"/>
</div>

<br>

### 2.3.4. Empathy Mapping

El Empathy Mapping es una herramienta esencial que nos permite adentrarnos en la mente y el corazón de nuestros usuarios, capturando sus pensamientos, sentimientos, percepciones y comportamientos en relación con sus actividades cotidianas. A través de este proceso, podemos comprender mejor las motivaciones, frustraciones y deseos que impulsan a nuestros usuarios, lo que nos ayuda a diseñar soluciones que realmente resuenen con sus necesidades.

**Arrendador**
<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282504118744780912/EmpathyArrendador.png?ex=66df9889&is=66de4709&hm=0ccbe609534f3355ae6c02746986cbd93d9813c31893c0b2246db5ee3f6ff8f1&=&format=webp&quality=lossless&width=820&height=1034"/>
</div>

<br>

**Inquilino**
<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282504118388260995/Empathy_Inquilino.png?ex=66df9889&is=66de4709&hm=c03604ef718efe4f25f9cbbe448d75d2572070d2eb244bf99cf7f8b56f126591&=&format=webp&quality=lossless&width=820&height=1034"/>
</div>

### 2.3.5. As-is Scenario Mapping

El As-Is Scenario Mapping es una herramienta clave que utilizamos para comprender el flujo actual de actividades, pensamientos y emociones que experimentan nuestros usuarios en su contexto cotidiano, antes de la implementación de nuestra solución. Este mapeo captura cómo los usuarios interactúan con las tecnologías y procesos existentes, identificando los puntos de dolor, las oportunidades de mejora y las áreas donde nuestra solución podría tener el mayor impacto

**Arrendador**
<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282504365550211162/As_is_Arrendador.png?ex=66df98c4&is=66de4744&hm=3c9a5cdf766c7d4b2ba0b164e7cc725b0e728b45aed47c58ed52b5eb39765fac&=&format=webp&quality=lossless&width=1410&height=538"/>
</div>

<br>

**Inquilino**
<div align="center">
    <img src="https://media.discordapp.net/attachments/1282501864642052189/1282504365256740934/As_Is_Inquilino.png?ex=66df98c4&is=66de4744&hm=0149f65baa64b3e5550794458b04b93f377c7215092025673fe893cb815f8664&=&format=webp&quality=lossless&width=1410&height=520"/>
</div>

## 2.4. Ubiquitous Language

Este glosario de Ubiquitous Language está centrado en la aplicación de **blockchain** y **contratos inteligentes** en el contexto de los alquileres, con el objetivo de garantizar que todos los miembros del equipo y stakeholders compartan una comprensión clara y común de los términos clave relacionados con esta tecnología dentro del proyecto **CasaFinder**.

### Blockchain
**Definición**: Tecnología de registro distribuido que permite almacenar transacciones de manera segura, transparente y descentralizada. En el contexto de alquileres, permite registrar contratos y pagos de forma inmutable, evitando fraudes o alteraciones.

### Contrato Inteligente (Smart Contract)
**Definición**: Programa o protocolo autoejecutable almacenado en una blockchain, donde los términos del contrato de alquiler (como pagos, fechas, penalidades) se ejecutan automáticamente cuando se cumplen ciertas condiciones, eliminando la necesidad de intermediarios.

### Descentralización
**Definición**: Principio clave de blockchain donde la información no está controlada por una única entidad, sino que se distribuye entre varios nodos. En el contexto de alquileres, esto garantiza que las transacciones y contratos sean transparentes y resistentes a la manipulación.

### Inmutabilidad
**Definición**: Característica de blockchain que asegura que una vez que los datos, como contratos o transacciones, son registrados en la cadena, no pueden ser alterados. Esto proporciona seguridad y confianza en los contratos de alquiler.

### Oráculos
**Definición**: Servicios que permiten que los contratos inteligentes interactúen con datos externos fuera de la blockchain (como verificaciones de pago o estado del alquiler). Los oráculos garantizan que la información necesaria para ejecutar un contrato esté disponible y sea confiable.

### Tokenización del Alquiler
**Definición**: Proceso de representar un activo de alquiler (como una propiedad o un pago) a través de tokens en una blockchain. Estos tokens pueden ser utilizados para representar derechos de propiedad, derechos de alquiler o depósitos de garantía, facilitando la transferencia y el fraccionamiento de propiedades.

### Automatización de Pagos
**Definición**: Uso de contratos inteligentes para gestionar el pago de alquileres de forma automática, ejecutando transacciones directamente desde la cuenta del inquilino al propietario una vez que se cumplen las condiciones predefinidas (como la fecha de vencimiento).

### Depósito de Garantía en Blockchain
**Definición**: Representación del depósito de garantía de un inquilino como un token o contrato inteligente en blockchain. Esto asegura que el dinero quede bloqueado y solo se libere automáticamente cuando ambas partes estén de acuerdo en las condiciones, evitando disputas.

### Resolución de Disputas Automatizada
**Definición**: Uso de contratos inteligentes para manejar automáticamente las disputas entre propietario e inquilino. Las reglas predefinidas en el contrato inteligente pueden resolver problemas, como el incumplimiento de pagos o reparaciones, sin la necesidad de intervención humana.

### Auditoría Transparente
**Definición**: Capacidad que ofrece la blockchain de tener un registro auditable y transparente de todas las transacciones y contratos, permitiendo a las partes (propietarios, inquilinos, y terceros) revisar los acuerdos y asegurarse de que se están cumpliendo las condiciones de manera justa.

### Plataforma de Alquiler Descentralizada
**Definición**: Plataforma de gestión de alquileres basada en blockchain que permite a propietarios e inquilinos interactuar sin intermediarios, gestionando contratos, pagos, y disputas a través de contratos inteligentes y transacciones descentralizadas.

### Wallet Digital
**Definición**: Monedero digital que permite a los usuarios almacenar y transferir criptomonedas o tokens utilizados en la plataforma de alquiler. Los inquilinos pueden usar wallets para realizar pagos automatizados a través de contratos inteligentes.

### Identidad Digital Descentralizada
**Definición**: Sistema que permite a inquilinos y propietarios verificar sus identidades en la blockchain sin depender de una autoridad central. Esto facilita el acceso a la plataforma de alquiler de forma segura y con mayor privacidad.

### Penalizaciones Automáticas
**Definición**: Ejecución automática de penalizaciones o multas cuando se incumplen los términos del contrato inteligente, como retrasos en el pago del alquiler o el incumplimiento de condiciones previamente acordadas.

### Rentabilidad Tokenizada
**Definición**: Proceso mediante el cual los ingresos por alquiler se distribuyen automáticamente a través de tokens en la blockchain, permitiendo a los propietarios recibir ingresos de manera más rápida y eficiente.

<br>


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

![Impact Mapping](img/Capitulo_3/ImpactMap.png)
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

