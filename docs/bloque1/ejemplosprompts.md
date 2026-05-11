# Ejemplos

## Ejemplos *trigger words*

A continuación se presentan tres ejemplos de prompts que emplean **palabras desencadenantes** para guiar el tipo de respuesta generada por un modelo de lenguaje.
Estos ejemplos muestran cómo el uso consciente de **trigger words** permite dirigir el comportamiento del modelo hacia análisis, razonamiento estructurado o evaluación crítica.

---

### 1 Prompt analítico

**Trigger words:** *analiza, identifica, concluye*

> **Analiza** el siguiente conjunto de datos de ventas mensuales.  
> **Identifica** las tendencias principales y los posibles factores que las explican.  
> **Concluye** con un breve resumen de las implicaciones para la toma de decisiones empresariales.

*Este prompt fuerza al modelo a estructurar la respuesta en fases de análisis y síntesis.*

---

### 2 Prompt explicativo paso a paso

**Trigger words:** *explica, paso a paso, justifica*

> **Explica paso a paso** cómo se resuelve una ecuación cuadrática utilizando la fórmula general.  
> **Justifica** cada uno de los pasos del procedimiento y utiliza un ejemplo numérico sencillo.

*Las palabras desencadenantes inducen razonamiento secuencial y claridad expositiva.*

> **Explica** cómo se resuelve una ecuación cuadrática usando la fórmula general.
> **Incluye** un ejemplo numérico sencillo.

---

### 3 Prompt comparativo y crítico

**Trigger words:** *compara, evalúa, argumenta*

> **Compara** los modelos de bases de datos relacional y NoSQL.  
> **Evalúa** sus ventajas e inconvenientes en el contexto de aplicaciones web a gran escala.  
> **Argumenta** en qué casos sería más adecuado utilizar cada uno.

*Este prompt orienta al modelo hacia una respuesta crítica y razonada, no meramente descriptiva.*

---

## Ejemplos *Chain of Thought (CoT)*

A continuación se muestran tres ejemplos que solicitan explícitamente **razonamiento paso a paso** para mejorar la calidad de la respuesta en tareas complejas.

---

### 1 Problema cuantitativo 
Razonamiento paso a paso

> Resuelve el siguiente problema **razonando paso a paso** y mostrando los cálculos intermedios:  
> Un tren sale de la estación A hacia B a 60 km/h. Al mismo tiempo, otro tren sale de B hacia A a 80 km/h. La distancia entre A y B es 300 km.  
> 1) ¿En qué punto se encuentran?  
> 2) ¿Cuánto tiempo ha pasado desde la salida?  
> Al final, incluye un **resumen** con el resultado y las unidades.

---

### 2 Decisión multicriterio
CoT + estructura

> Quiero que me ayudes a decidir entre dos ideas de emprendimiento.  
> - Idea A: tienda online de artículos y accesorios para mujeres.  
> - Idea B: promoción de productos por internet con comisiones de afiliados.  
> **Piensa paso a paso** evaluando: inversión inicial, riesgo, escalabilidad, tiempo hasta ingresos, complejidad operativa y sostenibilidad.  
> Devuelve la respuesta con esta estructura:
> 1. Análisis comparativo (criterio por criterio)  
> 2. Recomendación final  
> 3. Plan de acción en 5 pasos

---

### 3 Optimización de ruta
CoT + verificación

> Planeo un viaje de un día y quiero visitar cinco lugares minimizando el tiempo total de desplazamiento:  
> 1. Museo  
> 2. Parque  
> 3. Centro comercial  
> 4. Restaurante  
> 5. Teatro  
> Distancias (minutos) entre cada par:  
> - Museo–Parque: 10  
> - Museo–Centro comercial: 15  
> - Museo–Restaurante: 20  
> - Museo–Teatro: 25  
> - Parque–Centro comercial: 10  
> - Parque–Restaurante: 15  
> - Parque–Teatro: 20  
> - Centro comercial–Restaurante: 10  
> - Centro comercial–Teatro: 15  
> - Restaurante–Teatro: 10  
> Genera una ruta inicial y luego **optimízala paso a paso**, **evaluando cada cambio** antes de aplicar el siguiente.  
> Al final, proporciona:
> - Ruta final  
> - Tiempo total  
> - Breve explicación del porqué es mejor que la inicial

---

## Ejemplos de prompts con *Priming*

A continuación se presentan tres ejemplos de prompts que emplean la técnica de **priming** para influir en el estilo, nivel y enfoque de las respuestas generadas por un modelo de lenguaje.

Estos ejemplos muestran cómo el **priming** permite preparar al modelo antes de la tarea principal, mejorando la adecuación de las respuestas al contexto y a los objetivos del usuario.

---

### 1 Priming con rol experto

> Actúa como un **profesor universitario de informática especializado en inteligencia artificial**.  
> Explica el funcionamiento básico de los grandes modelos del lenguaje (LLMs) utilizando un lenguaje claro y riguroso, adecuado para estudiantes de último curso de grado.  
> Finaliza con un breve resumen de las ideas clave.

*El priming establece el rol y el nivel académico esperado antes de la generación de la respuesta.*

---

### 2 Priming con estructura y estilo

> Inicia tu respuesta con una **introducción breve**, continúa con una **explicación paso a paso** y finaliza con un **ejemplo práctico sencillo**.  
> El tema a tratar es: la resolución de ecuaciones cuadráticas mediante la fórmula general.  
> Utiliza un lenguaje accesible para alumnado de educación secundaria.

*El priming define explícitamente la estructura y el estilo de la respuesta.*

---

### 3 Priming con contexto de uso

> Imagina que estás asesorando a una **empresa tecnológica que desea adoptar ChatGPT** en sus procesos internos.  
> Describe las **ventajas**, **limitaciones** y **riesgos** de su uso en un entorno profesional.  
> La respuesta debe estar orientada a responsables de toma de decisiones y no superar las 400 palabras.

*El priming contextualiza la situación y condiciona el enfoque de la respuesta.*

---

## Ejemplos de *One-shot* y *Few-shot prompting*

A continuación se presentan ejemplos de prompts que utilizan las técnicas de **one-shot** y **few-shot prompting**, proporcionando uno o varios ejemplos previos para guiar el comportamiento del modelo.

Estos ejemplos ilustran cómo **one-shot** y **few-shot prompting** permiten moldear el comportamiento del modelo mediante ejemplos previos, sin necesidad de reglas explícitas.

---

### 1 One-shot 
con un único ejemplo

> Corrige y mejora la redacción del siguiente texto, haciéndolo más formal.  
>  
> **Ejemplo:**  
> Texto original: *"ola profe, no puedo ir a clase mañana"*  
> Texto corregido: *"Hola profesor, no podré asistir a clase mañana."*  
>  
> **Ahora corrige este texto:**  
> *"buenas tarde. quiero quitarme de la linea del tfno por que ya no uso mas"*

*El modelo dispone de un único ejemplo que actúa como referencia para la tarea.*

---

### 2 One-shot 
formato y estilo

> Resume el siguiente contenido siguiendo el formato del ejemplo.  
>  
> **Ejemplo:**  
> Texto original: *La fotosíntesis es el proceso mediante el cual las plantas...*  
> Resumen: *La fotosíntesis permite a las plantas producir su alimento utilizando la luz solar.*  
>  
> **Texto a resumir:**  
> *La inteligencia artificial es un campo de la informática que estudia...*

*Un solo ejemplo guía el nivel de síntesis y el estilo de la respuesta.*

---

### 3 Few-shot
varios ejemplos

> Clasifica el siguiente prompt según su tipo.  
>  
> **Ejemplos:**  
> Prompt: *"Analiza las causas del cambio climático."*  
> Clasificación: Trigger words  
>  
> Prompt: *"Resuelve este problema razonando paso a paso."*  
> Clasificación: Chain of Thought  
>  
> Prompt: *"Dime cosas sobre plantas."*  
> Clasificación: Prompt ineficiente  
>  
> **Ahora clasifica este prompt:**  
> *"Compara dos lenguajes de programación y argumenta cuál es más adecuado para ciencia de datos."*

*Varios ejemplos permiten al modelo inferir el patrón de clasificación.*

---

### 4 Few-shot 
rol y estilo consistente

> Actúa como un **asistente motivacional** para estudiantes universitarios.  
>  
> **Ejemplos:**  
> Entrada: *"Estoy desmotivado con la asignatura."*  
> Respuesta: *"Es normal sentirse así a veces, pero recuerda todo lo que ya has logrado. Sigue adelante."*  
>  
> Entrada: *"No creo que pueda aprobar el examen."*  
> Respuesta: *"Confía en tu esfuerzo. Has superado retos antes y este no será diferente."*  
>  
> **Ahora responde a:**  
> *"Siento que no avanzo en el proyecto."*

*El few-shot refuerza el tono, el rol y el estilo de respuesta.*

---
## Ejemplo *Tree of Thoughts (ToT)*

### 1 Tree of thoughts

```text
Resuelve el siguiente problema explorando múltiples enfoques posibles.
Organiza tus ideas como un árbol de razonamiento:
- Genera varias opciones en cada paso
- Evalúa brevemente cada una
- Continúa desarrollando las más prometedoras
Finalmente, proporciona la mejor solución encontrada.
```
---

## Ejemplo *Visualization of Thoughts (ToT)*

### 1 Visualization of thoughts

```text
Analiza el problema creando una representación visual de tus pensamientos.
Organiza la información como si fuera un diagrama o mapa conceptual:
- Identifica los elementos principales
- Muestra relaciones entre ellos
- Usa una estructura jerárquica clara
Después, explica la solución final.
```
---

## Ejemplos de prompts con formato

### 1 Especificar el formato de salida

**Texto plano:** Puedo generar respuestas en formato de texto sencillo, que es el formato de salida estándar en la mayoría de las conversaciones.  
**Listas y viñetas:** Puedo crear listas numeradas o con viñetas para organizar información de manera más estructurada.  
**Tablas:** Puedo generar tablas simples con filas y columnas para presentar datos de manera ordenada.  
**Código fuente:** Si necesitas ejemplos de código en lenguajes de programación populares, puedo generar código fuente en formatos como Python, Java, C++, etc.  
**Citas y referencias:** Si necesitas citas o referencias en tus respuestas, puedo proporcionarlas con el formato adecuado, como el estilo APA o MLA.  
**Resúmenes:** Puedo resumir información larga o documentos extensos en un formato más conciso y fácil de entender.  
**Párrafos largos:** Si prefieres respuestas más detalladas y expansivas, puedo generar párrafos largos con explicaciones completas.  
**Traducciones:** Puedo traducir texto de un idioma a otro si es necesario.  
**Resúmenes y extractos de URL's:** Puedo proporcionarte resúmenes o extractos de información contenida en URL's válidas, siempre y cuando no se trate de una fuente de suscripción o privada.  

---
