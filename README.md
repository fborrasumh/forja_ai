# ForjaIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22032189.svg)](https://doi.org/10.5281/zenodo.22032189)

Crea tu app docente con IA, sin programar. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/forja_ai/

**Idiomas:** español (por defecto), inglés y portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

ForjaIA guía al profesorado universitario, en 6 paradas, para convertir una idea de clase en una app web de un único fichero `index.html`, probarla y publicarla en GitHub Pages con DOI de Zenodo.

- **Clave:** se elige el proveedor de IA (OpenAI, Google Gemini o Anthropic Claude) y se pega la clave propia. Al probarla, el desplegable se rellena con los modelos disponibles en esa clave; también se puede escribir otro modelo a mano.
- **Tipo:** cinco tipos de app: generador de documentos, conversación (tutor o personaje simulado), cuestionario autocorregido, tarjetas de estudio y método Feynman.
- **Describe:** el docente cuenta su idea, la asignatura, el público y los límites; la IA propone la especificación (encargo, campos del formulario, textos). Las advertencias del docente que la IA no recoge se añaden por código al encargo.
- **Ajusta:** se revisa el encargo, los campos, el aspecto, las traducciones (español, inglés y portugués), la autoría con ORCID, la licencia y el proveedor y modelo que usará la app, con vista previa en vivo.
- **Prueba:** la app generada funciona dentro de ForjaIA (ordenador, tableta o móvil) con la clave guardada.
- **Publica:** descarga `index.html`, `README.md`, `CITATION.cff` y el proyecto en ZIP, con los pasos guiados de GitHub Pages y Zenodo, la cita y la ficha para el catálogo.

Incluye cinco ejemplos completos que se abren sin clave.

## Cómo se usa la IA

Con la clave propia de OpenAI, Google Gemini o Anthropic Claude; no hace falta servidor. Las apps generadas también permiten elegir cualquiera de los tres proveedores, cada persona con su clave.

## Privacidad

Todo funciona en el navegador. Las claves y los proyectos se guardan solo en el almacenamiento local del navegador; la clave solo se envía al proveedor elegido. Una política de seguridad de contenidos (CSP) impide que la página se conecte con otros servicios. El `index.html` que se descarga no contiene ninguna clave. No introduzcas datos personales de estudiantes.

## Límites

- La especificación y los textos los propone un modelo de lenguaje: revisa siempre el encargo, los campos y las traducciones antes de publicar.
- Las apps generadas no verifican por código las respuestas de la IA (casos, preguntas, tarjetas): el docente debe revisarlas y avisar a su alumnado.
- Se ha probado con respuestas de IA simuladas de los tres proveedores; el comportamiento con cada modelo real puede variar.
- La publicación en GitHub y Zenodo es guiada, pero la hace la propia persona en su cuenta.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche). ORCID: [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

Borrás Rocher, F. (2026). *ForjaIA* (v1.1.0) [Software]. Zenodo. https://doi.org/10.5281/zenodo.22032189

## Licencia

MIT. Véase [LICENSE](LICENSE).
