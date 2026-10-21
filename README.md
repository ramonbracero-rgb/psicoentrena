# PsicoEntrena v8 · Biblioteca completa de Psicología

Aplicación web progresiva (PWA) instalable, pensada para estudiar los PDF aportados por el usuario. Funciona con datos guardados localmente en el navegador.

## Biblioteca incluida

- **Psicopatología II:** 10 temas.
- **Condicionamiento, Motivación y Emoción:** 12 temas.
- **Fundamentos de Neuropsicología:** 6 temas.
- **Psicología del Lenguaje:** 11 temas.
- **Escuelas Psicoterapéuticas I:** 8 temas.
- **Psicología de los Grupos:** 8 temas.

Incluye **55 temas y 550 tarjetas de recuperación activa** generadas a partir de fragmentos de los PDF cargados, con referencia al archivo/asignatura, tema y página del PDF. Además, mantiene las 24 tarjetas seleccionadas previamente para Psicopatología II · Tema 9. La numeración se ha contrastado con los bloques temáticos detectados en los PDF unidos. En Psicología del Lenguaje, el Tema 4 es comprensión y el Tema 5 es producción del lenguaje. Conviene contrastar títulos y numeración con el aula oficial si hay cambios en la versión del temario.

## Novedades de la versión 8

- Selector de modo oscuro/claro en la barra superior; la preferencia se conserva en el navegador.
- Se corrigió el título duplicado del Tema 5 de Psicología del Lenguaje: **Producción del lenguaje**.
- Se actualizó la caché de la PWA para que la nueva interfaz se cargue al actualizar.

## Modos de aprendizaje

- **Cartas de memoria:** intenta recordar antes de revelar la respuesta y valora si no la recordaste, la recordaste con esfuerzo o la sabías.
- **Repaso inteligente:** limitado a la asignatura seleccionada y, si se elige, al tema seleccionado. Nunca mezcla asignaturas.
- **Asociaciones:** empareja pregunta y explicación dentro de la selección actual.
- **Detective de conceptos:** casos educativos para Psicopatología II · Tema 9 y retos de recuperación construidos con las tarjetas para el resto de las selecciones.
- **Mapa conceptual:** nodos interactivos extraídos de las tarjetas de la asignatura/tema actual.
- **Progresión:** XP, niveles, rachas, insignias, colección y maestría por carta.
- **Datos locales:** progreso guardado en localStorage; exportación e importación JSON.

## Instalar en Samsung

1. Descomprime el ZIP.
2. Publica **todo el contenido de la carpeta `psicoentrena_v3`** en un alojamiento HTTPS (por ejemplo, GitHub Pages).
3. Abre la URL publicada con Chrome en el Samsung.
4. Menú ⋮ → «Instalar aplicación» o «Añadir a pantalla de inicio».
5. Abre PsicoEntrena desde el icono. Después de la primera carga, los archivos de la PWA se almacenan para uso sin conexión.

No abras `index.html` directamente desde el gestor de archivos si quieres que funcionen la instalación PWA y el modo offline; necesita servirse por HTTPS o localhost.

## Importar tarjetas propias

Formato mínimo:

```json
{
  "topic": "Tema 1",
  "cards": [
    {
      "front": "¿Qué concepto debes recordar?",
      "back": "Definición fiel al material de estudio.",
      "zone": "Conceptos básicos",
      "association": "Regla mnemotécnica",
      "source": "Asignatura, Tema 1, p. 5 del PDF",
      "subject": "Nombre de la asignatura",
      "topic": "Tema 1"
    }
  ]
}
```

## Nota de calidad académica

Las 550 tarjetas se prepararon a partir de texto extraído de los PDF y se distribuyeron por los temas identificados. Son un primer banco amplio para jugar y repasar, no una edición manual validada línea por línea: antes de usarlas como única fuente para un examen, revisa las respuestas que te resulten ambiguas contra el PDF original. Las tarjetas mantienen una referencia a la página para facilitar esa comprobación. Los casos son educativos, no herramientas de diagnóstico clínico.
