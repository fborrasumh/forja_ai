# ForjaIA

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22032189.svg)](https://doi.org/10.5281/zenodo.22032189)

De tu idea, cuaderno o Guía Docente a una app docente con IA, probada y citable. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/forja_ai/

**Idiomas:** español (por defecto), inglés y portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

ForjaIA reproduce en el navegador el método de la skill *forja-app-builder*, con el que se han construido las apps Forja del catálogo:

- **Material:** lee entera la idea y los ficheros (cuadernos .ipynb, Word, PDF, PowerPoint, texto), resume la idea en 4-5 líneas y comprueba por código cada cita que la IA dice sacar del material. Retira las claves de API pegadas por error y avisa de que se revoquen.
- **Preguntas:** anuncia lo que da por hecho y hace como mucho tres preguntas, solo de decisiones que cambian la app.
- **Autoría:** autores con nombre, afiliación y ORCID (comprobado con su dígito de control), crédito de la idea original, contribuciones CRediT y conformidad de cada coautor con la licencia MIT, antes de escribir código.
- **Construcción híbrida:** la IA diseña la portada y escribe las pantallas y la lógica; ForjaIA añade el andamiaje Forja ya probado (proveedores OpenAI, Gemini y Claude con selector de modelos, verificación de citas y cifras, enmascarado de datos personales, aviso previo al envío, persistencia, tres idiomas, Word, CSV y ZIP sin red, CSP) y revisa el código: identificadores inexistentes, claves escritas, IA local, promesas no demostrables, clases reservadas y patrones de fiabilidad. Las traducciones que faltan se piden a la IA y el código comprueba huecos y etiquetas.
- **Pruebas:** abre la app generada en una vista previa (escritorio, tableta y móvil, con IA simulada o con la clave propia) y la recorre por código: carga sin errores, una pantalla por paso, ejemplo sin clave y sin llamadas a la IA, traducciones completas, idiomas, detección de una cita y una cifra inventadas, CSP, nombres accesibles, desbordes en móvil, claves y autores. Si hay errores, puede pedir a la IA que los corrija.
- **Publicación guiada:** genera `index.html`, `README.md`, `CITATION.cff`, `LICENSE` y `.zenodo.json` coherentes con los autores; bloquea el paquete si hay claves, texto de plantilla o autores incompletos; da los pasos de GitHub Pages y Zenodo y la ficha para el catálogo.
- **Modo asignatura:** a partir de la Guía Docente, autopsia con cita literal a la guía (ficha, alineación constructiva, carga, evaluación, ambigüedades, accesibilidad y palancas). Los pesos de evaluación, las horas frente a los ECTS, los resultados de aprendizaje sin evaluación y los DOI (en Crossref) los comprueba el código. Propone un único golpe de timón y genera una app de práctica adaptativa por resultados de aprendizaje: diagnóstico inicial, modelo de Elo con olvido, repaso espaciado de errores, intercalado y explicación de por qué toca cada pregunta; funciona sin clave y sin conexión, con analítica de ítems para el profesorado y exportación a Moodle XML, GIFT y CSV. Las preguntas las propone la IA, las valida el código y las revisa el profesorado una a una.

Incluye dos ejemplos completos que funcionan sin clave, en los tres idiomas: una idea y una Guía Docente ficticia.

## Cómo se usa la IA

Con la clave propia de OpenAI, Google Gemini o Anthropic Claude; no hace falta servidor. Para entender el material basta un modelo económico; para escribir el código conviene uno potente. Las apps generadas también funcionan con la clave de cada persona en cualquiera de los tres proveedores. No hay IA local.

## Privacidad

Todo funciona en el navegador. El proyecto y las claves se guardan solo en el almacenamiento local del navegador; la clave solo se envía al proveedor elegido. Antes de enviar algo se enmascaran correos, DNI y teléfonos y se retiran las claves pegadas, y antes del primer envío se muestra lo que sale. Las únicas otras conexiones son voluntarias: comprobar en GitHub si un nombre de repositorio está libre y comprobar DOI en Crossref. Una política de seguridad de contenidos (CSP) impide cualquier otra. ForjaIA no publica nada: los ficheros los sube cada persona a su cuenta. El proyecto exportado no contiene claves.

## Límites

- El código que escribe la IA puede fallar: las pruebas automáticas detectan muchos errores, pero no todos. Hay que revisar la app a mano, con IA simulada y con una clave real, antes de publicar.
- Las pruebas de ForjaIA no sustituyen una auditoría completa de accesibilidad: comprueban nombres accesibles y desbordes, no el contraste ni el teclado de la app generada.
- La autopsia de la guía solo da por buenos los hallazgos con cita literal verificada; los demás se marcan como opinión. Los PDF escaneados no se leen (no hay OCR).
- Las preguntas del modo asignatura las propone la IA: el profesorado debe revisarlas antes de publicar. La app de práctica produce datos, no evidencia publicable por sí sola.
- Se ha probado con respuestas de IA simuladas de los tres proveedores; el comportamiento con cada modelo real puede variar.
- Los proyectos de la versión 1 no se importan en la 2.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche). ORCID: [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

Borrás Rocher, F. (2026). *ForjaIA* (v2.0.0) [Software]. Zenodo. https://doi.org/10.5281/zenodo.22032189

## Licencia

MIT. Véase [LICENSE](LICENSE).
