# Cómo organizo Obsidian para que funcione como un segundo cerebro, no como otro cajón digital

Durante años hemos vendido la idea del "segundo cerebro" como si bastara con instalar una app, crear unas carpetas bonitas y empezar a guardar enlaces. El problema es que eso no crea pensamiento. Crea inventario.

Un segundo cerebro útil no es el sitio donde guardas todo. Es el sistema que te ayuda a volver a una idea cuando puede mejorar una decisión, un proyecto o una explicación.

Obsidian encaja muy bien en esa forma de trabajar porque no te obliga a pensar en documentos aislados. Te deja construir una red de notas en Markdown, con enlaces, propiedades, aliases, mapas de contenido y consultas. Pero precisamente por eso es fácil pasarse de diseño: demasiadas carpetas, demasiados plugins, demasiados campos, demasiadas etiquetas. Al final el sistema te pide más energía de la que te devuelve.

Mi enfoque es más simple: pocas carpetas, notas conectadas, metadatos mínimos y revisión constante.

## 1. Las carpetas son bandejas, no arquitectura del conocimiento

Una carpeta funciona bien cuando describe el estado de una nota. Por ejemplo:

```txt
0-Inbox
1-Templates
2-Notes
3-Media
```

Eso sí es útil.

- Inbox: capturas rápidas y material sin procesar.
- Templates: plantillas.
- Notes: conocimiento ya integrado.
- Media: PDFs, imágenes, dibujos, audios y archivos externos.

Lo que no funciona tan bien es intentar que las carpetas representen todo el conocimiento. Una idea rara vez pertenece a un único sitio. Una nota sobre aprendizaje puede tocar universidad, carrera profesional, psicología, idiomas y productividad. Si la estructura depende solo de carpetas, el sistema te obliga a elegir una caja. Y muchas ideas buenas viven precisamente entre cajas.

Por eso prefiero que las carpetas sean físicas y que el significado viva en enlaces, propiedades y mapas.

## 2. Los MOCs son mejores que una taxonomía rígida

Un MOC, o Map of Content, es una nota índice. No es una carpeta disfrazada. Es una puerta de entrada a un tema.

Por ejemplo, una nota `Languages` puede enlazar a italiano, inglés, gramática, vocabulario, expresiones, contrastes entre idiomas y recursos. La diferencia es que ese mapa puede tener criterio humano: notas principales, notas relacionadas, temas pendientes, consultas dinámicas y reglas de uso.

Una etiqueta te dice que algo pertenece a un tema. Un MOC te ayuda a navegarlo.

Esta diferencia parece pequeña, pero cambia mucho el sistema. Cuando un tema crece, no necesito reorganizar medio vault. Creo o actualizo un MOC. El conocimiento sigue conectado sin depender de una jerarquía perfecta.

## 3. Las propiedades deben servir para recuperar, no para decorar

Obsidian permite añadir Properties al frontmatter. Bien usadas, son una capa muy potente. Mal usadas, se convierten en burocracia.

Yo usaría un conjunto pequeño:

```yaml
type: note
area:
  - learning
topics:
  - "[[Obsidian]]"
  - "[[PKM]]"
aliases:
status: draft
lang:
  - en
created: 2026-05-31
updated: 2026-05-31
```

Lo importante no es tener muchos campos. Lo importante es que cada campo responda a una pregunta real:

- `type`: qué clase de nota es.
- `area`: en qué área principal vive.
- `topics`: con qué temas conecta.
- `aliases`: cómo puedo encontrarla con otros nombres.
- `status`: si es borrador, activa, estable, privada o archivada.
- `lang`: en qué idioma está escrita.
- `next_action`: qué hay que hacer después, si aplica.

Si un campo no ayuda a buscar, filtrar, revisar o actuar, probablemente sobra.

## 4. Dataview y Bases son capa de revisión, no sustituto del pensamiento

Las consultas son útiles para detectar problemas del sistema:

- notas sin área;
- proyectos sin próxima acción;
- ideas activas;
- tareas abiertas;
- deadlines próximos;
- notas en borrador que necesitan procesado.

Un dashboard con Dataview puede ser muy práctico. Pero hay una trampa: pasar más tiempo perfeccionando el dashboard que pensando en las notas.

La consulta no hace el trabajo intelectual. Solo lo hace visible.

Una buena nota sigue necesitando algo más básico: explicar una idea con tus palabras, conectarla con otras y decidir para qué sirve.

## 5. Tomar notas no es copiar: es procesar

Cuando leo un libro o veo un vídeo, intento evitar copiar párrafos enteros. Para eso ya está la fuente original.

La nota debería obligarme a recuperar y reformular:

1. leo o escucho una idea;
2. cierro la fuente;
3. intento explicarla con mis palabras;
4. si no puedo, vuelvo a la fuente;
5. copio literalmente solo definiciones, citas o frases que merecen conservarse tal cual.

Esto hace que la toma de notas se parezca más a active recall que a coleccionismo digital.

El objetivo no es tener una biblioteca de fragmentos. Es construir una red de ideas entendidas.

## 6. Una nota pequeña puede ser mejor que una nota gigante

Tendemos a crear notas enormes sobre temas generales: `Capitalismo`, `Inteligencia Artificial`, `Productividad`, `Italiano`, `Sistemas Operativos`.

No está mal tener notas grandes si funcionan como mapas. El problema aparece cuando una nota intenta contenerlo todo.

Si una sección empieza a tener vida propia, merece una nota propia. Una nota sobre "efectos del capitalismo en países en desarrollo" puede enlazar con `Capitalismo`, `Economía`, `Historia` y `Política`. No tiene que estar enterrada dentro de una nota madre.

La granularidad correcta no es "una nota por idea" de forma dogmática. La regla práctica es otra: si una idea puede reutilizarse, enlazarse o crecer de forma independiente, dale una nota.

## 7. La revisión semanal mantiene vivo el sistema

Un vault se degrada por acumulación. Capturar es fácil. Procesar es lo que cuesta.

Una revisión semanal mínima puede ser suficiente:

- vaciar Inbox;
- borrar lo que no aporta;
- convertir capturas útiles en notas reales;
- enlazar notas sueltas a MOCs;
- revisar proyectos e ideas activas;
- actualizar próximas acciones;
- detectar notas en borrador que llevan demasiado tiempo abiertas.

Sin revisión, Obsidian se convierte en otro sitio donde esconder pendientes.

## 8. La regla final

Una nota entra bien en el sistema si cumple al menos una de estas funciones:

- aclara una idea;
- conecta ideas;
- sirve como mapa;
- registra algo importante;
- transforma una fuente en conocimiento propio;
- deja una próxima acción clara.

Si no cumple ninguna, quizá no necesita estar en tu segundo cerebro.

## Repositorio público

He preparado un starter kit público con plantillas, ejemplos de MOCs, dashboard, consultas Dataview y una checklist de privacidad para no publicar accidentalmente información personal.

La idea no es copiar un vault entero. Eso sería un error. Un vault real contiene contexto privado, nombres, decisiones, emociones, rutas, archivos y enlaces que no pertenecen a GitHub.

Lo que sí tiene sentido publicar es el sistema: las reglas, las plantillas limpias y los ejemplos genéricos.

Repo: `obsidian-second-brain-starter`

Si trabajas con Obsidian, mi recomendación sería esta: empieza simple. No intentes diseñar el sistema perfecto. Diseña el sistema que te obligue a pensar mejor esta semana.
