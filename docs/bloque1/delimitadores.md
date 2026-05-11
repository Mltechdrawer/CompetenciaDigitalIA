## Delimitadores en los prompts

### ¿Qué son los delimitadores?

Los **delimitadores** son **símbolos o marcas especiales** que se utilizan en un prompt para **separar y señalar claramente distintas partes del texto**, como instrucciones, contexto o datos de entrada.

Su objetivo es ayudar al modelo a **entender qué información cumple cada papel** dentro del prompt.

En términos simples:

> **Un delimitador indica dónde empieza y dónde termina una parte concreta del prompt.**

---

### ¿Por qué son importantes?

Sin delimitadores, un modelo de lenguaje puede: 

- Confundir instrucciones con datos.  
- Mezclar el texto a procesar con la orden principal.  
- Interpretar mal qué información es relevante.  

El uso de delimitadores permite: 

- Mejorar la comprensión del prompt.  
- Aumentar la precisión de las respuestas.  
- Reducir ambigüedades.  
- Hacer los prompts más claros y reutilizables.  

---

### Tipos comunes de delimitadores

No existe un único delimitador obligatorio. Algunos de los más habituales son:

#### Comillas triples

"""
Texto delimitado
"""

#### Bloques de código
```
Texto delimitado
```

#### Etiquetas explícitas
```
<texto>
Contenido delimitado
</texto>
```

#### Guiones
```
--- Contenido delimitado ---
```

#### Tags
```
<Contenido delimitado> 
```

#### Igual
```
=== Contenido delimitado === 
```

#### Marcadores personalizados
```
### INSTRUCCIÓN ###
### CONTEXTO ###
### TEXTO ###
```

---

### Ejemplo práctico

#### Sin delimitadores

```
Resume el siguiente texto El aprendizaje automático es una rama de la inteligencia artificial que...
```

El modelo puede no identificar claramente dónde empieza el texto a resumir.

#### Con delimitadores

```
Resume el siguiente texto:

""" El aprendizaje automático es una rama de la inteligencia artificial que... """
```

Ahora el modelo entiende con claridad **qué contenido debe procesar**.

---

### Delimitadores y seguridad

Los delimitadores también ayudan a: 

- Aislar datos externos de las instrucciones principales.  
- Reducir riesgos de *prompt injection*.  
- Evitar que instrucciones ocultas dentro de un texto influyan en el modelo.  

Esto es especialmente importante cuando el texto proviene de usuarios o fuentes externas.

---

### Buenas prácticas

- Usa delimitadores de forma consistente.
- No mezcles muchos tipos diferentes sin necesidad.
- Elige delimitadores visualmente claros.
- Indica explícitamente qué contiene cada bloque si es relevante.

---
<details>
<summary> Ejemplos</summary>
Triples comillas dobles
<pre><code>
Resume el siguiente texto:
""" La ingeniería de software es una disciplina de la informática que se ocupa del diseño, desarrollo y mantenimiento de sistemas de software de alta calidad. """
</code></pre>
Triples comillas simples --- Bloques de código
<pre><code>
Explica qué hace el siguiente código:
``` for i in range(5):
    print(i).
```
</code></pre>
Etiquetas explícitas
<pre><code>
&lt;instruccion&gt;
Explica qué hace el siguiente código.
&lt;/instruccion&gt;
&lt;codigo&gt;
for i in range(3):
    print(i)
&lt;/codigo&gt;
&lt;publico&gt;
Estudiante de primero de universidad
&lt;/publico&gt;
</code></pre>
Guiones
<pre><code>
Resume el siguiente texto:
--- La ingeniería de software es una disciplina de la informática que se ocupa del diseño, desarrollo y mantenimiento de sistemas de software de alta calidad. ---
</code></pre>
Tags
<pre><code>
Resume el siguiente texto:
&lt;La ingeniería de software es una disciplina de la informática que se ocupa del diseño, desarrollo y mantenimiento de sistemas de software de alta calidad.&gt;
</code></pre>
Igual
<pre><code>
Resume el siguiente texto:
=== La ingeniería de software es una disciplina de la informática que se ocupa del diseño, desarrollo y mantenimiento de sistemas de software de alta calidad. ===
</code></pre>
Marcadores personalizados
<pre><code>
Resume el siguiente texto:
### La ingeniería de software es una disciplina de la informática que se ocupa del diseño, desarrollo y mantenimiento de sistemas de software de alta calidad. ###
</code></pre>
</details>
---

### Resumen

- Los delimitadores organizan y estructuran los prompts.
- Ayudan a diferenciar instrucciones y datos.
- Mejoran la precisión y la seguridad.
- Son una herramienta clave en la ingeniería de prompts y de contexto.

---

