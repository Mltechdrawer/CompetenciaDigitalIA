# Ingeniería de Prompts
## Prompt Engineering

## 1. Introducción

La **ingeniería de prompts** (*Prompt Engineering*) es la disciplina que estudia cómo **diseñar, formular y optimizar instrucciones** para interactuar de manera eficaz con modelos de lenguaje de gran tamaño (*Large Language Models*, LLMs).

Dado que los LLMs generan sus respuestas en función del texto de entrada, la calidad del *prompt* resulta determinante para obtener respuestas **precisas, coherentes, útiles y alineadas con los objetivos del usuario**.

---

## 2. ¿Qué es un prompt?

Un **prompt** es el texto de entrada que se proporciona a un modelo de lenguaje para guiar la generación de una respuesta. Puede adoptar múltiples formas, desde una pregunta sencilla hasta una instrucción compleja con contexto, ejemplos y restricciones.

Los prompts permiten:  
- Guiar la generación de respuestas.  
- Optimizar el rendimiento del modelo.  
- Adaptar el comportamiento del modelo a distintos contextos.  
- Evaluar la calidad y fiabilidad de las respuestas obtenidas  

---

## 3. Objetivos de la ingeniería de prompts

Los principales objetivos de la ingeniería de prompts son:

1. **Guiar la generación de respuestas**, reduciendo la ambigüedad.
2. **Optimizar el rendimiento del modelo**, obteniendo respuestas más relevantes.
3. **Adaptar el prompt al contexto**, dominio y nivel del usuario.
4. **Evaluar y mejorar la calidad de los prompts**, detectando deficiencias y sesgos.

---

## 4. Anatomía de un prompt

Un prompt eficaz suele componerse de los siguientes elementos:

1. **Claridad y especificidad**  
2. **Contexto y antecedentes**  
3. **Objetivo o propósito**  
4. **Palabras clave y términos relevantes**  
5. **Limitaciones o directrices específicas** 

### Ejemplo de estructura eficiente

- **Introducción:**  
  *Estoy interesado en las prácticas sostenibles en la agricultura moderna.*

- **Pregunta específica:**  
  *¿Podrías explicar cómo las técnicas de agricultura de precisión y la agricultura orgánica contribuyen a la sostenibilidad medioambiental?*

- **Directrices:**  
  *La respuesta debe ser técnica, detallada y no superar las 500 palabras.*

---

## 5. Prompts ineficientes

Un prompt mal diseñado puede generar respuestas vagas o irrelevantes.

**Ejemplo de prompt ineficiente:**
> *“Dime cosas sobre plantas.”*

Este prompt carece de:  
- claridad,  
- contexto,  
- objetivo definido,  

No define qué aspecto de las plantas interesa(biología,uso en jardinería, importancia ecológica, etc.), no proporciona contexto o antecedentes, y no establece un objetivo o propósito claro para la respuesta.
Esta falta de estructura y detalles puede resultar en una respuesta de la IA que no cumpla con las expectativas o necesidades del usuario.

---

## 6. Tipos de prompts

Según su finalidad, los prompts pueden clasificarse en:

1. **Informativos**  
   *Ejemplo:* Explica las causas y efectos del cambio climático.

2. **Creativos**  
   *Ejemplo:* Escribe un cuento corto sobre un viaje a Marte en el año 2100.

3. **Educativos**  
   *Ejemplo:* Describe el proceso de fotosíntesis.

4. **Interactivos**  
   *Ejemplo:* ¿Cuál es tu película favorita y por qué?

5. **Analíticos**  
   *Ejemplo:* Analiza las tendencias de ventas del último trimestre.

6. **Técnicos**  
   *Ejemplo:* Explica el funcionamiento de los motores eléctricos.

---

## 7. Principios de diseño de prompts

Un buen diseño de prompts se basa en los siguientes principios:

1. **Claridad y precisión**  
2. **Especificidad**  
3. **Contexto y relevancia**  
4. **Objetivo definido**  
5. **Concisión**  
6. **Adaptabilidad**  

Estos principios permiten maximizar la utilidad del modelo y reducir respuestas erróneas o ambiguas.

[Delimitadores](delimitadores.md)

---

## 8. Técnicas avanzadas de prompting

### 8.1 Trigger words
Las *trigger words* o **palabras desencadenantes** orientan al modelo hacia un tipo de razonamiento o respuesta concreta, por ejemplo: *analiza*, *justifica*, *compara*, *resume*.

[Analítico](ejemplosprompts.md#1-prompt-analitico)

[Explicativo](ejemplosprompts.md#2-prompt-explicativo-paso-a-paso)

[Comparativo y crítico](ejemplosprompts.md#3-prompt-comparativo-y-critico)

---
### 8.2 Chain of Thought (CoT)

La técnica **Chain of Thought** consiste en pedir explícitamente al modelo que **razone paso a paso**, lo que mejora el rendimiento en problemas complejos.

**Ejemplo:**
> *Resuelve el problema paso a paso, explicando el razonamiento seguido.*

[Problema cuantitativo](ejemplosprompts.md#1-problema-cuantitativo)

[Decisión multicriterio](ejemplosprompts.md#2-decision-multicriterio)

[Optimización de ruta](ejemplosprompts.md#3-optimizacion-de-ruta)

---

### 8.3 Prompt Priming

El **priming** consiste en proporcionar instrucciones iniciales que preparan al modelo antes de la tarea principal.

**Ejemplo:**
> *Inicia tu respuesta con una introducción breve, continúa con un ejemplo paso a paso y finaliza con una pregunta de práctica.*

[Priming con rol experto](ejemplosprompts.md#1-priming-con-rol-experto)

[Priming con estructura y estilo](ejemplosprompts.md#2-priming-con-estructura-y-estilo)

[Priming con contexto de uso](ejemplosprompts.md#3-priming-con-contexto-de-uso)

---

### 8.4 One-shot y Few-shot prompting

- **One-shot:** se proporciona un único ejemplo.
- **Few-shot:** se proporcionan varios ejemplos para guiar el comportamiento del modelo.

Estas técnicas permiten **modelar el estilo, formato y nivel de detalle** de la respuesta.

[One shot un único ejemplo](ejemplosprompts.md#1-one-shot)

[One shot formato y estilo](ejemplosprompts.md#2-one-shot)

[Few shot varios ejemplos](ejemplosprompts.md#3-few-shot)

[Few shot rol y estilo consistente](ejemplosprompts.md#4-few-shot)

### 8.5 Tree of Thoughts (ToT)

La técnica **Tree of Thoughts (ToT)** es una extensión avanzada del enfoque *Chain of Thought* que permite a los modelos de lenguaje **explorar múltiples caminos de razonamiento en paralelo**, organizados en forma de árbol, en lugar de seguir una única secuencia lineal de pensamiento.

#### Idea principal

En lugar de generar una sola cadena de razonamiento, el modelo:

* Produce **varias alternativas de pensamiento** en cada paso,
* Evalúa la calidad o viabilidad de cada alternativa,
* Descarta ramas poco prometedoras,
* Continúa explorando las ramas más relevantes hasta alcanzar una solución final.

Este enfoque resulta especialmente eficaz en **problemas complejos**, donde la exploración, la planificación y la evaluación intermedia son fundamentales.

#### Diferencias con Chain of Thought

| Chain of Thought                    | Tree of Thoughts                  |
| ----------------------------------- | --------------------------------- |
| Razonamiento lineal                 | Razonamiento ramificado           |
| Una única secuencia                 | Múltiples caminos posibles        |
| Sin evaluación intermedia explícita | Evaluación y poda de ramas        |
| Adecuado para problemas moderados   | Adecuado para problemas complejos |

[Árbol de pensamientos](ejemplosprompts.md#1-tree-of-thoughts)

#### Casos de uso recomendados

* Problemas de lógica y razonamiento abstracto
* Planificación y toma de decisiones
* Juegos, puzzles y búsqueda de estrategias
* Tareas donde existen múltiples soluciones posibles

#### Ventajas

* Fomenta un razonamiento más deliberado y profundo
* Reduce la probabilidad de soluciones apresuradas
* Mejora la calidad en tareas que requieren exploración

#### Limitaciones

* Incrementa el coste computacional
* No siempre es necesario para tareas simples

---

### 8.6 Visualization of Thoughts (VoT)

La **Visualization of Thoughts (VoT)** es una técnica emergente que propone inducir al modelo a **representar su razonamiento de forma visual o espacial**, como diagramas mentales, mapas conceptuales o estructuras gráficas, con el objetivo de mejorar su capacidad de razonamiento en determinados dominios.

#### Idea principal

El modelo no solo explica sus pasos, sino que:

* Organiza el razonamiento como si fuera un **esquema visual**,
* Usa estructuras espaciales (listas jerárquicas, grafos, mapas),
* Simula la construcción de un “mapa mental” del problema.

Esta técnica ha mostrado resultados prometedores en tareas de **razonamiento espacial**, navegación, planificación y comprensión estructural.

[Visualización de pensamientos](ejemplosprompts.md#1-visualization-of-thoughts)

#### Casos de uso potenciales

* Razonamiento espacial o geométrico
* Análisis de sistemas complejos
* Problemas que se benefician de esquemas o mapas
* Apoyo al razonamiento multimodal

#### Estado actual de la técnica

**Técnica experimental**

* No está aún consolidada como estándar en ingeniería de prompts
* Procede principalmente de investigación académica reciente
* Se considera una **línea emergente**, más que una práctica establecida

#### Recomendación didáctica

Esta técnica es adecuada para:

* Introducir tendencias actuales de investigación
* Mostrar los límites y evolución de la ingeniería de prompts
* Contextos avanzados o exploratorios

No se recomienda como técnica básica o generalista.

---

## 9. Especificación del formato de salida

Los prompts pueden indicar explícitamente el **formato de la respuesta**, como:

- Texto plano
- Listas y viñetas
- Tablas
- Código fuente
- Resúmenes
- Traducciones
- Formatos estructurados (CSV, JSON, etc.)

[Especificar el formato de salida](ejemplosprompts.md#1-especificar-el-formato-de-salida)

---

## 10. Reflexión final

La ingeniería de prompts no consiste únicamente en “hacer buenas preguntas”, sino en **comprender cómo interactúan los modelos de lenguaje con el texto de entrada**.

Dominar esta disciplina permite:    
- mejorar la calidad de las respuestas,  
- reducir errores y alucinaciones,  
- aprovechar de forma crítica y responsable el potencial de los LLMs.  

Este conocimiento es clave para el uso profesional y académico de herramientas como ChatGPT.

[Ejemplos prácticos](ejemplosparaprobar.md) 

[Actividad 1](actividad1.md)
