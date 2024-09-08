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
| Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.     |  |
| Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerarquicos, en el marco del desarrollo de un proyecto en ingeniería.. |  |                                               |

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
| Estudio Ingeniería de Software porque me apasiona solucionar problemas de la vida real usando la tecnología. Los conocimientos técnicos con los que aportaré a este grupo son Java, Spring boot, MySql y React. Considero que mis habilidades son ser autodidacta, responsable y colaborativa con lo cual espero complementar bien a mi equipo. | ![Grecia Perfil](img/integrantes/Grecia.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                           | Michael Carrillo Mainicta              |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| Estudiante de la carrera de ingeniería de software, actualmente cursando el 9no ciclo. Me considero una persona entusiasta que le gusta aprender y desarrollar nuevas habilidades, lo cual me ha ayudado a adquirir conocimientos en lenguajes como Python, C++ y C#. Así mismo, me apasiona explorar nuevas tecnologías como Realidad Virtual (VR) y Realidad Aumentada (AR) y a su vez buscar soluciones innovadoras con las mismas. | ![Michael Perfil](img/integrantes/Michael.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Farid Hinostroza Mavila             |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| Estudiante de Ingeniería de Software con un interés particular en la inteligencia artificial y la gestión de bases de datos. Mi enfoque es la mejora continua y la implementación de soluciones innovadoras que resuelvan problemas reales. Además, soy proactivo y colaborativo, lo que me permite trabajar eficazmente en equipo para alcanzar los objetivos propuestos, siempre con la vista puesta en la excelencia y la eficiencia del proyecto.
 | ![Farid Perfil](img/integrantes/Farid.png) |

| Integrante                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Cristopher Rondon Añaños              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| Estudiante de la carrera de Ingeniería en Software. Soy una persona dinámica y curiosa, siempre dispuesta a adquirir nuevas habilidades y conocimientos. Esta actitud me ha permitido familiarizarme con herramientas y lenguajes como Java, JavaScript y SQL. Además, me entusiasma investigar y experimentar con tecnologías emergentes como el Internet de las Cosas (IoT) y la Inteligencia Artificial (IA), con el objetivo de desarrollar soluciones creativas e impactantes en el campo tecnológico | ![Cristopher Perfil](img/integrantes/Cristopher.png) |

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