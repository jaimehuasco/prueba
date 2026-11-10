# Actividades preparatorias para una revisión de alcance

Nov 8, 2026 · @JH

Antes de redactar una revisión de alcance (scoping review), el estudiante prepara el terreno en tres pasos: construye fórmulas de búsqueda, ajusta su tema con abstracts reales y comprueba que nadie haya hecho ya la misma revisión.

Toda la guía sigue un mismo caso del campo de la educación: **la retroalimentación con IA (inteligencia artificial) en la escritura académica de estudiantes universitarios.**

![Esquema de los tres pasos](esquema-pasos.png)

Los pasos 1 y 2 se trabajan con IA (inteligencia artificial); el paso 3, solo en bases y registros. Siglas del esquema: PCC (Población, Concepto, Contexto), ERIC (Education Resources Information Center), SciELO (Scientific Electronic Library Online), OSF (Open Science Framework) y JBI (Joanna Briggs Institute).

## Paso 1. Construir fórmulas de búsqueda con IA

El estudiante entrega su tema provisional a una IA (inteligencia artificial) y obtiene fórmulas booleanas en tres niveles, de lo simple a lo complejo, adaptadas a cada base.

**Tema provisional del caso:** retroalimentación con IA (inteligencia artificial) en la escritura académica de estudiantes universitarios.

| Elemento PCC (Población, Concepto, Contexto) | Contenido en el caso |
| --- | --- |
| Población | Estudiantes universitarios de pregrado |
| Concepto | Retroalimentación generada por IA (inteligencia artificial) a textos escritos |
| Contexto | Cursos de escritura académica en educación superior |

### Prompt modelo

```markdown
Actúa como especialista en revisiones de alcance (scoping reviews) en educación.
Mi tema provisional es: "Retroalimentación con inteligencia artificial en la escritura académica de estudiantes universitarios".
1. Desglosa el tema según el marco PCC (Población, Concepto, Contexto).
2. Para cada elemento, propón sinónimos en inglés, español y portugués.
3. Genera fórmulas booleanas en tres niveles: nivel 1 simple, nivel 2 con sinónimos, nivel 3 completo con campos, truncamiento, filtros y NOT.
4. Adapta el nivel 3 a la sintaxis de Scopus, ERIC, SciELO y Dialnet.
5. Explica en una línea qué cambia de un nivel a otro.
```

### Fórmulas graduales en Scopus

**Nivel 3 · completo.** Incorpora la población, el truncamiento, la exclusión con NOT y los filtros de año, tipo y lengua.

```
TITLE-ABS-KEY ( ( "artificial intelligence" OR "generative AI" OR "large language model*" OR chatgpt OR "automated writing evaluation" )
AND ( feedback OR "formative assessment" OR revision* )
AND ( "academic writing" OR "writing skill*" OR essay* OR "L2 writing" )
AND ( universit* OR undergraduate* OR "higher education" OR college ) )
AND NOT TITLE-ABS-KEY ( "secondary school" OR "primary school" )
AND PUBYEAR > 2017
AND ( LIMIT-TO ( DOCTYPE , "ar" ) )
AND ( LIMIT-TO ( LANGUAGE , "English" ) OR LIMIT-TO ( LANGUAGE , "Spanish" ) )
```

### El nivel 3 en las otras bases

**ERIC (Education Resources Information Center).** 
```
(descriptor:"Artificial Intelligence" OR "generative AI" OR ChatGPT OR "automated writing evaluation")
AND (descriptor:"Feedback (Response)" OR "automated feedback")
AND (descriptor:"Writing Instruction" OR descriptor:"Writing Evaluation" OR "academic writing")
AND descriptor:"Higher Education"
```

**SciELO (Scientific Electronic Library Online).** 
```
("inteligencia artificial" OR "inteligência artificial" OR "artificial intelligence" OR ChatGPT)
AND (retroalimentación OR feedback OR "evaluación formativa")
AND ("escritura académica" OR "redacción académica" OR "escrita acadêmica" OR "academic writing")
AND (universit$ OR "educación superior" OR "ensino superior")
```

**Dialnet.** Su buscador admite poca sintaxis booleana; funciona mejor con dos o tres búsquedas cortas entre comillas y los filtros de la búsqueda avanzada (artículos de revista, materia Educación, años).
```
"inteligencia artificial" "escritura académica" retroalimentación
"ChatGPT" "redacción académica" universitarios
```

### Cómo leer los resultados

| Resultados de la fórmula | Decisión |
| --- | --- |
| Más de 2000 | Subir de nivel: más campos, filtros o NOT |
| Entre 100 y 2000 | Fórmula adecuada para explorar el tema |
| Menos de 30 | Bajar de nivel o sumar sinónimos con OR |

La IA (inteligencia artificial) propone la sintaxis, pero el estudiante la prueba en cada base y corrige los errores que la plataforma señale.

## Paso 2. Perfilar el tema con los abstracts

El estudiante pega al menos 10 abstracts en la misma conversación del paso 1, y la IA (inteligencia artificial) ajusta el tema a lo que la literatura realmente estudia.

### Antes de pegar

1. Elige abstracts de las cuatro bases, no solo de Scopus.
2. Numera cada abstract y agrega su referencia en formato APA (American Psychological Association).
3. Pega solo el resumen, sin el artículo completo.

### Prompt modelo

```markdown
Te comparto 10 abstracts numerados que obtuve con las fórmulas anteriores.
A partir de ellos:
1. Identifica la población, el concepto y el contexto que más se repiten.
2. Señala los términos clave que no estaban en mis fórmulas.
3. Detecta qué aspectos casi no se estudian.
4. Propón una versión ajustada de mi tema y de su PCC (Población, Concepto, Contexto).
5. Indica el número del abstract que respalda cada afirmación.
No agregues información que no esté en los abstracts.

[Abstract 1] Referencia APA + resumen
[Abstract 2] ...
```

La instrucción 5 permite que el estudiante compruebe cada afirmación de la IA (inteligencia artificial) en el abstract correspondiente.

### Ejemplo de respuesta (ilustrativo)

Supongamos que la IA (inteligencia artificial) devuelve estos hallazgos sobre los 10 abstracts del caso:

- La mayoría estudia ChatGPT y sistemas AWE (automated writing evaluation, evaluación automatizada de la escritura) con estudiantes de inglés como lengua extranjera.
- Predominan las encuestas de percepción; pocos estudios observan si el estudiante corrige su texto después de la retroalimentación.
- Casi no hay estudios en español ni en universidades latinoamericanas.
- Términos nuevos para las fórmulas: *feedback uptake*, *AI-generated feedback*, *revision behavior*.

### Tema antes y después

|  | Tema provisional | Tema ajustado |
| --- | --- | --- |
| Enunciado | Retroalimentación con IA en la escritura académica de universitarios | Retroalimentación generada por IA y revisión de textos académicos en estudiantes universitarios: mapa de la evidencia 2018-2025 |
| Población | Estudiantes universitarios | Estudiantes universitarios de pregrado, en lengua materna o extranjera |
| Concepto | Retroalimentación con IA | Retroalimentación generada por IA y su incorporación en la revisión del texto |
| Contexto | Escritura académica | Cursos de escritura académica en educación superior |

Con el tema ajustado, el estudiante vuelve al paso 1 y agrega los términos nuevos al nivel 3 de sus fórmulas.

## Paso 3. Verificar el carácter inédito

El tema es inédito si no existe una revisión publicada ni un protocolo registrado con el mismo PCC (Población, Concepto, Contexto). Este paso se hace directamente en las bases y registros, no con la IA, porque puede inventar revisiones.

### Método recomendado: verificación doble

1. **OSF Registries (Open Science Framework Registries).** Es la fuente más confiable para revisiones en curso, porque allí se registran los protocolos de scoping reviews antes de su publicación. Busca en [osf.io/registries](https://osf.io/registries) con dos o tres combinaciones cortas en inglés y español.
2. **Scopus.** Localiza las revisiones ya publicadas. Une la fórmula del tema ajustado con los tipos de revisión en el campo del título.
3. **Complemento.** Revisa JBI (Joanna Briggs Institute) Evidence Synthesis y Campbell Systematic Reviews, dos revistas especializadas en síntesis de evidencia; Campbell cubre educación.

PROSPERO (International Prospective Register of Systematic Reviews), el registro más conocido, no sirve para este caso: no acepta scoping reviews y se centra en salud.

### Búsquedas del caso

**OSF Registries (Open Science Framework Registries):**

```
scoping review AI feedback writing
systematic review ChatGPT academic writing feedback
revisión retroalimentación inteligencia artificial escritura
```

**Scopus:** el filtro por título es más preciso que el filtro de tipo de documento, porque muchas scoping reviews figuran como artículos.

```
TITLE ( "scoping review" OR "systematic review" OR "literature review" OR "mapping review" OR "meta-analys*" )
AND TITLE-ABS-KEY ( ( "artificial intelligence" OR "generative AI" OR chatgpt OR "automated writing evaluation" )
AND ( feedback OR "feedback uptake" OR revision* )
AND ( writing OR essay* ) )
AND PUBYEAR > 2020
```

El límite desde 2021 sirve para este tema porque la IA (inteligencia artificial) generativa cambió el campo desde 2022; en otros temas conviene revisar los últimos cinco años.

### Cómo decidir (ejemplo ilustrativo)

El estudiante lee el título y el abstract de cada revisión hallada y compara su PCC (Población, Concepto, Contexto) con el propio.

| Hallazgo | Decisión |
| --- | --- |
| Scoping review reciente con el mismo PCC | No es inédito: cambiar población, concepto o contexto |
| Revisión sistemática sobre percepciones de estudiantes de inglés como lengua extranjera | Inédito con justificación: el caso estudia la revisión del texto, no las percepciones |
| Protocolo en OSF Registries (Open Science Framework Registries) aún sin publicar | Leer el protocolo y ajustar el tema para no duplicarlo |
| Revisión con el mismo PCC de hace más de cinco años | Inédito como actualización, sobre todo si el campo cambió |
| Ningún resultado coincidente | Inédito: guardar capturas de las búsquedas con fecha |

Las capturas con fecha y el número de resultados sirven como evidencia del carácter inédito en la introducción de la revisión.

## Lista de cotejo del estudiante

Marca cada tarea al completarla; las tres actividades están listas cuando todas las casillas tienen marca.

- [ ] Desglosé mi tema provisional según el PCC (Población, Concepto, Contexto).
- [ ] Obtuve fórmulas de nivel 1, 2 y 3, y anoté el número de resultados de cada una.
- [ ] Probé el nivel 3 en Scopus, ERIC (Education Resources Information Center), SciELO (Scientific Electronic Library Online) y Dialnet.
- [ ] Seleccioné al menos 10 abstracts numerados y con referencia APA (American Psychological Association).
- [ ] Comparé cada afirmación de la IA (inteligencia artificial) con el abstract que la respalda.
- [ ] Redacté el tema ajustado y actualicé mis fórmulas con los términos nuevos.
- [ ] Busqué protocolos en OSF Registries (Open Science Framework Registries).
- [ ] Busqué revisiones publicadas en Scopus con el filtro por título.
- [ ] Guardé capturas con fecha de las búsquedas de verificación.
- [ ] Justifiqué por escrito el carácter inédito de mi tema.
