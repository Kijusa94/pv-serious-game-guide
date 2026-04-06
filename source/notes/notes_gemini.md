# Guía Diseño Sistemas Fotovoltaicos RV

**Exported:** 4/6/2026 14:38:03  
**Link:** [https://gemini.google.com/app/3c2ea70e8415aa39?hl=es](https://gemini.google.com/app/3c2ea70e8415aa39?hl=es)

## Prompt:
> evaluacion_jurado_1 - PDF

> draft_app_guide - DOCX

> evaluacion_jurado_2 - PDF

> anteproyecto - PDF

Requiero que te comportes como un investigador academico en el area de la Ingeniería, particularmente, Ingeniería Industrial y electrica.

Requiero generar una guía de laboratorio considerando los adjuntos.

Requiero ser detallado con las descripciones y la información de cada sección, dado que son estudiantes de 4to semestre que solo conocen los fundamentos de la electricidad.

## Response:
¡Hola! Es un excelente proyecto. Como investigador y docente en ingeniería, entiendo perfectamente el reto: los estudiantes de cuarto semestre ya tienen bases de electricidad, pero necesitan una estructura muy clara y pedagógica para conectar esos conceptos abstractos con el diseño de sistemas reales.

A continuación, te presento una propuesta detallada de la guía de laboratorio, estructurada para ser comprensible, rigurosa y alineada con la metodología de evaluación basada en herramientas de realidad virtual (RV).

* * *

GUÍA DE LABORATORIO: Diseño de Sistemas Fotovoltaicos mediante Simulación en Realidad Virtual
=============================================================================================

1\. Propósito de la Práctica
----------------------------

Evaluar la efectividad del videojuego educativo en realidad virtual como herramienta de aprendizaje para comprender el dimensionamiento básico de sistemas fotovoltaicos, análisis energético y toma de decisiones técnicas. Se espera que los estudiantes relacionen la teoría energética con decisiones prácticas y comprendan el diseño fotovoltaico como un sistema integral.

+1

2\. Perfil de los Participantes
-------------------------------

Esta práctica está diseñada para estudiantes de ingeniería con conocimientos básicos en análisis cuantitativo y procesos energéticos.

3\. Marco Teórico Básico
------------------------

Antes de ingresar al entorno de realidad virtual, es fundamental recordar los principios de los sistemas que vamos a dimensionar:

*   **Energía Fotovoltaica:** La energía solar fotovoltaica convierte la radiación solar directamente en energía eléctrica mediante el efecto fotovoltaico. Este es un fenómeno físico en el que la luz solar excita los electrones en materiales semiconductores, generando una corriente eléctrica.
*   **Estructura Física:** Los paneles solares están compuestos por módulos fotovoltaicos que incluyen múltiples células solares. Varias células interconectadas forman un módulo. A su vez, las matrices fotovoltaicas están formadas por varios módulos conectados.
    +2
*   **Conexiones Eléctricas:** Los módulos pueden conectarse en serie (denominadas "cadenas") o en paralelo (llamadas "bloques"). En la configuración en serie, el voltaje total del sistema aumenta, mientras que en la configuración en paralelo se incrementa la corriente.
    +1
*   **Componentes de un Sistema Autónomo:** Estos sistemas incluyen componentes como generadores fotovoltaicos, inversores, reguladores de carga y baterías. Estos elementos aseguran el almacenamiento y la distribución de la energía para consumos tanto en corriente directa (DC) como en corriente alterna (AC).
    +1

4\. Recursos del Laboratorio
----------------------------

Para el desarrollo de esta práctica en el laboratorio, se requerirá:

*   **Hardware:** Gafas Meta Quest 2 o 3, un PC con Unity (modo simulación opcional) y un área segura para el movimiento en RV.
*   **Software:** Versión estable del "serious game", sistema de puntuación activo y registro de resultados.
*   **Material de Apoyo:** Consentimiento informado, encuesta pre y post prueba, y hoja de observación del evaluador.

5\. Procedimiento Matemático de Diseño (Flujo del Sistema)
----------------------------------------------------------

Durante la experiencia inmersiva, el estudiante deberá tomar decisiones de diseño siguiendo estas 8 etapas secuenciales:

+1

### Etapa 1: Análisis de Cargas (Consumo)

Se debe calcular cuánta energía consumen los equipos a conectar.

*   Se requieren los datos de potencia nominal (W) y tiempo de operación (h).
*   La fórmula a aplicar es:
    $$
    Energıˊa=Potencia\times Tiempo
    $$

### Etapa 2: Conversión de Cargas AC a DC

Dado que los paneles y baterías operan en corriente directa (DC), debemos convertir el consumo de los electrodomésticos convencionales (AC) a DC, asumiendo una pérdida por el uso del inversor.

*   La energía AC equivalente en DC se calcula dividiendo la energía de las cargas AC por la eficiencia del inversor.
*   Para este cálculo, la eficiencia del inversor se estima en un 90%.
*   La ecuación es:
    $$
    Energıˊa_{AC\to DC}=\frac{Energıˊa_{AC}}{0.9}
    $$

### Etapa 3: Energía Total Diaria

*   Se suman las necesidades energéticas obtenidas en las etapas anteriores:
    $$
    Energıˊa_{Total}=Energıˊa_{DC}+Energıˊa_{AC\to DC}
    $$

### Etapa 4: Selección de Tensión Nominal del Sistema

*   Se debe elegir a qué voltaje operará el banco de baterías: 12 V, 24 V o 48 V.
*   Con este dato, se calcula el requerimiento de carga diaria en Amperios-hora (Ah):
    $$
    Requerimiento_{diario}\left(Ah/dia\right)=\frac{Energıˊa_{Total}\left(Wh/dia\right)}{Tensioˊn_{nominal}\left(V\right)}
    $$

### Etapa 5: Factor de Pérdidas del Sistema

Los cables, conexiones y el regulador tienen pérdidas naturales.

*   Se estima una eficiencia del sistema del 90%, lo que representa una pérdida del 10%.
*   La fórmula para la demanda final ajustada es:
    $$
    Demanda_{final}=\frac{Requerimiento_{diario}\left(Ah/dia\right)}{0.9}
    $$

### Etapa 6: Corriente del Arreglo Fotovoltaico

Se requiere calcular la corriente total que deben inyectar los paneles usando el concepto de Horas de Sol Equivalente (ESH).

*   La fórmula a utilizar es:
    $$
    Corriente_{requerida}\left(A\right)=\frac{Demanda_{final}\left(Ah/dia\right)}{ESH\left(h/dia\right)}
    $$

### Etapa 7: Dimensionamiento de Módulos (Paneles)

A partir de la interfaz de usuario en el sistema de cálculos del entorno virtual, el estudiante debe elegir las especificaciones del módulo fotovoltaico.

*   Se necesitan dos datos técnicos del panel seleccionado: la tensión en el punto de máxima potencia ( $V_{mp}$ ) y la corriente en el punto de máxima potencia ( $I_{mp}$ ).
*   Cálculo de módulos en paralelo ( $N_{p}$ ):
    $$
    N_{p}=\frac{Corriente_{requerida}\left(A\right)}{I_{mp}}
    $$
*   Cálculo de módulos en serie ( $N_{s}$ ):
    $$
    N_{s}=\frac{Voltaje_{nominal}\left(V\right)}{V_{mp}}
    $$
*   **Número total de módulos:** Se calcula multiplicando los módulos en paralelo por los módulos en serie. El valor teórico mínimo siempre será de 1 módulo.
    +1
    $$
    Total_{Moˊdulos}=N_{p}\times N_{s}
    $$

### Etapa 8: Dimensionamiento del Banco de Baterías

*   Se debe decidir la cantidad de días de reserva o autonomía (por ejemplo, 5 días).
*   **Capacidad requerida:**
    $$
    Capacidad_{requerida}\left(Ah\right)=Demanda_{final}\left(Ah/dia\right)\times Dıˊas_{reserva}
    $$
*   **Ajuste por profundidad de descarga segura (DoD):** Para prolongar la vida útil, se asume un uso máximo del 80% de la capacidad de la batería.
    $$
    Capacidad_{nominal}\left(Ah\right)=\frac{Capacidad_{requerida}\left(Ah\right)}{0.8}
    $$
*   **Baterías en serie:** Depende del voltaje nominal del sistema y el voltaje de la batería comercial elegida (ejemplo: 12 V).
    $$
    N_{serie}=\frac{Voltaje_{nominal}\left(V\right)}{Voltaje_{baterıˊa}\left(V\right)}
    $$
*   Baterías en paralelo:
    $$
    N_{paralelo}=\frac{Capacidad_{nominal}\left(Ah\right)}{Capacidad_{baterıˊa}}
    $$

* * *

6\. Metodología de Evaluación y Diseño Experimental
---------------------------------------------------

Para los docentes a cargo de validar esta práctica, se empleará un diseño cuasi-experimental:

1.  **Grupos de Estudio:** Se debe comparar el aprendizaje del grupo experimental (estudiantes que usan la RV) con un grupo de control (instrucción tradicional). En lo posible, asignar a los estudiantes aleatoriamente para minimizar sesgos.
    +3
2.  **Evaluación:** Se aplicará un pre-test y un post-test para medir el conocimiento de los estudiantes antes y después de la intervención.
    +1
3.  **Ejecución:** El estudiante dispondrá de 30 minutos en el entorno virtual para seguir las etapas del flujo de cálculos. El docente no debe intervenir ni explicar fórmulas durante la simulación, permitiendo el aprendizaje activo y el registro de errores.
    +2

* * *

Espero que esta estructura brinde la claridad y la precisión académica que buscas para tus estudiantes de ingeniería. ¡Éxito con las pruebas piloto!

## Prompt:
Ok. Empecemos a detallar cada sección. Introducción primero.

Que debería tener una excelente introducción para esta guia?

## Response:
Para que una introducción en una guía de laboratorio de ingeniería sea excelente, especialmente para estudiantes de cuarto semestre, debe cumplir tres funciones críticas: **contextualizar** la importancia del tema, **justificar** el uso de la tecnología elegida y **conectar** la teoría con la aplicación profesional.

Aquí tienes el contenido detallado para la sección de **Introducción** de tu guía, redactado con un enfoque académico y pedagógico:

### 1\. Introducción

La transición energética global hacia fuentes de energía asequible y limpia es una prioridad consignada en los Objetivos de Desarrollo Sostenible (ODS 7). En Colombia, este proceso ha cobrado gran relevancia, particularmente en regiones con altos niveles de radiación solar como el departamento del Cauca. A pesar de que el Cauca cuenta con uno de los promedios de radiación solar más altos del país (aprox.  $4.25 kWh/m^{2}$ ), la implementación de tecnologías fotovoltaicas sigue siendo reducida, lo que representa un reto y una oportunidad para los futuros ingenieros.

+3

Sin embargo, la formación práctica en el diseño de estos sistemas suele enfrentarse a barreras económicas debido a los altos costos de los equipos y la infraestructura necesaria para la experimentación directa. Esta limitación a menudo genera una brecha entre el aprendizaje teórico y las competencias técnicas requeridas en el campo profesional.

+2

Como respuesta a este desafío, esta guía incorpora el uso de la **Realidad Virtual (RV)** y los **Serious Games** como herramientas pedagógicas innovadoras. La RV permite sumergirse en un entorno simulado donde es posible interactuar con componentes fotovoltaicos, realizar cálculos complejos y tomar decisiones de diseño sin los riesgos físicos o las limitaciones de espacio de un laboratorio convencional.

+4

A través de esta práctica inmersiva, el estudiante no solo reforzará los fundamentos de la electricidad, sino que aprenderá a ver el diseño fotovoltaico como un sistema integral. El objetivo es que logres relacionar la teoría energética con decisiones prácticas, mejorando la retención de conocimientos mediante el aprendizaje experiencial y preparándote para liderar proyectos de energía renovable en la región.

+4

* * *

**¿Qué hace que esta introducción sea efectiva para tus estudiantes?**

*   **Motivación Regional:** Al mencionar la radiación solar en el Cauca, el estudiante siente que lo que aprende tiene aplicación inmediata en su entorno.
    +1
*   **Justificación Tecnológica:** Explica por qué están usando gafas de RV en lugar de paneles reales, validando la tecnología como una solución ante los altos costos de los laboratorios físicos.
*   **Claridad de Propósito:** Define claramente que el problema a resolver es la brecha entre "saber la fórmula" y "saber diseñar un sistema".

¿Deseas que continuemos con la sección de **Objetivos** o prefieres ajustar algo de este texto?

## Prompt:
Esta introducción sustenta la aplicacion y el proyecto, pero no se orienta al estudiante que utiliza la herramienta para aprender sobre el diseño de sistemas fotovoltaicos

## Response:
Tienes razón. Una excelente guía de laboratorio debe hablarle directamente al estudiante, planteando el **desafío técnico** que va a resolver y el **valor práctico** de lo que está a punto de hacer.

Aquí tienes una propuesta de introducción enfocada 100% en el aprendizaje del estudiante y en el proceso de ingeniería de diseño:

### 1\. Introducción

Bienvenido a esta práctica de laboratorio. Como futuro ingeniero, te encuentras en un momento crucial de la transición energética global, donde el diseño de sistemas de energía limpia es una de las competencias más demandadas en el sector industrial. El diseño de un sistema fotovoltaico no consiste solo en aplicar fórmulas aisladas; es un proceso de ingeniería integral que requiere entender cómo interactúan el consumo de energía, las pérdidas del sistema y las especificaciones técnicas de los equipos.

+3

En este laboratorio, dejarás de lado los ejercicios de lápiz y papel para convertirte en el diseñador de una solución real. Utilizarás un entorno de **Realidad Virtual (RV)** que te permite "entrar" en el sistema. El objetivo no es solo que navegues por un entorno digital, sino que utilices esta herramienta para realizar un **dimensionamiento técnico preciso**. A través de ocho etapas lógicas, realizarás una auditoría energética, calcularás la demanda real considerando pérdidas críticas y seleccionarás la configuración óptima de paneles y baterías para garantizar la autonomía del sistema.

+4

Esta experiencia está diseñada para que cierres la brecha entre la teoría eléctrica de tus libros y la implementación práctica en campo. Al finalizar, no solo habrás aprendido a calcular componentes; habrás desarrollado el criterio técnico necesario para tomar decisiones de diseño basadas en la eficiencia y la sostenibilidad, habilidades fundamentales para tu futuro profesional en la ingeniería.

+2

* * *

### ¿Por qué esta versión es mejor para el estudiante?

*   **Define un Rol:** El estudiante ya no es un "sujeto de prueba", es un "diseñador de una solución real".
*   **Presenta la Hoja de Ruta:** Menciona explícitamente que pasará por un proceso de 8 etapas, dándole una estructura mental de lo que va a hacer.
    +1
*   **Enfoque en Competencias:** Resalta que aprenderá a tener "criterio técnico" y a "tomar decisiones", que es lo que realmente hace un ingeniero.
    +1
*   **Imagen Sugerida:** Podrías insertar aquí: para que visualicen el camino que van a recorrer.

¿Te parece que este tono es más adecuado para tus alumnos de cuarto semestre? Si es así, podemos proceder a detallar la sección de **Objetivos de Aprendizaje**.

## Prompt:
> FO-CU-005 ...t29Julio25 - CSV

La practica se orienta a estudiantes de ingenieria industrial que ven la asignatura de Instrumentación Industrial. Este es el contenido tematico de la asignatura.

## Response:
```
import pandas as pd

# Let's inspect the uploaded CSV file
file_path = 'FO-CU-005 INSTRUMENTACION INDUSTRIAL - Act29Julio25.csv'
df = pd.read_csv(file_path, sep=';', skiprows=7) # The metadata says estimatedRowsAboveHeader: 7
print(df.head())
print("---")
print(df.info())

```

Salida de código

```
                                                     Nombre del Tema 1:                                                            Unnamed: 1                                                                          objetivo especifico por \nUnidad 1 dia   mes año  Estrategía Pedagógica (Presencial)\nRevisar las del punto 3 Estrategía Pedagógica (Independiente)\nRevisar las del punto 3 Hr trabajo Presencial Hr Trabajo Independiente Unnamed: 10
0               Historia corta del control e instrumentación industrial               Historia corta del control e instrumentación industrial  Identificar  los elementos de automatización e instrumentación involucrados en los procesos de producción.  NaN  NaN  NaN                                                         1.1                                                            1.3                     3                        6         NaN
1                                                     Conceptos básicos                                                     Conceptos básicos                                                                                                         NaN  NaN  NaN  NaN                                                         NaN                                                            NaN                   NaN                      NaN         NaN
2  Características de los sistemas de control de lazo abierto y cerrado  Características de los sistemas de control de lazo abierto y cerrado                                                                                                         NaN  NaN  NaN  NaN                                                         NaN                                                            NaN                   NaN                      NaN         NaN
3                                                   Esquemas de control                                                   Esquemas de control                                                                                                         NaN  NaN  NaN  NaN                                                         NaN                                                            NaN                   NaN                      NaN         NaN
4                                  Sistema de lazo cerrado generalizado                                  Sistema de lazo cerrado generalizado                                                                                                         NaN  NaN  NaN  NaN                                                         NaN                                                            NaN                   NaN                      NaN         NaN
---
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 95 entries, 0 to 94
Data columns (total 11 columns):
 #   Column                                                         Non-Null Count  Dtype 
---  ------                                                         --------------  ----- 
 0   Nombre del Tema 1:                                             48 non-null     object
 1   Unnamed: 1                                                     33 non-null     object
 2   objetivo especifico por 
Unidad 1                              10 non-null     object
 3   dia                                                            5 non-null      object
 4   mes                                                            5 non-null      object
 5   año                                                            5 non-null      object
 6   Estrategía Pedagógica (Presencial)
Revisar las del punto 3     21 non-null     object
 7   Estrategía Pedagógica (Independiente)
Revisar las del punto 3  21 non-null     object
 8   Hr trabajo Presencial                                          21 non-null     object
 9   Hr Trabajo Independiente                                       21 non-null     object
 10  Unnamed: 10                                                    1 non-null      object
dtypes: object(11)
memory usage: 8.3+ KB
None

```

```
topics = df['Nombre del Tema 1:'].dropna().tolist()
for i, topic in enumerate(topics):
    print(f"{i}: {topic}")

```

Salida de código

```
0: Historia corta del control e instrumentación industrial
1: Conceptos básicos
2: Características de los sistemas de control de lazo abierto y cerrado
3: Esquemas de control
4: Sistema de lazo cerrado generalizado
5: Instrumentos típicos en un lazo de control 
6: Definiciones básicas en instrumentación y control
7: Sistemas de transmisión de señal
8: Transmisores de señal
9: Redes de comunicación industrial
10: Controladores lógicos programables y sistemas de control distribuidos
11: Descripción conceptual en el diseño de automatización de un proceso industrial
12: Nombre del Tema 2:
13: Campos electricos
14: Potencial electrico
15: Corriente y Resistencia
16: Circucitos de corriente continua
17: Campos magneticos
18: Ley de Faraday
19: Circuitos de corriente alterna
20: Parcial I
21: Nombre del Tema 3:
22: Diagrama PFD
23: Diagrama P&ID
24: Diagrama de lazo de instrumentos
25: Diagramas de mando, potencia y escalera
26: Nombre del Tema 4:
27: Introducción
28: Propiedades de los instrumentos de medición.
29: Medición de temperatura
30: Medición de presión
31: Medición de caudal
32: Medición de nivel
33: Medición de otras variables 
34: Transmisión de señales eléctricas
35: Parcial II
36: Nombre del Tema 5:
37: Introducción
38: Válvulas de control
39: Convertidor I/P
40: Accesorios de las válvulas de control
41: Motor eléctrico
42: Relés y contactores
43: Accesorios de los motores eléctricos
44: Cilindros neumáticos e hidráulicos
45: Otros tipos de actuadores
46: Parcial III
47: Nombre del Tema 6:

```

¡Excelente detalle! Saber que esta práctica se inserta en la asignatura de **Instrumentación Industrial** y conocer su contenido temático (particularmente la **Unidad 2 sobre electricidad y circuitos DC/AC**, y la **Unidad 3 sobre diagramas de procesos y lazos**) es clave para darle pertinencia académica a la guía.

Vamos a detallar la siguiente sección de la guía, enfocándonos en los **Objetivos de Aprendizaje y Competencias**. Redactaré esta parte conectando directamente los fundamentos teóricos de la asignatura con la experiencia en Realidad Virtual.

Aquí tienes la propuesta para la continuación de la guía:

* * *

### 2\. Objetivos de Aprendizaje

Esta práctica ha sido diseñada para articular los conceptos teóricos de la asignatura de **Instrumentación Industrial** con la toma de decisiones en un entorno de ingeniería aplicada. Al finalizar la simulación inmersiva, se espera que logres:

**Objetivo General:** Diseñar un sistema fotovoltaico autónomo básico en un entorno de Realidad Virtual, aplicando los fundamentos de circuitos eléctricos (DC/AC), medición y análisis de variables energéticas para satisfacer los requerimientos de carga de un proceso industrial o residencial.

**Objetivos Específicos:**

*   **Identificar e interpretar variables eléctricas:** Analizar la potencia nominal (W) y el tiempo de operación (h) de diferentes cargas para estructurar un perfil de consumo energético diario.
*   **Aplicar principios de circuitos de corriente continua (DC) y alterna (AC):** Calcular la conversión de cargas AC a DC considerando la eficiencia de los equipos (inversores), aplicando los principios de conservación de energía.
*   **Diseñar arreglos serie-paralelo:** Dimensionar la matriz de paneles solares fotovoltaicos y el banco de baterías, calculando correctamente las variaciones de tensión (Voltaje) y corriente (Amperaje) según el tipo de conexión (serie o paralelo).
*   **Analizar las pérdidas del sistema:** Reconocer la caída de tensión y pérdida de eficiencia (10%) en los lazos de transmisión y regulación de energía, ajustando la demanda final del sistema.

### 3\. Relación con el Contenido de la Asignatura

El diseño de un sistema fotovoltaico es, en esencia, la estructuración de un sistema de generación y transmisión de energía local. Las decisiones que tomarás en el entorno virtual pondrán a prueba los conocimientos adquiridos en clase, específicamente en:

*   **Fundamentos de Electricidad (Conexión con Unidad 2):** Aplicarás la Ley de Ohm y la Ley de Watt de forma práctica. Entenderás la diferencia física entre circuitos de corriente continua (DC, propios de paneles y baterías) y corriente alterna (AC, propios del consumo final), y cómo se relacionan matemáticamente en un circuito real.
*   **Lectura de Variables e Instrumentación (Conexión con Unidad 1 y 4):** Aunque el sistema lo hace automáticamente en el juego, comprenderás que todo panel tiene valores nominales medibles ( $V_{mp}$  y  $I_{mp}$ ) que dictan el comportamiento del sistema bajo un esquema de lazo abierto de generación.
*   **Diagramación Lógica (Conexión con Unidad 3):** Para realizar los cálculos adecuadamente, deberás concebir mentalmente el diagrama de flujo del proceso: desde la radiación solar captada, pasando por la regulación, el almacenamiento (baterías) y la inversión (inversor DC/AC), hasta llegar a la carga final.

* * *

**¿Por qué este enfoque es ideal para tus alumnos?**

*   **Conecta los "puntos":** Los estudiantes suelen ver "Circuitos DC/AC" (Unidad 2) como pura matemática. Al conectarlo explícitamente en la guía, entenderán que sumar voltajes en serie es exactamente lo que necesitan hacer para alcanzar los 24V o 48V de un banco de baterías.
*   **Eleva el rigor académico:** Cumple con la exigencia de los evaluadores del proyecto de tener claridad metodológica y pedagógica, justificando por qué este _serious game_ no es solo un juego, sino un laboratorio de instrumentación y electricidad.

¿Te gusta esta estructuración de objetivos? Si estás de acuerdo, el siguiente paso ideal sería desarrollar la sección del **Marco Teórico**, donde explicamos la teoría de los paneles de forma muy concisa, adaptada para estudiantes que apenas están viendo las bases de corriente y resistencia eléctrica.

## Prompt:
Volvamos a redactar la introducción considerando este nuevo contexto.

## Response:
Entendido. Como investigador y docente, comprendo que el tono y el enfoque deben ajustarse exactamente al momento académico del estudiante: acaban de cursar los conceptos básicos de electricidad (corriente, voltaje, circuitos DC/AC) y ahora deben ver su aplicación directa en la industria sin sentirse abrumados por conceptos que aún no dominan.

Aquí tienes la versión reescrita de la introducción, integrando la realidad de la asignatura de Instrumentación Industrial, el nivel de cuarto semestre y los datos de tu proyecto:

* * *

### 1\. Introducción

La transición hacia fuentes de energía sostenibles exige que los futuros ingenieros industriales estén plenamente capacitados para diseñar, evaluar e instrumentar sistemas de generación limpia. En regiones con un alto potencial energético como el departamento del Cauca, el cual registra niveles de radiación solar de hasta **4.25 kWh/m²** diarios , el aprovechamiento de la energía solar fotovoltaica se perfila como una solución tecnológica fundamental.

+3

En la asignatura de Instrumentación Industrial, ustedes han estudiado los principios fundamentales de la electricidad, abarcando el comportamiento de la corriente, el potencial eléctrico, la resistencia y la diferencia operativa entre los circuitos de corriente continua (DC) y alterna (AC). Esta práctica de laboratorio representa el puente exacto entre esos fundamentos matemáticos y la aplicación industrial real. El diseño de un sistema fotovoltaico requerirá que analicen cómo la energía fluye desde una fuente en corriente continua (los paneles y baterías), se transforma (mediante inversores) y finalmente alimenta cargas comerciales que operan en corriente alterna.

+2

Comúnmente, la formación práctica en el montaje y dimensionamiento de estos sistemas es limitada por los altos costos de adquisición de equipos reales y la infraestructura de experimentación. Para superar este obstáculo, utilizaremos un entorno de Realidad Virtual (RV) inmersiva estructurado como un _serious game_. Esta tecnología educativa les permitirá interactuar de manera segura con componentes industriales virtuales, visualizando el impacto directo de sus cálculos en el rendimiento de un sistema fotovoltaico sin los riesgos de la experimentación física.

+4

A lo largo de esta guía, asumirán el rol de diseñadores. Su objetivo no será simplemente navegar en un entorno virtual, sino aplicar sus conocimientos de circuitos para identificar cargas energéticas, calcular el consumo equivalente, estimar las pérdidas de eficiencia y, finalmente, dimensionar de manera funcional tanto el arreglo fotovoltaico como el banco de almacenamiento. Al concluir la sesión experiencial, comprenderán el diseño solar no como una teoría aislada, sino como un sistema integral de ingeniería que responde a necesidades técnicas reales.

+1

* * *

**¿Por qué esta versión es la indicada para tu contexto?**

*   **Reconoce su nivel:** Valida explícitamente que son estudiantes de 4to semestre que conocen de voltaje, corriente y DC/AC, dándoles confianza para abordar la práctica.
*   **Justifica la asignatura:** Conecta directamente los temas de la Unidad 2 (Campos eléctricos, circuitos DC/AC) con el funcionamiento del panel (generador DC) y el inversor (convertidor a AC).
*   **Formalidad investigativa:** Mantiene el rigor de una guía universitaria, justificando el uso de la RV por las barreras económicas y de seguridad de los laboratorios físicos.

Si esta introducción refleja exactamente lo que necesitas proyectar, podemos avanzar a detallar la sección del **Marco Teórico (Conceptos Básicos de Fotovoltaica para Estudiantes de Instrumentación)**. ¿Te parece bien?

## Prompt:
Excelente, continuemos con los objetivos de la practica.

## Response:
Como investigador y docente, considero que los objetivos de una guía de laboratorio no deben ser una simple lista de tareas, sino declaraciones claras de lo que el estudiante logrará comprender y aplicar, redactados bajo la filosofía SMART (Específicos, Medibles, Alcanzables, Relevantes y con Tiempo definido) sugerida en los estándares de evaluación académica.

Dado que tus estudiantes de cuarto semestre ya manejan los conceptos de la **Unidad 2 (circuitos DC/AC, voltaje, corriente y potencia)**, los objetivos deben retarlos a usar esas herramientas matemáticas en un caso aplicado.

Aquí tienes la propuesta detallada para la sección de Objetivos y Competencias:

* * *

### 2\. Objetivos de la Práctica

Esta sesión de laboratorio inmersivo tiene como propósito fundamental evaluar y consolidar la efectividad del aprendizaje práctico mediante el uso de entornos simulados. Durante los 30 minutos de ejecución en el entorno virtual, el estudiante deberá cumplir con los siguientes objetivos:

+1

#### 2.1. Objetivo General

Diseñar y dimensionar integralmente un sistema fotovoltaico autónomo utilizando un entorno de simulación en Realidad Virtual (RV), aplicando los principios fundamentales de circuitos eléctricos de corriente continua (DC) y alterna (AC) para satisfacer una demanda energética específica.

#### 2.2. Objetivos Específicos

Para alcanzar el objetivo general, el estudiante logrará secuencialmente:

1.  **Cuantificar la demanda energética:** Identificar las cargas energéticas del sistema e interpretar el consumo eléctrico diario, aplicando la relación fundamental entre potencia nominal y tiempo de operación ( $Energıˊa=Potencia\times Tiempo$ ).
    +2
2.  **Analizar la eficiencia de conversión eléctrica:** Comprender el impacto de las pérdidas del sistema y realizar la conversión matemática de las cargas de corriente alterna (AC) a su equivalente en corriente continua (DC), asumiendo una eficiencia del inversor del 90%.
    +1
3.  **Diseñar el arreglo de generación (Paneles):** Dimensionar un arreglo fotovoltaico funcional, determinando la cantidad exacta de módulos solares requeridos y su configuración de conexión (en serie para sumar voltaje, o en paralelo para sumar corriente) con base en las Horas de Sol Equivalente (ESH) y la demanda final.
    +2
4.  **Dimensionar el sistema de almacenamiento (Baterías):** Calcular correctamente la capacidad del banco de baterías requerida para garantizar los días de reserva (autonomía) del sistema, aplicando factores de corrección técnicos como la profundidad de descarga segura (DoD).
    +3

#### 2.3. Competencias a Desarrollar (Relación con Instrumentación Industrial)

Esta práctica aterriza los conceptos vistos en las clases teóricas en habilidades de ingeniería aplicada:

*   **Aplicación de Circuitos Eléctricos (Unidad 2):** El estudiante dejará de ver la corriente y el voltaje como conceptos abstractos. Entenderá que al conectar paneles solares en **serie** ( $N_{serie}=\frac{Voltaje_{nominal_sistema}}{V_{mp}}$ ) se aumenta el potencial eléctrico (V) para igualar el requerimiento del inversor o banco de baterías , mientras que conectarlos en **paralelo** aumenta la capacidad de corriente (A).
    +4
*   **Análisis de Lazo Abierto de Generación (Unidad 1 y 3):** Comprenderá que un sistema fotovoltaico es un proceso que sigue un diagrama de flujo de energía unidireccional: Captación (Paneles)  $\to$  Regulación  $\to$  Almacenamiento (Baterías)  $\to$  Inversión (DC a AC)  $\to$  Consumo final.
*   **Toma de Decisiones bajo Restricciones:** El estudiante aprenderá que en la ingeniería real los sistemas no son 100% ideales; deberá sobredimensionar matemáticamente el sistema para compensar un 10% de pérdidas de transmisión y regulación.

* * *

**Notas pedagógicas sobre esta redacción:**

*   **Claridad en la meta:** Los verbos "Cuantificar", "Analizar" y "Diseñar" marcan acciones cognitivas claras que tú, como evaluador, podrás medir a través del registro de decisiones correctas y el tiempo de resolución en la herramienta de RV.
*   **Articulación directa:** Explicamos brevemente _por qué_ es importante saber conectar en serie o paralelo, lo que refresca su memoria de lo visto en la asignatura de Instrumentación.

Si apruebas esta sección, el siguiente paso natural es redactar el **Marco Teórico**. En esta parte, les daremos un "repaso exprés" de cómo funciona un panel y cómo se estructuran las fórmulas que verán en la simulación, manteniendo el nivel adecuado para cuarto semestre. ¿Procedemos con el Marco Teórico?

## Prompt:
Para la redacción de los objetivos y del resto de la guia (marco teorico, procedimiento, calculos), considero pertiente tener presente cuales son los pasos para el diseño descritos en el archivo draft\_app\_guide.docx, asi como las interacciones y pasos que realiza dentro del entorno de RV.

El serious game se desarrolló en Unity, este cuenta con un entorno de una casa en la que se disponen multiples objetos electrónicos y eléctricos que el estudiante debe buscar, cargar y depositar en un punto (vehiculo de mudanza). Esto determina la cantidad de carga que se requiere para el diseño del sistema. Primer paso en el diseño.

Este escenario simulaba en la historia una mudanza, en aras de determinar la potencia/consumo total para el diseño de un sistema de paneles fotovoltaicos off-grid.

## Response:
Es fundamental integrar la narrativa de la "mudanza" con el rigor técnico del dimensionamiento. Esta analogía permite que el estudiante de Instrumentación Industrial vea el levantamiento de cargas no como una lista aburrida, sino como una **auditoría energética activa**.

A continuación, presento las secciones de **Marco Teórico**, **Procedimiento** y **Cálculos** detalladas para la guía, vinculando la experiencia en Unity con el flujo de diseño técnico.

* * *

### 3\. Marco Teórico

Para diseñar un sistema fotovoltaico autónomo (_Off-grid_), es necesario comprender cómo interactúan los componentes que permiten captar, regular, almacenar y transformar la energía.

*   **Sistemas Fotovoltaicos Autónomos:** Son instalaciones diseñadas para operar de forma independiente a la red eléctrica convencional. Se componen de paneles, reguladores de carga, bancos de baterías e inversores.
    +1
*   **Auditoría de Cargas (Demanda Energética):** Es el primer paso de cualquier diseño de ingeniería. Consiste en identificar cada receptor eléctrico, su potencia nominal (en Watts) y su tiempo de uso estimado. En un sistema autónomo, las cargas pueden ser de Corriente Directa (DC) o Corriente Alterna (AC).
    +1
*   **Configuración de Arreglos (Serie vs. Paralelo):** \* **Conexión en Serie:** Aumenta el voltaje total del sistema manteniendo la corriente igual a la de un solo módulo. Se usa para alcanzar la tensión nominal de operación del inversor.
    +1
    *   **Conexión en Paralelo:** Aumenta la corriente total del sistema manteniendo el voltaje igual al de un solo módulo. Se usa para satisfacer la demanda de corriente requerida por el consumo.
        +1
*   **Almacenamiento y Autonomía:** Debido a que el sol es una fuente intermitente, se requieren baterías para suministrar energía durante la noche o días nublados. La **autonomía** define cuántos días puede el sistema alimentar las cargas sin recibir radiación solar.
    +1
*   **Eficiencia de Conversión (Inversor):** El inversor transforma la energía de las baterías (DC) en energía utilizable por electrodomésticos estándar (AC). Este proceso no es perfecto y conlleva una pérdida de energía, usualmente estimada en un 10% (eficiencia del 0.9).
    +2

* * *

### 4\. Procedimiento de la Práctica en RV

El laboratorio se desarrolla en un entorno inmersivo de Realidad Virtual que simula una mudanza. Tu misión es determinar qué equipos se llevarán a la nueva locación y diseñar el sistema solar que los alimentará.

1.  **Fase de Introducción y Diagnóstico:** Antes de iniciar, deberás completar una encuesta inicial sobre tus conocimientos previos en electricidad y experiencia en entornos de RV.
    +1
2.  **Fase de Auditoría de Cargas (La Mudanza):** \* Explora la vivienda virtual e identifica los objetos electrónicos y eléctricos disponibles.
    *   Deberás cargar cada objeto seleccionado y depositarlo en el vehículo de mudanza.
    *   **Nota Técnica:** Al depositar el objeto, el sistema registrará su potencia y uso diario. Este paso es crítico, ya que determina la "Energía Total" que tu sistema deberá generar.
3.  **Fase de Centro de Cálculos:** Una vez finalizada la mudanza, te desplazarás a la interfaz de diseño donde aplicarás el flujo matemático de 8 etapas para dimensionar el sistema. Tienes un tiempo máximo de 30 minutos para completar el diseño.
    +2

* * *

### 5\. Guía de Cálculos y Dimensionamiento

Sigue este flujo lógico dentro de la interfaz del _serious game_ para asegurar un diseño funcional:

*   **Etapa 1. Energía por Carga:** Calcula el consumo individual de cada objeto que pusiste en el vehículo.
    $$
    Energıˊa=Potencia\left(W\right)\times Tiempo\left(h\right)
    $$
*   **Etapa 2. Equivalencia AC a DC:** Si el objeto usa corriente alterna, ajusta el valor por la eficiencia del inversor (90%).
    $$
    Energıˊa_{equiv_DC}=\frac{Energıˊa_{AC}}{0.9}
    $$
*   **Etapa 3. Demanda Total Diaria:** Suma todos los valores obtenidos para conocer el requerimiento total de la vivienda en Wh/día.
*   **Etapa 4. Selección de Tensión:** Elige la tensión nominal del sistema (12V, 24V o 48V). Calcula el requerimiento en Amperios-hora (Ah/día):
    $$
    Ah/dıˊa=\frac{Energıˊa_{Total}}{Tensioˊn_{nominal}}
    $$
*   **Etapa 5. Demanda Final con Pérdidas:** Considera un 10% de pérdidas por cableado y regulación (eficiencia del sistema 0.9).
    $$
    Demanda_{final}=\frac{Requerimiento\left(Ah/dıˊa\right)}{0.9}
    $$
*   **Etapa 6. Corriente del Arreglo:** Utiliza las Horas Sol Equivalente (ESH) para determinar la corriente necesaria que deben entregar los paneles.
    +1
*   **Etapa 7. Número de Módulos:** Selecciona un panel de la base de datos (observa su  $V_{mp}$  e  $I_{mp}$ ) y calcula:
    *   **Módulos en Paralelo ( $N_{p}$ ):**  $\frac{Corriente_{requerida}}{I_{mp}}$ 
    *   **Módulos en Serie ( $N_{s}$ ):**  $\frac{Voltaje_{nominal_sistema}}{V_{mp}}$ 
    *   **Total:**  $N_{p}\times N_{s}$ 
*   **Etapa 8. Banco de Baterías:** Define los días de reserva (ej. 5 días). Calcula la capacidad nominal ajustando por una profundidad de descarga (DoD) del 80% para proteger la vida útil de la batería.
    +2

* * *

**¿Qué sigue?** Podemos redactar ahora la sección de **Métricas de Evaluación y Resultados Esperados**, donde le explicamos al estudiante qué indicadores (tiempo, precisión, puntaje) determinarán su éxito en la práctica. ¿Te parece bien continuar con eso?

## Prompt:
Antes de la redacción de estas secciones, requiero que revises si los pasos son los correctos, antes de continuar. Ademas, requiero que seas critico con el proyecto, la guia, los pasos que se realizan, el publico objetivo, etc.

## Response:
Como investigador y colega en el área de ingeniería, valoro profundamente esta pausa. Es exactamente lo que exige el rigor académico: cuestionar la herramienta y el método antes de dar por sentado que funcionarán perfectamente en la práctica.

Revisando detalladamente los documentos del proyecto, el sílabo de la asignatura y la mecánica del _serious game_, he identificado varios puntos críticos que debemos analizar para asegurar que el proyecto no solo sea un "juego llamativo", sino una herramienta pedagógica robusta para estudiantes de cuarto semestre.

Aquí tienes mi evaluación crítica dividida en cuatro dimensiones:

### 1\. Crítica a los Cálculos Matemáticos (Etapa 7)

El flujo matemático planteado en la guía base (draft\_app\_guide.docx) es, en su mayoría, coherente para un diseño básico _off-grid_. Sin embargo, hay un problema conceptual grave en el cálculo de los módulos en serie (Etapa 7).

*   **El error:** La fórmula estipula  $N_{serie}=\frac{Voltaje_{nominal_sistema}}{V_{mp}}$ . Si el sistema es de 24 V y el panel tiene un  $V_{mp}$  de 30 V, el resultado es 0.8 paneles, lo que obligaría al estudiante a redondear a 1.
*   **La realidad técnica:** Para cargar un banco de baterías, el voltaje del panel ( $V_{mp}$ ) **siempre** debe ser superior al voltaje de la batería para vencer su resistencia interna (por ejemplo, para cargar 24 V necesitas tensiones cercanas a 28.8 V o más, dependiendo del controlador). Dividir el voltaje nominal entre el  $V_{mp}$  causará confusión en los estudiantes, ya que matemáticamente podrían obtener fracciones ilógicas.
*   **La solución:** A este nivel, sería mejor replantear la fórmula indicando que se debe dividir el voltaje nominal del sistema entre el _voltaje nominal del panel_ (ej. panel de 12 V o 24 V), o establecer una regla clara sobre cómo manejar el  $V_{mp}$  respecto al controlador de carga (PWM vs. MPPT).

### 2\. Crítica a la Narrativa vs. Perfil del Estudiante

*   **La desconexión:** El escenario del juego es una casa y una "mudanza" residencial. Sin embargo, el público objetivo son estudiantes de **Ingeniería Industrial** viendo **Instrumentación Industrial**. Según el sílabo que compartiste, ellos están estudiando motores eléctricos, válvulas de control, cilindros neumáticos y PLCs.
*   **El impacto:** Un estudiante de ingeniería industrial podría percibir el cálculo de consumo de "televisores y licuadoras" como algo más propio de un técnico electricista residencial que de su perfil profesional.
*   **La solución didáctica:** Aunque no cambies el entorno de Unity (dado que ya está programado), en la guía escrita debes hacer un puente cognitivo. Puedes indicar: _"Aunque en esta simulación realizaremos la auditoría energética de equipos residenciales, este mismo principio de levantamiento de cargas se aplica para dimensionar el suministro de tableros de control aislados, estaciones de bombeo remotas o instrumentación de campo"_. Esto "salva" la pertinencia de la práctica.

### 3\. Crítica a la Carga Cognitiva y Ergonomía en RV

*   **El reto de calcular en RV:** La guía indica que el estudiante pasará por una fase de "ejecución del videojuego siguiendo el flujo de cálculos (30 minutos)". Hacer matemáticas complejas (divisiones, conversiones, eficiencia del 0.9) **dentro** de un entorno inmersivo puede ser exhaustivo. Las gafas de RV pueden generar fatiga visual o mareo, y tener que recordar números o usar calculadoras virtuales suele ser frustrante.
    +1
*   **La recomendación:** Es vital asegurar que el _serious game_ tenga una interfaz (UI) excelente para esta fase de cálculo. Idealmente, el juego debería registrar las variables automáticamente y el estudiante solo debería ingresar las operaciones lógicas, o permitirle quitarse las gafas un momento para usar papel, calculadora y la guía, y luego volver a ingresar los datos finales al simulador.
    +1

### 4\. Crítica al Diseño Experimental (Evaluación del Jurado)

*   **Las exigencias de los jurados:** El evaluador #1 fue muy enfático en que necesitas un diseño experimental sólido: _"Comparar el rendimiento... de un grupo experimental que utiliza el serious game en RV con un grupo de control que recibe instrucción tradicional"_.
    +1
*   **Integración en la guía:** La guía debe reflejar que los estudiantes que hagan esto en RV están siendo evaluados no solo por su nota de la asignatura, sino para validar tu proyecto de investigación. Tu encuesta pre-test y post-test debe estar calibrada para medir la misma competencia exacta en ambos grupos.
    +2

Como ves, la herramienta tiene muchísimo potencial, pero el éxito pedagógico dependerá de cómo justifiquemos estas pequeñas desconexiones en la guía de laboratorio.

Considerando el problema técnico de la fórmula del panel (Etapa 7) y el enfoque de la narrativa (residencial vs. industrial), ¿prefieres que ajustemos matemáticamente la etapa 7 en la guía o que nos enfoquemos en redactar las secciones faltantes adaptando la narrativa para "enganchar" al estudiante de ingeniería industrial?

## Prompt:
La parte del grupo de control, es complicada, pues no contamos con los equipos fisicos, Podrian hacerlo todo manualmente (lapiz y papel), tras una explicación magistral.

La parte de residencia se hizo porque es el primer escenario del proyecto, y resultaba para los estudiantes asociar facilmente las cargas (cosas cotidianas). Sin mebargo, si puedes sugerir comentarios respecto a esto, o justificaciones que me ayuden a sustentar esto frente a los evaluadores, mejor.

Los calculos, aunque integrados en la app RV, se pueden calcular sin usar el casco, y luego ingresarlos en la interfaz para su validación. Sería adecuado indicarlo en los pasos que el estudiante realiza.

## Response:
Me parece una excelente lectura de la situación. Como investigadores, constantemente debemos adaptar el diseño experimental a los recursos reales con los que contamos, y tus soluciones son pedagógicamente muy sólidas.

A continuación, te proporciono los argumentos académicos para defender tus decisiones ante los evaluadores (Jurados), seguidos de la redacción ajustada de los pasos de la guía de laboratorio incorporando el uso "híbrido" (RV + papel).

* * *

### 1\. Argumentos para defender el proyecto ante los evaluadores

#### Sobre el Grupo de Control (Lápiz y papel vs. RV)

La solución que propones es **exactamente** lo que se define en investigación educativa como un diseño cuasi-experimental válido. El evaluador 1 solicitó comparar un grupo experimental en RV con un grupo de control que reciba "instrucción tradicional".

*   **Tu argumento de defensa:** El diseño de sistemas fotovoltaicos actualmente se enseña de manera tradicional mediante clases magistrales y resolución de problemas en papel. Por lo tanto, el grupo de control con lápiz y papel representa fielmente la línea base actual de la educación en ingeniería. No contar con equipos físicos no es una debilidad del diseño de investigación; de hecho, justifica aún más la necesidad de validar la Realidad Virtual como alternativa frente a la carencia de laboratorios físicos costosos.

#### Sobre el Escenario Residencial para Estudiantes de Ingeniería Industrial

Utilizar cargas cotidianas (electrodomésticos) es una estrategia pedagógica altamente defendible bajo las teorías de diseño instruccional, lo cual responde a la inquietud del Jurado 1 sobre los "Fundamentos pedagógicos" incorporados en el diseño.

*   **Tu argumento de defensa (Teoría de la Carga Cognitiva):** Si a un estudiante que apenas domina los conceptos eléctricos se le presenta un escenario con cargas industriales complejas (ej. válvulas proporcionales o motores trifásicos), su cerebro gastará energía tratando de entender la máquina, en lugar de enfocarse en el objetivo de aprendizaje real: **el flujo del cálculo fotovoltaico**. Al usar una vivienda con objetos que ya conoce (un televisor, una nevera), reducimos la "carga cognitiva extrínseca".
*   **Andamiaje (Scaffolding):** El escenario residencial sirve como un puente cognitivo. Una vez que el estudiante domina el _proceso_ de dimensionamiento fotovoltaico (captación  $\to$  regulación  $\to$  almacenamiento) con cargas conocidas, transferir ese mismo procedimiento matemático para alimentar un tablero de control industrial será un paso trivial en su vida profesional.

* * *

### 2\. Redacción Ajustada para la Guía: Metodología y Procedimiento

Con esto en mente, aquí tienes la redacción de la sección de Procedimiento para tu guía de laboratorio, integrando la pausa para calcular en papel. Esta estructura reduce la fatiga visual de la RV y mejora el rigor analítico.

### Fases de Ejecución del Laboratorio

Esta práctica utilizará una metodología híbrida que combina la inmersión de la Realidad Virtual para la auditoría de campo, y el cálculo de ingeniería tradicional (lápiz y papel) para el análisis matemático.

**Fase 1: Auditoría Energética Inmersiva (Duración: 10 min)**

1.  Colóquese el visor de RV (Meta Quest) e ingrese al escenario de simulación ("La Mudanza").
2.  Identifique las cargas eléctricas disponibles en el entorno. Para cada equipo que deba ser energizado por el sistema solar, interactúe con él y deposítelo en el vehículo de recolección.
3.  El sistema registrará la potencia nominal ( $W$ ) y las horas de uso estimadas ( $h$ ) de los equipos seleccionados. Tome nota mental (o solicite a su compañero de laboratorio que registre) los datos proporcionados por la interfaz gráfica.

**Fase 2: Desconexión y Dimensionamiento Matemático (Duración: 15 min)**

1.  Retírese el visor de RV para evitar fatiga visual y ubicarse en su estación de trabajo física.
2.  Utilizando los datos de carga recolectados en la simulación, aplique el flujo de cálculos de ingeniería detallado en la **Sección 5** de esta guía (Etapas 1 a 8).
3.  Utilice su calculadora y registre en la hoja de resultados:
    *   Consumo total equivalente ( $Ah/dia$ ).
    *   Demanda final con pérdidas estimadas (eficiencia del  $0.9$ ).
    *   Número de paneles (Arreglo en Serie y Paralelo).
    *   Capacidad del banco de baterías (ajustado al 80% de profundidad de descarga).

**Fase 3: Validación Técnica en Entorno Virtual (Duración: 5 min)**

1.  Vuelva a colocarse el visor de RV e ingrese a la interfaz del "Centro de Cálculos" del _serious game_.
2.  Introduzca los valores paramétricos que calculó manualmente en papel.
3.  El sistema evaluará sus decisiones de diseño. Si los cálculos son correctos para garantizar la autonomía energética de las cargas seleccionadas, el simulador validará la instalación. Si hay errores (ej. baterías insuficientes para los días de autonomía), el sistema le exigirá iterar sobre su diseño.

* * *

**¿Por qué este ajuste es fundamental?** Al establecer esta pausa (Fase 2), resuelves el problema ergonómico de la RV, permites que los estudiantes trabajen en parejas (uno en RV, otro anotando, lo cual fomenta habilidades blandas), y garantizas que realmente hagan el proceso matemático en lugar de simplemente "adivinar" números dentro del juego para avanzar rápido.

Si estás de acuerdo con este enfoque metodológico, podemos proceder a estructurar la última parte de la guía: **El Formato de Recolección de Datos / Hoja de Resultados** que los estudiantes deberán llenar en esa "Fase 2" de lápiz y papel.

## Prompt:
Considerando lo dialogado, retomemos la redacción de cada sección. Volvamos a la introducción, es necesario cambiarla?

## Response:
Como investigador, te diré con franqueza: la introducción anterior era buena, pero con las decisiones pedagógicas y metodológicas que acabamos de tomar (el uso híbrido de papel/RV y la justificación de la carga cognitiva), **sí es necesario ajustarla**.

Una introducción académica de alto nivel no solo presenta el tema, sino que "setea las expectativas" del estudiante y defiende el diseño de la práctica. Si no les explicamos _por qué_ están en una casa haciendo una mudanza, los estudiantes de Ingeniería Industrial podrían subestimar el rigor del laboratorio.

Aquí tienes la introducción definitiva, estructurada para engranar todo el contexto, defender tus decisiones instruccionales y motivar al estudiante:

* * *

### 1\. Introducción

La transición hacia fuentes de energía sostenibles exige que los futuros ingenieros industriales estén plenamente capacitados para diseñar, evaluar e instrumentar sistemas de generación limpia. En regiones con un alto potencial energético como el departamento del Cauca, que registra un promedio diario de radiación solar de 4.25 kWh/m², el aprovechamiento de la energía solar fotovoltaica se perfila como una solución tecnológica y económica fundamental.

+1

En la asignatura de Instrumentación Industrial, ustedes han estudiado los principios teóricos de la electricidad, abarcando el comportamiento de la corriente, el potencial eléctrico, la resistencia y la diferencia operativa entre los circuitos de corriente continua (DC) y alterna (AC). Esta práctica de laboratorio representa el puente entre esos fundamentos matemáticos y la aplicación en la ingeniería real. El diseño de un sistema fotovoltaico requiere analizar cómo la energía fluye desde una fuente DC (paneles y baterías), se transforma y finalmente alimenta cargas finales en AC.

Comúnmente, la formación en el montaje de estos sistemas está limitada por los altos costos de los equipos y la infraestructura. Para superar esto, utilizaremos un entorno inmersivo en Realidad Virtual (RV) estructurado como un _serious game_.

+4

**Sobre el entorno de simulación:** El laboratorio los situará en un escenario residencial (una "mudanza"), donde deberán realizar una auditoría de cargas cotidianas. Si bien su perfil profesional se orientará a la industria, el uso de un entorno familiar es una estrategia pedagógica intencional orientada a reducir la "carga cognitiva". Al trabajar con consumos que ya conocen, podrán concentrar todo su esfuerzo analítico en dominar el algoritmo matemático del diseño fotovoltaico. Una vez asimilado este procedimiento estructurado, la transferencia de este conocimiento para dimensionar suministros eléctricos para instrumentación de campo, estaciones de bombeo o tableros de control aislados será un proceso natural.

A lo largo de esta sesión, emplearemos una **metodología híbrida**: utilizarán la RV para la exploración e identificación de variables , se desconectarán para aplicar el rigor del cálculo de ingeniería tradicional (lápiz y papel), y volverán al entorno virtual para someter su diseño a validación. Al concluir, comprenderán el diseño solar como un sistema integral, desarrollando el criterio técnico necesario para la toma de decisiones.

+4

* * *

**¿Por qué esta es la versión definitiva?**

1.  **Defensa proactiva:** Aborda el "elefante en la habitación" (el escenario de la casa) transformándolo en una fortaleza pedagógica. Esto le demuestra a los jurados que tienes pleno control sobre tu diseño instruccional.
2.  **Claridad del método:** Les advierte desde el inicio que no estarán 30 minutos con el casco puesto de forma ininterrumpida, sino que habrá trabajo matemático tradicional de por medio.
3.  **Alineación total:** Conecta el _Anteproyecto_ , los objetivos del _draft_ y el perfil de la materia de Instrumentación.
    +3

¿Qué te parece? Si estamos de acuerdo, podemos ensamblar la versión final de la **Sección 2 (Objetivos)** y la **Sección 3 (Marco Teórico y Fórmulas ajustadas)** con este mismo nivel de pulido investigativo.

## Prompt:
Consulta: Entiendo que los estudiantes son del curso de instrumentación industrial, pero eso no implica que este procedimiento se limite a ambientes industriales. Estos sistemas off-grid con el ejemplo de una zona residencial podria sustentarse en el contexto del Cauca, donde las empresas son pequeñas y hay poca industria. Ademas, estos sistemas off-grid son propicios para casas en fincas/campesinado/rural

## Response:
Tienes toda la razón y es una excelente lectura del entorno socioeconómico. Como investigador, te doy toda la razón metodológica: **la pertinencia regional es el mejor argumento posible para defender el diseño de tu proyecto ante los evaluadores.** De hecho, tu propio anteproyecto sustenta maravillosamente esta idea al mencionar que la adopción de estas tecnologías ayudará a mejorar la calidad de vida en "comunidades rurales no interconectadas" del Cauca y que estos sistemas autónomos tienen aplicaciones vitales en zonas rurales y agrícolas. Justificar el escenario residencial y de finca no como una "simplificación para el estudiante", sino como una **respuesta directa a las necesidades del territorio**, le da un peso investigativo y social enorme a tu trabajo de grado.

+1

Reescribamos ese fragmento de la introducción para que refleje este poderoso enfoque territorial y social, sin perder el rigor técnico.

* * *

### 1\. Introducción (Versión Ajustada con Pertinencia Regional)

La transición hacia fuentes de energía sostenibles exige que los futuros ingenieros industriales estén plenamente capacitados para diseñar, evaluar e instrumentar sistemas de generación limpia. En regiones con un alto potencial energético como el departamento del Cauca, que registra un promedio diario de radiación solar de 4.25 kWh/m², el aprovechamiento de la energía solar fotovoltaica se perfila como una solución tecnológica y económica fundamental.

En la asignatura de Instrumentación Industrial, ustedes han estudiado los principios teóricos de la electricidad, abarcando el comportamiento de la corriente, el potencial eléctrico, la resistencia y la diferencia operativa entre los circuitos de corriente continua (DC) y alterna (AC). Esta práctica de laboratorio representa el puente entre esos fundamentos matemáticos y su aplicación en la ingeniería real. El diseño de un sistema fotovoltaico autónomo (_off-grid_) requiere analizar cómo la energía fluye desde una fuente de generación DC, se almacena, se transforma y finalmente alimenta cargas convencionales.

Comúnmente, la formación en el montaje de estos sistemas está limitada por los altos costos de los equipos y la infraestructura. Para superar esto, utilizaremos un entorno inmersivo en Realidad Virtual (RV) estructurado como un _serious game_.

+1

**Sobre el entorno de simulación y su pertinencia:** El laboratorio los situará en un escenario residencial interactivo (una "mudanza"), simulando el levantamiento de cargas energéticas para una instalación aislada. Aunque su perfil es industrial, el diseño de sistemas _off-grid_ para viviendas, fincas y zonas rurales no interconectadas es una de las áreas de mayor impacto profesional en el Cauca. Nuestro tejido empresarial está compuesto en gran medida por pequeñas empresas y vocación agrícola, donde la automatización y el suministro energético a menudo deben resolverse de manera autónoma. Al dominar el dimensionamiento de cargas en este entorno cotidiano y rural, no solo reducirán la complejidad inicial de los cálculos matemáticos, sino que adquirirán competencias técnicas para solucionar problemas energéticos reales y apremiantes de nuestro contexto regional.

+1

A lo largo de esta sesión, emplearemos una **metodología híbrida**: utilizarán la RV para la exploración e identificación de variables , se desconectarán físicamente del visor para aplicar el rigor del cálculo de ingeniería tradicional (lápiz y papel), y volverán al entorno virtual para someter su diseño a validación matemática y técnica. Al concluir, comprenderán el diseño solar como un sistema integral, desarrollando el criterio analítico necesario para la toma de decisiones.

+1

* * *

Esta justificación me parece impecable para presentarla ante los jurados y para motivar a los estudiantes, demostrando que están resolviendo problemas de su propia región.

¿Continuamos redactando la **Sección 2 (Objetivos)** y la **Sección 3 (Marco Teórico)** integrando esta dinámica de cálculo híbrido (RV + Papel) y asegurando que las fórmulas sean claras para su nivel?

## Prompt:
Continuemos con la sección de Objetivos.

## Response:
Aquí tienes la redacción detallada para la sección de Objetivos, manteniendo el rigor académico, conectando con el sílabo de Instrumentación Industrial y empleando los lineamientos de tu documento de diseño de la prueba piloto:

* * *

### 2\. Objetivos de Aprendizaje y Competencias

Esta sesión de laboratorio inmersivo tiene como propósito fundamental evaluar la efectividad del videojuego educativo en realidad virtual como herramienta de aprendizaje para comprender el dimensionamiento básico de sistemas fotovoltaicos, el análisis energético y la toma de decisiones técnicas. Al finalizar la práctica, el estudiante habrá consolidado las siguientes metas:

#### 2.1. Objetivo General

Diseñar y dimensionar integralmente un sistema fotovoltaico autónomo (_off-grid_) utilizando un entorno de simulación en Realidad Virtual (RV) y herramientas de cálculo tradicional, aplicando los principios fundamentales de circuitos eléctricos de corriente continua (DC) y alterna (AC) para satisfacer una demanda energética específica.

#### 2.2. Objetivos Específicos

Para alcanzar el objetivo general, el estudiante deberá completar secuencialmente las siguientes metas de aprendizaje:

1.  **Identificar y cuantificar la demanda energética:** Reconocer las cargas eléctricas disponibles en el entorno inmersivo e interpretar su consumo energético diario, aplicando la relación matemática entre potencia nominal y tiempo de operación.
2.  **Analizar la eficiencia de conversión eléctrica:** Comprender el impacto de las pérdidas del sistema y realizar la conversión matemática de las cargas de corriente alterna (AC) a su equivalente en corriente continua (DC).
3.  **Diseñar el arreglo de generación fotovoltaica:** Dimensionar un arreglo fotovoltaico funcional, determinando la cantidad de módulos solares requeridos y su configuración de conexión (en serie o paralelo) para satisfacer las exigencias de tensión y corriente del diseño.
4.  **Dimensionar el sistema de almacenamiento:** Calcular y dimensionar correctamente el banco de baterías para garantizar los días de reserva (autonomía) del sistema, aplicando factores de corrección técnicos y parámetros seguros de descarga.

#### 2.3. Competencias a Desarrollar (Relación con Instrumentación Industrial)

Esta práctica permite a los estudiantes relacionar la teoría energética con decisiones prácticas y comprender el diseño fotovoltaico como un sistema integral, aterrizando los conceptos de la asignatura en habilidades aplicadas:

*   **Aplicación de Circuitos Eléctricos (Unidad 2):** El estudiante dejará de ver la corriente y el voltaje como meros conceptos abstractos. Comprenderá operativamente que, al conectar paneles o baterías en **serie**, se suma el potencial eléctrico (Voltaje) para alcanzar los requerimientos operativos del inversor; mientras que la conexión en **paralelo** permite sumar la capacidad de corriente (Amperaje).
*   **Análisis de Procesos Industriales (Unidades 1 y 3):** El estudiante afianzará la comprensión lógica de un proceso estructurado. Visualizará el sistema fotovoltaico como un diagrama de bloques secuencial: Captación (Paneles)  $\to$  Regulación  $\to$  Almacenamiento (Baterías)  $\to$  Inversión (DC a AC)  $\to$  Consumo final.
*   **Criterio Técnico bajo Restricciones Reales:** Aprenderán que, en la ingeniería aplicada, los sistemas no poseen una eficiencia del 100%. Desarrollarán el criterio analítico para sobredimensionar matemáticamente el sistema y compensar las pérdidas inherentes a la transmisión y transformación de la energía.

* * *

Esta estructura cumple con los criterios SMART y deja muy claro para los evaluadores cómo el _serious game_ se articula con el currículo oficial del programa de Ingeniería Industrial.

Si esta sección te parece sólida, el siguiente paso es redactar el **Marco Teórico (Sección 3)**, donde daremos un "repaso" conceptual muy preciso sobre paneles, inversores y baterías, adaptado para estudiantes que apenas están viendo las bases de corriente y resistencia eléctrica. ¿Te parece bien que avancemos con esa sección?

## Prompt:
Continuemos con la siguiente sección. El Marco Teorico. Este debe detallar los conceptos más básicos de electricidad, luego los conceptos generales de los sistemas fotovoltaicos, luego el procedimiento de diseño (a pesar de que este se desarrolle en el juego paso a paso, considero que tenerlo en esta sección es fundamental para su estudio previo a la ejecución), etc.

## Response:
Aquí tienes la propuesta detallada para la sección del Marco Teórico. Tal como sugieres, estructurarlo de manera progresiva —desde los principios eléctricos hasta el algoritmo de diseño— es vital para que el estudiante utilice esta guía como material de estudio previo a la práctica inmersiva.

* * *

### 3\. Marco Teórico

Para comprender y dimensionar adecuadamente un sistema de generación fotovoltaica autónomo (_off-grid_), es indispensable dominar tanto los principios eléctricos que rigen el comportamiento de la energía, como la función específica de cada componente dentro del sistema.

#### 3.1. Fundamentos de Electricidad y Circuitos

Antes de diseñar el sistema, repasaremos los conceptos fundamentales abordados en la asignatura de Instrumentación Industrial:

*   **Potencia Eléctrica (W):** Es la cantidad de energía consumida o generada por un elemento en un instante de tiempo. Se mide en Vatios (Watts). Matemáticamente, es el producto del voltaje y la corriente ( $P=V\times I$ ).
*   **Energía Eléctrica (Wh):** Representa el consumo o generación de potencia a lo largo del tiempo. Es el factor principal para nuestra auditoría energética. Su ecuación básica es:
    $$
    Energıˊa=Potencia\times Tiempo
    $$
*   **Corriente Continua (DC) vs. Corriente Alterna (AC):** Los sistemas fotovoltaicos operan de forma mixta. Los paneles solares y las baterías generan y almacenan energía en Corriente Continua (DC), donde el flujo de electrones es unidireccional. Por el contrario, la mayoría de los electrodomésticos e instrumentos finales operan en Corriente Alterna (AC). Para vincular ambos circuitos se requiere un equipo de transformación (Inversor).
*   **Conexiones de Circuitos (Leyes de Kirchhoff):** \* **Conexión en Serie:** Se conectan los polos opuestos (+ con -). En esta configuración, la **tensión (Voltaje) se suma**, mientras que la corriente (Amperaje) se mantiene constante.
    +1
    *   **Conexión en Paralelo:** Se conectan los polos iguales (+ con +, - con -). En esta configuración, la **corriente (Amperaje) se suma**, mientras que el voltaje se mantiene constante.
        +1

#### 3.2. Sistemas Fotovoltaicos Autónomos

La energía solar fotovoltaica convierte la radiación solar directamente en energía eléctrica mediante el efecto fotovoltaico, un fenómeno físico en el que la luz solar excita los electrones en materiales semiconductores.

Los sistemas autónomos se utilizan en áreas sin acceso a la red eléctrica (como zonas rurales e industriales remotas). Estos sistemas están compuestos principalmente por:

+1

1.  **Módulos Fotovoltaicos (Paneles):** Arreglo de células solares que captan la radiación y generan corriente DC.
    +1
2.  **Regulador de Carga:** Protege el banco de baterías contra sobrecargas o descargas profundas.
3.  **Banco de Baterías:** Almacena la energía en DC para garantizar la autonomía del sistema durante la noche o días nublados.
4.  **Inversor (DC/AC):** Transforma la energía de las baterías (DC) a corriente alterna (AC) para el consumo final. Este proceso tiene pérdidas térmicas, por lo que su eficiencia suele rondar el 90%.
    +1
![a standalone solar photovoltaic system diagram, generada por IA](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcTeBsRNsyFWm7UErN6oLRq3M0mekyOnh_OLGZFvhqpd9Cp8e0tH4sqI-fJNaFw0XQkqQ11bXBOnIAEI3Ix2-_JKupAGuU530JToW3Sex4sx4c5lfBw)
Shutterstock

#### 3.3. Procedimiento Matemático de Diseño y Dimensionamiento

Durante la sesión, aplicaremos un algoritmo de diseño secuencial de 8 etapas. **Este es el flujo de cálculo que deberá aplicar en su formato de lápiz y papel (Fase 2) antes de validar los datos en el entorno de Realidad Virtual:**

*   **Etapa 1: Energía por Carga** Determine la demanda diaria de cada equipo identificado.
    $$
    Energıˊa\left(Wh\right)=Potencia\left(W\right)\times Tiempo\left(h\right)
    $$
    +1
*   **Etapa 2: Conversión de Cargas AC a DC** Dado que las baterías entregan DC, el consumo de los equipos AC debe ajustarse dividiéndolo por la eficiencia del inversor (0.9).
    +1
    $$
    Energıˊa_{DC_equiv}=\frac{Energıˊa_{AC}}{0.9}
    $$
*   **Etapa 3: Energía Total Diaria** Se consolida el requerimiento sumando las cargas nativas en DC y las cargas convertidas de AC a DC.
    +1
    $$
    Energıˊa_{Total}=Energıˊa_{DC}+Energıˊa_{DC_equiv}
    $$
*   **Etapa 4: Requerimiento en Amperios-hora (Ah)** Seleccione la tensión nominal del banco de baterías (12 V, 24 V o 48 V).
    +1
    $$
    Requerimiento_{diario}\left(Ah/dia\right)=\frac{Energıˊa_{Total}\left(Wh/dia\right)}{Tensioˊn_{nominal}\left(V\right)}
    $$
*   **Etapa 5: Demanda Final con Pérdidas del Sistema** Ajuste el requerimiento diario asumiendo una pérdida del 10% (cables, regulador, etc.), es decir, una eficiencia del 0.9.
    +1
    $$
    Demanda_{final}\left(Ah/dia\right)=\frac{Requerimiento_{diario}}{0.9}
    $$
*   **Etapa 6: Corriente Total Requerida** Utilice las Horas de Sol Equivalente (ESH) de la zona para saber cuánta corriente debe entregar el arreglo de paneles.
    +1
    $$
    Corriente_{requerida}\left(A\right)=\frac{Demanda_{final}\left(Ah/dia\right)}{ESH\left(h/dia\right)}
    $$
*   **Etapa 7: Dimensionamiento del Arreglo Fotovoltaico (Módulos)** A partir de la ficha técnica del panel virtual seleccionado ( $V_{mp}$  e  $I_{mp}$ ), determine las conexiones:
    +1
    *   **Módulos en paralelo ( $N_{p}$ ):**
        $$
        N_{paralelo}=\frac{Corriente_{requerida}\left(A\right)}{I_{mp}}
        $$
        +1
    *   **Módulos en serie ( $N_{s}$ ):**
        $$
        N_{serie}=\frac{Voltaje_{nominal_sistema}}{V_{mp}}
        $$
        _(Nota técnica: A efectos de esta simulación académica, utilice esta relación teórica)._
        +1
    *   **Total de módulos:**
        $$
        Total=N_{paralelo}\times N_{serie}
        $$
*   **Etapa 8: Dimensionamiento del Banco de Baterías** Defina los días de reserva o autonomía.
    +1
    *   **Capacidad Requerida:**
        $$
        Capacidad_{req}\left(Ah\right)=Demanda_{final}\times Dıˊas_{reserva}
        $$
    *   **Capacidad Nominal (Ajuste por Descarga):** Asumiendo una profundidad de descarga segura (DoD) del 80%.
        $$
        Capacidad_{nominal}\left(Ah\right)=\frac{Capacidad_{req}}{0.8}
        $$
    *   **Baterías en Serie:**
        $$
        N_{serie}=\frac{Voltaje_{nominal_sistema}\left(V\right)}{Voltaje_{baterıˊa}\left(V\right)}
        $$
        +1
    *   **Baterías en Paralelo:**
        $$
        N_{paralelo}=\frac{Capacidad_{nominal_requerida}}{Capacidad_{baterıˊa}}
        $$

* * *

Esta sección provee a los estudiantes todo el sustento teórico y analítico antes de ponerse el visor. ¿Te gustaría que avancemos a la sección final detallando las **Métricas de Evaluación y Entregables** (el formato que el estudiante te entregará)?

## Prompt:
Me gustaroia explicar en mas detalle los del 3.3, indicando porque esos pasos, porqué esa secuencia, que hace cada uno, ¿me explico?

## Response:
Comprendo perfectamente. Como docentes de ingeniería, sabemos que si los estudiantes solo memorizan y aplican fórmulas a ciegas, no están haciendo ingeniería; están haciendo aritmética. Necesitan entender la lógica del flujo del proceso.

El diseño de un sistema fotovoltaico se calcula "de atrás hacia adelante" (desde la carga final hasta el panel que capta la energía). Vamos a desglosar la sección 3.3 para explicar el _porqué_ de cada paso y cómo se conectan lógicamente, dándole un enfoque de análisis de procesos.

Aquí tienes la versión ampliada y detallada de esa sección:

* * *

#### 3.3. Lógica y Procedimiento Matemático de Diseño

El dimensionamiento de un sistema fotovoltaico autónomo no es una colección de fórmulas aisladas, sino un proceso secuencial. Como en cualquier diseño industrial, partimos de conocer la necesidad final (la demanda del usuario), calculamos las ineficiencias del proceso de transporte y transformación, y con ese total determinamos cuánta materia prima (energía solar y baterías) necesitamos instalar.

+1

A continuación, se detalla la lógica detrás de las 8 etapas de cálculo que deberá aplicar:

**Fase 1: Auditoría de la Demanda (¿Cuánta energía necesito?)**

*   **Etapa 1: Energía por Carga**
    *   _¿Qué hace?_ Convierte la potencia instantánea de un equipo en un volumen de energía consumida en el tiempo.
    *   _¿Por qué?_ Saber que un televisor consume 100 W no nos dice mucho; necesitamos saber cuánto "tamaño" de energía extraerá de la batería. Si se usa 5 horas, extraerá 500 Wh.
    *   _Fórmula:_  $Energıˊa=Potencia\times Tiempo$ 
*   **Etapa 2: Conversión de Cargas AC a DC**
    *   _¿Qué hace?_ Ajusta el consumo de los equipos domésticos (que operan en Corriente Alterna) al "idioma" de las baterías (Corriente Directa).
    *   _¿Por qué?_ El inversor que transforma la DC en AC no es perfecto; genera calor. Ese calor es energía perdida (usualmente un **10%**). Por tanto, para entregar 100 Wh en AC, debemos extraer aproximadamente 111 Wh de la batería en DC. Para calcularlo, dividimos entre la eficiencia del inversor (**0.9**).
    *   _Fórmula:_  $Energıˊa_{DC_equiv}=\frac{Energıˊa_{AC}}{0.9}$ 
*   **Etapa 3: Energía Total Diaria**
    *   _¿Qué hace?_ Unifica todos los consumos en un solo valor diario.
    *   _¿Por qué?_ Nos da el "tamaño del tanque" diario que nuestro sistema debe llenar.
    *   _Fórmula:_  $Energıˊa_{Total}=Energıˊa_{DC}+Energıˊa_{DC_equiv}$ 

**Fase 2: Adaptación al Sistema Eléctrico (¿A qué presión y caudal trabajaré?)**

*   **Etapa 4: Requerimiento en Amperios-hora (Ah)**
    *   _¿Qué hace?_ Traduce la energía (Wh) a capacidad de corriente en el tiempo (Ah), que es la unidad estándar comercial de las baterías.
    *   _¿Por qué?_ Debemos elegir una "presión" de trabajo para el sistema (**12 V**, **24 V** o **48 V**). A mayor voltaje, menor será la corriente requerida para la misma energía, lo que permite usar cables más delgados y reduce los riesgos de sobrecalentamiento.
    *   _Fórmula:_  $Requerimiento_{diario}\left(Ah/dia\right)=\frac{Energıˊa_{Total}\left(Wh/dia\right)}{Tensioˊn_{nominal}\left(V\right)}$ 
*   **Etapa 5: Demanda Final con Pérdidas del Sistema**
    *   _¿Qué hace?_ Agrega un margen de seguridad por ineficiencias físicas.
    *   _¿Por qué?_ Los cables tienen resistencia, las conexiones se calientan y el regulador de carga pierde energía. Asumimos una eficiencia general del sistema del **90%** (pérdida del **10%**). Sobredimensionamos la demanda dividiendo entre **0.9** para asegurar que la energía final entregada sea la correcta.
        +1
    *   _Fórmula:_  $Demanda_{final}=\frac{Requerimiento_{diario}}{0.9}$ 

**Fase 3: Dimensionamiento de la Generación (Paneles)**

*   **Etapa 6: Corriente Total Requerida**
    *   _¿Qué hace?_ Calcula cuántos Amperios deben inyectar los paneles durante las horas útiles de sol.
        +2
    *   _¿Por qué?_ El sol no brilla con la misma fuerza todo el día. Usamos el concepto de Horas de Sol Equivalente (ESH), que comprime toda la radiación del día en unas pocas horas de rendimiento al 100%.
    *   _Fórmula:_  $Corriente_{requerida}\left(A\right)=\frac{Demanda_{final}\left(Ah/dia\right)}{ESH\left(h/dia\right)}$ 
*   **Etapa 7: Dimensionamiento del Arreglo Fotovoltaico (Módulos)**
    *   _¿Qué hace?_ Define la cantidad física de paneles y cómo se conectarán.
        +1
    *   _¿Por qué en Paralelo?_ Para alcanzar la corriente total calculada en la etapa anterior. Se divide la corriente requerida entre la corriente que aporta un solo panel ( $I_{mp}$ ).
        +1
    *   _¿Por qué en Serie?_ Para alcanzar el voltaje nominal del sistema. Se divide el voltaje del sistema entre el voltaje que aporta un solo panel ( $V_{mp}$ ).
        +2
    *   _Fórmulas:_ \*  $N_{paralelo}=\frac{Corriente_{requerida}\left(A\right)}{I_{mp}}$ 
        *    $N_{serie}=\frac{Voltaje_{nominal_sistema}}{V_{mp}}$ 
        *    $Total=N_{paralelo}\times N_{serie}$ 

**Fase 4: Dimensionamiento del Almacenamiento (Baterías)**

*   **Etapa 8: Dimensionamiento del Banco de Baterías**
    *   _¿Qué hace?_ Define cuántas baterías se necesitan para soportar el sistema cuando no hay sol.
    *   _Días de Reserva (Autonomía):_ Se multiplica la demanda diaria por los días nublados consecutivos que el sistema debe soportar (ej. **5 días**).
    *   _Profundidad de Descarga (DoD):_ Bajar la carga de una batería a cero la destruye rápidamente. Para prolongar su vida útil, calculamos una batería más grande de lo que necesitamos para solo usar, por ejemplo, el **80%** de su capacidad (dividiendo entre **0.8**).
    *   _Conexiones:_ Al igual que los paneles, las baterías se conectan en serie para sumar voltaje (alcanzando los **12 V** o **24 V** del sistema) y en paralelo para sumar la capacidad en Ah .

* * *

¿Esta explicación te parece que le da mucho más sentido ingenieril a las fórmulas? Si estás de acuerdo, podemos avanzar a detallar la última sección: las Métricas de Evaluación y los entregables de la práctica.

## Prompt:
Redactalos en parrafos, sin las preguntas.

Las matematicas asignalas así:

\$\$

fx

\$\$

## Response:
Aquí tienes la redacción de la sección 3.3 ajustada a un formato de párrafos descriptivos, eliminando la estructura de preguntas y respuestas, y aplicando rigurosamente el formato matemático solicitado para los bloques de ecuaciones.

* * *

#### 3.3. Lógica y Procedimiento Matemático de Diseño

El dimensionamiento de un sistema fotovoltaico autónomo es un proceso analítico secuencial que se calcula en sentido inverso al flujo de la energía: partimos de la necesidad final del usuario, compensamos las ineficiencias del proceso de transformación y transporte, y finalmente determinamos la cantidad de generación y almacenamiento requerida. A continuación, se detalla la justificación técnica de las 8 etapas de cálculo que deberá aplicar en su diseño.

+1

**Fase 1: Auditoría de la Demanda Energética**

En la primera etapa, el objetivo es convertir la potencia instantánea de cada equipo identificado en un volumen de energía consumida a lo largo del tiempo. Conocer únicamente la potencia nominal en vatios (W) es insuficiente; es indispensable multiplicarla por el tiempo de operación estimado en horas (h) para dimensionar la extracción real de energía.

+1

$$
Energıˊa\left(Wh\right)=Potencia\left(W\right)\times Tiempo\left(h\right)
$$

Posteriormente, en la etapa dos, se debe realizar la conversión de las cargas de corriente alterna (AC). Dado que el banco de baterías entrega energía en corriente continua (DC), el consumo de los equipos electrodomésticos debe ajustarse para compensar las ineficiencias térmicas del inversor. Asumiendo una eficiencia de conversión del 90%, la energía solicitada a las baterías será matemáticamente mayor al consumo real del equipo AC.

+1

$$
Energıˊa_{DC_equiv}=\frac{Energıˊa_{AC}}{0.9}
$$

Para concluir la primera fase, la etapa tres unifica todos los requerimientos energéticos calculados. Se consolida la demanda sumando las cargas nativas en DC y las cargas equivalentes convertidas de AC, obteniendo así el requerimiento energético total diario de la instalación.

+1

$$
Energıˊa_{Total}=Energıˊa_{DC}+Energıˊa_{DC_equiv}
$$

**Fase 2: Adaptación al Sistema Eléctrico**

En la etapa cuatro, se traduce la energía total (Wh) a capacidad de corriente en el tiempo (Ah), la cual es la unidad estándar comercial para el dimensionamiento de baterías. Para ello, el diseñador debe establecer la tensión nominal de operación del sistema, seleccionando típicamente entre 12 V, 24 V o 48 V. Operar a mayor voltaje permite reducir la corriente transitada, minimizando así las caídas de tensión y el calibre del cableado requerido.

+1

$$
Requerimiento_{diario}\left(Ah/dia\right)=\frac{Energıˊa_{Total}\left(Wh/dia\right)}{Tensioˊn_{nominal}\left(V\right)}
$$

La etapa cinco introduce un margen de seguridad esencial para compensar las ineficiencias físicas del sistema. Los conductores eléctricos presentan resistencia, las conexiones disipan calor y los reguladores de carga consumen energía en su operación. Para garantizar que la demanda final sea satisfecha plenamente, se asume una eficiencia general del sistema del 90%, lo que obliga a sobredimensionar el requerimiento diario calculado previamente.

+2

$$
Demanda_{final}\left(Ah/dia\right)=\frac{Requerimiento_{diario}\left(Ah/dia\right)}{0.9}
$$

**Fase 3: Dimensionamiento de la Generación Fotovoltaica**

En la etapa seis, se determina la inyección de corriente necesaria por parte del arreglo de paneles. Debido a que la radiación solar fluctúa a lo largo del día, se utiliza el parámetro de Horas de Sol Equivalente (ESH), el cual estandariza la radiación disponible asumiendo un rendimiento pleno.

+2

$$
Corriente_{requerida}\left(A\right)=\frac{Demanda_{final}\left(Ah/dia\right)}{ESH\left(h/dia\right)}
$$

La etapa siete define la arquitectura física del generador solar basándose en la ficha técnica del módulo seleccionado, específicamente en su tensión de máxima potencia ( $V_{mp}$ ) y su corriente de máxima potencia ( $I_{mp}$ ). Para satisfacer la demanda de corriente calculada, los paneles se agrupan en paralelo. Simultáneamente, para alcanzar la tensión nominal del sistema, se conectan en serie. El tamaño final del arreglo es el producto de ambas configuraciones.

+4

$$
N_{paralelo}=\frac{Corriente_{requerida}\left(A\right)}{I_{mp}}
$$

$$
N_{serie}=\frac{Voltaje_{nominal_sistema}\left(V\right)}{V_{mp}}
$$

$$
Total_{moˊdulos}=N_{paralelo}\times N_{serie}
$$

**Fase 4: Dimensionamiento del Almacenamiento**

Finalmente, en la etapa ocho, se estructura el banco de baterías responsable de mantener la autonomía energética. Primero, se calcula la capacidad bruta requerida multiplicando la demanda final por los días de reserva estipulados para soportar periodos sin radiación solar. Sin embargo, para preservar la vida útil de los acumuladores, se aplica un factor de profundidad de descarga (DoD). Al limitar la descarga a un máximo del 80%, la capacidad nominal requerida se incrementa matemáticamente. Una vez obtenida esta capacidad, las unidades físicas se disponen en configuraciones serie y paralelo para cumplir con la tensión y capacidad calculadas.

+4

$$
Capacidad_{requerida}\left(Ah\right)=Demanda_{final}\left(Ah/dia\right)\times Dıˊas_{reserva}
$$

$$
Capacidad_{nominal}\left(Ah\right)=\frac{Capacidad_{requerida}\left(Ah\right)}{0.8}
$$

$$
N_{serie_baterias}=\frac{Voltaje_{nominal_sistema}\left(V\right)}{Voltaje_{baterıˊa}\left(V\right)}
$$

$$
N_{paralelo_baterias}=\frac{Capacidad_{nominal}\left(Ah\right)}{Capacidad_{baterıˊa}\left(Ah\right)}
$$

## Prompt:
Continuemos con la sección de procedimiento.

## Response:
A continuación, presento la redacción de la **Sección 4: Procedimiento de la Práctica**.

Esta sección estructura la metodología híbrida que acordamos, dividiendo la carga de trabajo entre el entorno inmersivo y el cálculo analítico tradicional. Además, integra las encuestas diagnósticas y de retroalimentación que el proyecto de investigación exige.

+2

* * *

### 4\. Procedimiento de la Práctica

El desarrollo de esta práctica se rige bajo una metodología de aprendizaje experiencial e híbrido. Para garantizar la asimilación técnica y minimizar la fatiga visual propia de los entornos inmersivos, la sesión alterna entre la interacción en Realidad Virtual (RV) y el cálculo analítico en estación de trabajo.

El tiempo estimado para la ejecución total del laboratorio es de 45 a 50 minutos. Se requiere el uso de calculadora, libreta de apuntes y seguir estrictamente las siguientes fases:

**Fase Pre-Laboratorio: Diagnóstico Inicial**

1.  Antes de iniciar la interacción con los equipos, el estudiante deberá diligenciar la encuesta diagnóstica inicial provista por el docente.
    +1
2.  Este instrumento tiene como objetivo establecer la línea base de sus conocimientos teóricos en energía solar, circuitos eléctricos y su nivel de experiencia previa con tecnologías de Realidad Virtual.

**Fase 1: Auditoría Energética Inmersiva (Tiempo estimado: 10 min)**

1.  Colóquese el visor de RV (Meta Quest) y acceda a la simulación inicial correspondiente al escenario residencial (La Mudanza).
2.  Recorra el entorno virtual con el propósito de identificar las cargas eléctricas disponibles (electrodomésticos y equipos electrónicos).
3.  Seleccione los objetos que requerirán suministro eléctrico en la locación remota y deposítelos en el vehículo de carga dispuesto en la simulación.
4.  Al interactuar con cada equipo, la interfaz de usuario desplegará sus especificaciones técnicas. Registre cuidadosamente en su libreta de apuntes la **potencia nominal (W)** y el **tiempo de operación diario estimado (h)** de cada carga. Esta recolección de datos es el insumo fundamental para su diseño.

**Fase 2: Dimensionamiento Analítico (Tiempo estimado: 20 min)**

1.  Retírese el visor de RV para realizar el trabajo de escritorio.
2.  Utilizando los datos recolectados en la Fase 1, aplique el algoritmo matemático de 8 etapas detallado en la **Sección 3.3** de esta guía.
3.  Deberá calcular y registrar de manera estructurada:
    *   El consumo energético de cada equipo y su conversión equivalente a corriente continua (DC).
    *   La demanda total diaria consolidada y ajustada con el factor de pérdidas del sistema (eficiencia del 0.9).
    *   La configuración del arreglo fotovoltaico (cantidad de módulos conectados en serie y en paralelo).
    *   La configuración del banco de baterías, garantizando los días de autonomía definidos por el docente y respetando el límite de profundidad de descarga (DoD).

**Fase 3: Validación Técnica en el Entorno Virtual (Tiempo estimado: 10 min)**

1.  Vuelva a colocarse el visor de RV e ingrese a la segunda etapa del _serious game_: la interfaz del "Centro de Cálculos" o panel de diseño del sistema.
2.  Introduzca las configuraciones paramétricas (número de paneles, arreglo serie/paralelo, capacidad de baterías) que obtuvo en su análisis manual.
3.  Ejecute la validación dentro del simulador. El sistema evaluará el balance energético de su propuesta; si los cálculos garantizan la estabilidad y autonomía del sistema para las cargas seleccionadas, la instalación será aprobada. Si el sistema arroja fallos por subdimensionamiento o sobrecarga, deberá revisar sus cálculos matemáticos e iterar su diseño.
    +2

**Fase Post-Laboratorio: Evaluación y Cierre**

1.  Tras finalizar la simulación y retirarse los equipos, el estudiante deberá completar la encuesta de salida.
2.  Esta evaluación medirá tanto la comprensión técnica adquirida (conceptos de cálculo de energía diaria, relación de tensión/corriente y dimensionamiento) , como la percepción ergonómica de la herramienta virtual (facilidad de uso, nivel de inmersión y presencia de fatiga visual o mareo).
    +2
3.  Finalmente, entregue al evaluador su hoja de cálculos analíticos (Fase 2) como soporte del trabajo de ingeniería realizado.

* * *

Con esta sección, el estudiante sabe exactamente qué tiene que hacer, en qué orden, y con qué propósito.

Para finalizar la guía, nos quedaría estructurar la **Sección 5: Entregables y Criterios de Evaluación**. Allí podemos especificar qué debe contener esa "hoja de cálculos analíticos" y cómo se medirá su éxito. ¿Avanzamos con esta última parte?

## Prompt:
Perfecto, continuemos con esa sección

## Response:
A continuación, presento la redacción de la última sección de la guía. Esta parte es fundamental para formalizar el compromiso del estudiante y para recolectar los datos requeridos por tu diseño experimental (validación del _serious game_).

* * *

### 5\. Entregables y Criterios de Evaluación

Esta práctica de laboratorio no solo evalúa el desempeño académico en la asignatura de Instrumentación Industrial, sino que forma parte de una prueba piloto para validar tecnologías inmersivas en la enseñanza de la ingeniería. Por lo tanto, la evaluación se dividirá en la entrega de soportes físicos y el análisis de las métricas obtenidas dentro del simulador.

+3

#### 5.1. Entregables del Laboratorio

Al finalizar la sesión, el estudiante (o su equipo de trabajo) deberá entregar al docente los siguientes soportes:

1.  **Encuestas de la prueba piloto:** Entrega formal de la encuesta diagnóstica inicial y la encuesta posterior de retroalimentación.
    +2
2.  **Hoja de Auditoría Energética:** Un listado claro con los equipos identificados en la simulación (Fase 1), detallando su potencia nominal (W) y tiempo de uso estimado (h).
3.  **Memoria de Cálculos Analíticos:** El desarrollo matemático estructurado de las 8 etapas de dimensionamiento (Fase 2), demostrando el cálculo de:
    *   Energía total diaria (incluyendo conversión AC/DC).
        +1
    *   Demanda final ajustada por pérdidas del sistema.
        +1
    *   Dimensionamiento del arreglo fotovoltaico (cálculo de módulos en serie y paralelo).
        +1
    *   Dimensionamiento del banco de baterías (incluyendo días de reserva y factor de profundidad de descarga).
        +2

#### 5.2. Criterios de Evaluación Cuantitativa

El desempeño técnico se medirá a través de las variables registradas directamente por el sistema de puntuación del _serious game_:

+1

*   **Precisión del diseño:** Se evaluará el número de decisiones correctas al ingresar los parámetros en el Centro de Cálculos virtual.
*   **Eficiencia operativa:** Se medirá el tiempo total de resolución requerido para completar la validación técnica en el entorno virtual.
*   **Iteraciones:** Se contabilizará el número de intentos necesarios para lograr un diseño funcional. (Un alto número de intentos sugiere fallos en la Fase 2 de cálculo analítico).
*   **Puntaje global:** Puntaje final obtenido y registrado en el juego.

#### 5.3. Criterios de Evaluación Cualitativa

Adicional a los cálculos, se evaluará la asimilación conceptual y la experiencia tecnológica del usuario:

*   **Asimilación de conceptos:** Medida a través de la encuesta post-experiencia, evaluando si el estudiante comprende la relación entre tensión y corriente, la conversión de energía diaria y la justificación técnica detrás del dimensionamiento de baterías.
*   **Experiencia de Usuario (UX):** Se recolectarán datos sobre la facilidad de interacción en la realidad virtual, la claridad de las interfaces, el nivel de inmersión y la posible presencia de fatiga o mareo durante la simulación.
    +2

* * *



---
Powered by [Gemini Exporter](https://www.ai-chat-exporter.com)