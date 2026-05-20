# Sesión 3 – Búsqueda, síntesis y validación de información con IA

# Introducción

Durante los primeros años de popularización de la inteligencia artificial generativa, gran parte de la atención se centró en aprender a escribir buenos prompts. Se hablaba constantemente de “ingeniería de prompts”, de técnicas avanzadas para formular instrucciones y de estrategias para conseguir mejores respuestas de los modelos.

Sin embargo, el ecosistema actual está cambiando rápidamente. Los sistemas de IA ya no se limitan únicamente a responder preguntas o generar texto. Cada vez son más capaces de utilizar herramientas externas, recordar contexto, dividir problemas complejos en tareas más pequeñas, buscar información, ejecutar acciones e incluso colaborar con usuarios humanos durante procesos completos de trabajo.

La IA generativa está evolucionando desde simples chatbots hacia asistentes y agentes capaces de participar activamente en tareas reales.

Esta transformación no elimina la necesidad del ser humano. Al contrario: cambia el papel que desempeñamos. Ya no basta con escribir instrucciones. Ahora debemos supervisar, validar, coordinar y comprender cómo funcionan estos sistemas.

---

# 1. De los primeros prompts a la IA actual

## 1.1. La primera etapa de la IA generativa

Cuando aparecieron los primeros modelos conversacionales accesibles al público, la interacción era relativamente sencilla. El usuario escribía una pregunta y el sistema generaba una respuesta.

Por ejemplo:

- “Resume este texto.”
- “Explícame qué es una base de datos.”
- “Genera un correo formal.”
- “Escribe código en Python.”

En esta etapa: 

- el usuario dirigía completamente la conversación;  
- la IA no tenía memoria persistente;  
- no podía acceder a herramientas externas;  
- y su comportamiento dependía enormemente de cómo estuviese redactado el prompt.  

La calidad de las respuestas variaba mucho dependiendo de la habilidad del usuario para formular instrucciones.

---

## 1.2. La explosión de la ingeniería de prompts

A medida que los modelos mejoraron, surgió una disciplina informal conocida como *prompt engineering* o ingeniería de prompts.

El objetivo era aprender a comunicarse mejor con los modelos.

Comenzaron a popularizarse técnicas como:

### Zero-shot prompting
Consiste en pedir directamente una tarea sin proporcionar ejemplos previos.

Ejemplo:
> “Clasifica este comentario como positivo o negativo.”

---

### Few-shot prompting
Se proporcionan varios ejemplos antes de solicitar la tarea.

Ejemplo:

Comentario: “Me encantó el servicio.” → Positivo  
Comentario: “La aplicación falla constantemente.” → Negativo  

Ahora clasifica:
> “La interfaz es lenta pero útil.”

---

### Chain of Thought

Consiste en pedir al modelo que razone paso a paso antes de responder.

Ejemplo:
> “Resuelve el problema razonando paso a paso.”

Esta técnica mejoró enormemente el comportamiento de los modelos en tareas complejas.

---

## 1.3. ¿Qué está ocurriendo ahora?

Actualmente, muchos modelos:  
- razonan mejor;  
- necesitan menos instrucciones complejas;  
- mantienen contexto durante conversaciones largas;  
- utilizan memoria;  
- interactúan con herramientas externas;  
- ejecutan tareas en varios pasos;  
- y generan distintos tipos de contenido simultáneamente.  

La consecuencia es importante:

> La ingeniería de prompts no ha desaparecido, pero ya no ocupa el mismo lugar que hace dos años.

Antes, gran parte del esfuerzo estaba en “descubrir cómo hablarle al modelo”.  
Ahora, cada vez más esfuerzo se dedica a:  
- diseñar procesos;  
- supervisar resultados;  
- validar información;  
- coordinar herramientas;  
- y automatizar tareas completas.  

---

# 2. Del chatbot al agente inteligente

## 2.1. ¿Qué es un chatbot?

Un chatbot tradicional:  
- responde preguntas;  
- mantiene una conversación;  
- genera contenido;  
- pero normalmente no actúa fuera del entorno conversacional.  

Por ejemplo:  
- redacta textos;  
- responde dudas;  
- genera resúmenes;  
- traduce contenido.  

Su función principal es producir respuestas.

---

## 2.2. ¿Qué es un agente de IA?

Un agente de IA va más allá de la conversación.

Un agente:  
- puede planificar tareas;  
- dividir problemas complejos;  
- utilizar herramientas externas;  
- consultar información;  
- ejecutar acciones;  
- evaluar resultados;  
- y continuar trabajando hasta alcanzar un objetivo.  

En lugar de responder únicamente a preguntas, intenta completar tareas.

---

## 2.3. Diferencias principales

| Chatbot tradicional | Agente de IA |
|---|---|
| Conversa | Ejecuta tareas |
| Responde preguntas | Persigue objetivos |
| Genera texto | Utiliza herramientas |
| Depende continuamente del usuario | Puede actuar parcialmente de forma autónoma |
| Sesiones aisladas | Mantiene contexto y memoria |

---

## 2.4. Ejemplos actuales

Hoy existen asistentes capaces de:  
- buscar información en Internet;  
- resumir documentos extensos;  
- generar presentaciones;  
- programar aplicaciones;  
- analizar datos;  
- consultar bases de datos;  
- crear imágenes;  
- automatizar tareas repetitivas;  
- organizar información;  
- y colaborar con usuarios humanos.  

Muchas plataformas actuales integran ya capacidades de agente.

Entre ellas:
- OpenAI  
- Google  
- Microsoft  
- Anthropic  

---

# 3. Cómo funciona un agente de IA

Aunque los sistemas reales son muy complejos, podemos simplificar su arquitectura en cuatro grandes componentes.

---

## 3.1. El modelo de lenguaje

Es el núcleo del sistema.

El modelo:  
- interpreta instrucciones;  
- genera respuestas;  
- razona;  
- produce texto, código o contenido multimodal.  

Es la parte “inteligente” del sistema.  

---

## 3.2. La memoria

Permite recordar:
- contexto;   
- preferencias;  
- conversaciones anteriores;  
- información relevante.  

Sin memoria, cada interacción comenzaría desde cero.

---

## 3.3. Las herramientas

Muchos agentes pueden utilizar herramientas externas:  
- navegadores web;  
- bases de datos;  
- calculadoras;  
- sistemas de archivos;  
- APIs;  
- generadores de imágenes;  
- hojas de cálculo;  
- editores de código.  

Aquí aparece uno de los mayores cambios respecto a los primeros chatbots.

La IA ya no solo “habla”.  
Ahora también “opera”.

---

## 3.4. El sistema de planificación

Un agente puede dividir un problema complejo en tareas más pequeñas.

Por ejemplo:

Objetivo:
> “Prepara un informe sobre energías renovables.”

Posible proceso:  
1. Buscar información.  
2. Seleccionar fuentes fiables.  
3. Extraer datos.  
4. Resumir contenidos.  
5. Crear gráficos.  
6. Redactar conclusiones.  
7. Generar el documento final.  

Esto se aproxima más al comportamiento de un asistente digital que al de un simple chatbot.

---

# 4. Búsqueda, síntesis y validación de información con IA

## 4.1. La transformación de la búsqueda de información

Durante décadas, la búsqueda de información en Internet se basó principalmente en motores de búsqueda tradicionales. El usuario introducía palabras clave y obtenía una lista de enlaces que debía revisar manualmente.

La llegada de la IA generativa ha comenzado a transformar este modelo.

Actualmente, muchos sistemas permiten:  
- realizar preguntas en lenguaje natural;  
- obtener respuestas sintetizadas;  
- resumir múltiples fuentes;  
- comparar información;  
- y recibir explicaciones adaptadas al contexto del usuario.  

Esto cambia profundamente la experiencia de búsqueda.

Antes:
- el usuario buscaba enlaces.

Ahora:
- el usuario recibe directamente una interpretación de la información.

---

## 4.2. La IA como herramienta de síntesis

Una de las capacidades más potentes de la IA generativa es la síntesis automática de información.

Los modelos actuales pueden:  
- resumir artículos científicos;  
- comparar documentos;  
- extraer ideas principales;  
- simplificar lenguaje técnico;  
- reorganizar contenido complejo;  
- generar conclusiones preliminares;  
- y producir explicaciones adaptadas a distintos niveles de conocimiento.  

Por ejemplo, un estudiante puede solicitar:
> “Resume este artículo científico en cinco ideas clave.”

O también:
> “Explícame este documento como si fuera para alumnado de secundaria.”

La IA permite reducir enormemente el tiempo necesario para procesar grandes volúmenes de información.

Sin embargo, esta ventaja también introduce riesgos importantes.

---

## 4.3. El problema de la fiabilidad

La IA generativa no “comprende” la información como un ser humano. Los modelos generan respuestas probabilísticas a partir de patrones aprendidos durante el entrenamiento.

Como consecuencia:  
- pueden mezclar información correcta e incorrecta;  
- inventar referencias;  
- generar datos falsos;  
- producir citas inexistentes;  
- o crear explicaciones aparentemente convincentes pero erróneas.  

Este fenómeno se conoce como alucinación.

Uno de los mayores riesgos de la IA generativa es precisamente su capacidad para producir respuestas falsas con gran apariencia de credibilidad.

Por ello, utilizar IA correctamente implica desarrollar una actitud crítica permanente.

---

## 4.4. Estrategias de validación de información

La validación de información se convierte en una competencia fundamental en la era de la IA.

No basta con obtener respuestas rápidas. También es necesario verificar su calidad y fiabilidad.

Algunas estrategias importantes son:

### Contrastar múltiples fuentes
Nunca depender de una única respuesta generada por IA.

---

### Revisar las fuentes originales
Siempre que sea posible:
- consultar artículos originales;  
- verificar enlaces;  
- comprobar autores;  
- y revisar publicaciones oficiales.  

---

### Comprobar fechas y contexto
La información puede estar desactualizada o fuera de contexto.

---

### Verificar datos numéricos
Los modelos pueden cometer errores matemáticos o estadísticos.

---

### Detectar exceso de seguridad
Las respuestas muy seguras no siempre son correctas.

Una IA puede afirmar algo incorrecto con total convicción.

---

### Mantener pensamiento crítico
La IA debe funcionar como apoyo al razonamiento humano, no como sustituto del criterio personal.

---

## 4.5. Nuevas competencias digitales

La expansión de la IA está modificando profundamente las competencias digitales necesarias en la sociedad actual.

Durante muchos años, una habilidad fundamental consistía en:
> “Saber buscar información.”

Hoy, además de buscar, necesitamos:  
- interpretar;  
- validar;  
- contrastar;  
- supervisar;  
- y evaluar información generada automáticamente.  

La competencia digital moderna ya no consiste únicamente en acceder a la información, sino también en determinar si dicha información es fiable.

---

# 5. Automatización cognitiva y trabajo aumentado

## 5.1. ¿Qué significa automatizar tareas cognitivas?

Tradicionalmente, las máquinas automatizaban tareas físicas:  
- mover objetos;  
- fabricar piezas;  
- transportar mercancías.  

La IA actual automatiza tareas intelectuales:
- redactar;  
- clasificar;  
- resumir;  
- programar;  
- analizar;  
- buscar información;  
- generar ideas;  
- traducir;  
- organizar contenido.  

Esto se conoce frecuentemente como automatización cognitiva.

---

## 5.2. El concepto de trabajo aumentado

La IA no siempre sustituye completamente al ser humano.

En muchos casos:  
- amplifica capacidades;  
- acelera procesos;  
- reduce tareas repetitivas;  
- y mejora la productividad.  

El profesional humano sigue siendo fundamental para:
- supervisar;  
- validar;  
- interpretar;  
- tomar decisiones;  
- y asumir responsabilidad.  

---

## 5.3. Cambios en el perfil profesional

En numerosos sectores, el trabajo está cambiando rápidamente.

Por ejemplo:  
- programadores que utilizan copilotos de código;  
- investigadores que resumen artículos automáticamente;  
- docentes que generan materiales educativos;  
- periodistas que automatizan borradores;  
- diseñadores que utilizan generación de imágenes;  
- analistas que procesan datos mediante IA.  

El profesional deja de ser únicamente “productor de contenido” para convertirse también en:  
- supervisor;  
- coordinador;  
- evaluador;  
- diseñador de procesos;  
- y verificador de resultados.  

---

# 6. Riesgos y limitaciones

## 6.1. Alucinaciones

Los modelos pueden generar información falsa con apariencia convincente.

Este fenómeno recibe el nombre de alucinación.

La IA puede:  
- inventar referencias;  
- generar datos incorrectos;  
- producir explicaciones erróneas;  
- o afirmar información inexistente.  

Por ello, nunca debe asumirse automáticamente que una respuesta es correcta.

---

## 6.2. Sesgos

Los modelos aprenden a partir de grandes volúmenes de información humana.

Como consecuencia:  
- pueden reproducir prejuicios;  
- estereotipos;  
- sesgos culturales;  
- o desigualdades existentes en los datos.  

---

## 6.3. Dependencia tecnológica

Un uso excesivamente pasivo de la IA puede provocar:  
- pérdida de pensamiento crítico;  
- dependencia de herramientas;  
- reducción del esfuerzo cognitivo;  
- y dificultades para validar información.  

---

## 6.4. Supervisión humana

La supervisión humana sigue siendo imprescindible.

La IA puede ayudar enormemente, pero:  
- no comprende el mundo como un ser humano;  
- no posee responsabilidad legal;  
- no tiene criterio ético propio;  
- y puede cometer errores graves.  

Por ello:

> Utilizar IA de forma competente implica saber cuándo confiar… y cuándo no hacerlo.

---

# 8. Conclusiones

La inteligencia artificial generativa está evolucionando rápidamente.

En pocos años hemos pasado:  
- de simples sistemas conversacionales;  
- a asistentes capaces de utilizar herramientas;  
- planificar tareas;  
- generar contenido multimodal;  
- y colaborar activamente con usuarios humanos.  

Este cambio transforma nuestra forma de trabajar y de acceder al conocimiento.

La IA permite:  
- buscar información;  
- sintetizar documentos;  
- acelerar procesos;  
- y automatizar tareas cognitivas.  

Sin embargo, también introduce nuevos desafíos relacionados con:
- la fiabilidad;  
- la validación;  
- los sesgos;  
- y la dependencia tecnológica.  

La cuestión ya no es únicamente:
> “¿Cómo escribir buenos prompts?”

Ahora también debemos preguntarnos:  
- cómo validar respuestas generadas automáticamente;  
- cómo supervisar sistemas complejos;  
- cómo automatizar procesos correctamente;  
- y cómo mantener el pensamiento crítico en entornos altamente automatizados.  

La competencia digital moderna ya no consiste solamente en usar herramientas.    
Consiste en comprenderlas críticamente.  

---
**Resultados de aprendizaje:** RA02, RA05  
**Competencias:** CG02, CG04, CG05, CE02, CE05

<details>
<summary><strong>Resultados de aprendizaje</strong></summary>

<strong>RA02</strong> Seleccionar y utilizar herramientas digitales y sistemas de inteligencia artificial, incluida la IA generativa, para tareas académicas y profesionales. </p>

<p>Adquirir este resultado de aprendizaje es parecido a aprender a elegir correctamente las herramientas de un taller especializado. No todas las aplicaciones sirven para cualquier tarea, y utilizar una herramienta inadecuada puede generar resultados poco útiles o poco fiables. La competencia digital implica saber analizar qué sistema resulta más adecuado según el problema, el contexto y los objetivos perseguidos.</p>


<strong>RA05</strong> Aplicar soluciones digitales y de inteligencia artificial para mejorar procesos de aprendizaje, investigación o trabajo.</p> 

<p>Alcanzar este resultado supone entender que la IA no es únicamente una herramienta para generar respuestas rápidas, sino una tecnología capaz de integrarse en procesos más amplios de análisis, organización, automatización y apoyo a la toma de decisiones. La verdadera utilidad de estas herramientas aparece cuando ayudan a trabajar de manera más eficiente, estructurada y reflexiva.</p>

</details>

<details>
<summary><strong>Competencias</strong></summary>

<p><strong>CG02</strong> Identificar y seleccionar herramientas digitales y sistemas de inteligencia artificial adecuados a distintos contextos académicos y profesionales, atendiendo a criterios de utilidad, fiabilidad y pertinencia. </p>

<p>Desarrollar esta competencia es similar a convertirse en el responsable de una caja de herramientas inteligente: no se trata de usar cualquier aplicación, sino de comprender qué solución encaja mejor en cada situación y qué limitaciones presenta cada sistema.</p>


<p><strong>CG04</strong> Utilizar de forma eficaz herramientas digitales y de inteligencia artificial para la búsqueda, análisis, gestión y producción de información y contenidos digitales.</p> 

<p>Esta competencia permite transformar la tecnología en una herramienta real de productividad y apoyo al trabajo intelectual. La IA puede acelerar procesos y ampliar capacidades humanas, pero únicamente cuando se utiliza de forma organizada y crítica.</p>


<p><strong>CG05</strong> Integrar soluciones digitales y basadas en inteligencia artificial para la mejora y optimización de procesos de aprendizaje, investigación o trabajo, adoptando una perspectiva reflexiva y orientada a la mejora continua. </p>

<p>Adquirir esta competencia es como aprender a diseñar sistemas de trabajo más inteligentes. La IA deja de ser una herramienta aislada y pasa a convertirse en parte de procesos estructurados capaces de mejorar la organización, el análisis de información y la toma de decisiones.</p>


<p><strong>CE02</strong> Utilizar de forma aplicada herramientas digitales y sistemas de inteligencia artificial, incluida la IA generativa, para la búsqueda, análisis y producción de información en contextos académicos y profesionales. </p>

<p>Esta competencia representa el paso desde el conocimiento teórico hacia la aplicación práctica. Igual que aprender a conducir requiere práctica real y no únicamente estudiar normas de circulación, el uso competente de IA exige experimentar, evaluar resultados y desarrollar criterio propio sobre cómo integrar estas tecnologías en situaciones reales.</p>


<p><strong>CE05</strong> Diseñar y justificar una propuesta aplicada de uso de herramientas digitales y de inteligencia artificial orientada a la mejora de procesos de aprendizaje, investigación o trabajo. </p>

<p>Esta competencia supone dar un paso más allá del uso básico de tecnología. Igual que un arquitecto no se limita a conocer materiales, sino que diseña estructuras completas adaptadas a una finalidad concreta, trabajar con IA implica aprender a construir procesos organizados, coherentes y eficientes que integren herramientas digitales de forma estratégica y justificada.</p>

</details>