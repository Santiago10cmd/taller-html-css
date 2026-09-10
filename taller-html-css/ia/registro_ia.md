# Registro de Evidencia de Colaboración con IA

Este documento registra las interacciones significativas con la Inteligencia Artificial durante el diseño, estructuración y desarrollo del sitio web y su sistema de estilos.

---

## Caso 1: Sugerencia aceptada después de verificarla

* **Herramienta:** Gemini (Google)
* **Objetivo:** Garantizar la accesibilidad web en elementos interactivos mediante teclado.
* **Prompt:** "Incluye un estado :focus visible para elementos interactivos asegurando que cumpla con buenas prácticas de accesibilidad."
* **Respuesta obtenida:** La IA sugirió implementar un selector global combinando `a:focus-visible`, `button:focus-visible`, `input:focus-visible` y `textarea:focus-visible` con un contorno personalizado basado en el color de acento (`--color-accent`).
* **Evaluación:** Se verificó que el selector utilizara `:focus-visible` en lugar del genérico `:focus` para evitar que el contorno aparezca al hacer clic con el ratón, mejorando la experiencia visual sin descuidar la navegación por teclado.
* **Decisión:** **Aceptada**, porque cumple directamente con los estándares de accesibilidad WCAG sin sobrecargar el código.
* **Resultado:** Se añadió la regla CSS para el enfoque visible, mejorando la usabilidad para usuarios que navegan con teclado.

---

## Caso 2: Sugerencia modificada

* **Herramienta:** Gemini (Google)
* **Objetivo:** Diseñar un contenedor de tarjetas flexible y adaptable a diferentes tamaños de pantalla.
* **Prompt:** "¿Cómo puedo hacer que las tarjetas se adapten a escritorio y móvil usando Flexbox?"
* **Respuesta obtenida:** La IA propuso un diseño basado en un ancho fijo por tarjeta con `flex: 0 0 30%` y media queries complejas para forzar los saltos de línea.
* **Evaluación:** El uso de porcentajes fijos limitaba la reutilización real si se añadía una cuarta tarjeta y requería demasiadas líneas de código innecesarias en las media queries.
* **Decisión:** **Modificada**. Se adaptó la solución utilizando `flex: 1 1 280px` junto con `flex-wrap: wrap`, permitiendo que el navegador gestione de forma automática el flujo y los saltos de línea ante cualquier cantidad de tarjetas sin romper el diseño responsive.
* **Resultado:** Se implementó una clase `.cards` y `.card` limpia, flexible y 100% reutilizable.

---

## Caso 3: Sugerencia rechazada por no ajustarse al requisito

* **Herramienta:** Gemini (Google)
* **Objetivo:** Implementar estilos y un menú desplegable para dispositivos móviles.
* **Prompt:** "¿Cómo puedo crear un menú hamburguesa interactivo para la versión móvil?"
* **Respuesta obtenida:** La IA sugirió importar un framework externo de CSS (como Bootstrap) o implementar un script completo en JavaScript con lógica de eventos para alternar clases de visibilidad.
* **Evaluación:** El proyecto requería una solución ligera basada estrictamente en HTML semántico y CSS puro (utilizando `@media (max-width: 700px)` y `flex-direction: column` para la navegación móvil), sin dependencias de frameworks pesados ni lógica de JavaScript innecesaria en esta fase.
* **Decisión:** **Rechazada**, porque contravenía los principios de ligereza y el alcance técnico solicitado para el diseño responsive con CSS nativo.
* **Resultado:** Se descartó el uso de frameworks o scripts complejos, resolviendo la adaptación móvil únicamente con la regla `@media (max-width: 700px)` y la reorganización vertical del menú.

# Taller HTML5 + CSS 
 
## Objetivo 
Se construyó una landing page web institucional de una sola página, estructurada con HTML5 semántico y estilizada con CSS3 modular. Incluye una barra de navegación adaptable, una sección de servicios con tarjetas flexibles reutilizables, y un formulario de contacto validado nativamente, garantizando una excelente experiencia visual y accesibilidad en dispositivos móviles y de escritorio.
 
## Variante asignada 
* **Contexto:** Sitio web corporativo para presentación de servicios institucionales y captación de clientes mediante formulario de contacto.
* **Restricción visual:** Uso estricto de paleta de colores corporativa definida mediante variables CSS (`:root`), tipografía moderna y limpia, y maquetación libre de desbordamientos horizontales.
* **Requisito técnico:** Uso de Flexbox para el diseño de tarjetas responsivas (`flex-wrap`, `flex-basis`), clases reutilizables (`.card`, `.btn`), selectores eficientes y manejo de accesibilidad mediante `:focus-visible`.
 
## Tecnologías 
HTML5, CSS3, Git y GitHub. 
 
## Cómo ejecutar 
1. Clona o descarga los archivos del proyecto.
2. Abre la carpeta en tu editor de código preferido (ej. VS Code).
3. Abre el archivo **`index.html`** en cualquier navegador web o ejecuta un servidor local (como *Live Server*).
 
## Decisiones de diseño 
1. **Centralización con Variables CSS (`:root`):** Se definieron propiedades globales para colores, fuentes y espaciados, lo que permite un mantenimiento centralizado del diseño y asegura una coherencia visual en todo el sitio.
2. **Componente de Tarjetas Flexible:** Se utilizó Flexbox (`flex: 1 1 280px` y `flex-wrap`) para que las tarjetas se adapten automáticamente a cualquier ancho de pantalla y permitan añadir elementos adicionales (como una 4ª tarjeta) sin romper el diseño de la cuadrícula.
3. **Accesibilidad con `:focus-visible`:** Se implementó un resaltado por teclado exclusivo para elementos interactivos, mejorando la usabilidad y cumpliendo con los estándares de accesibilidad web para usuarios que no emplean ratón.
 
## Uso de IA 
Se utilizó **Gemini** como asistente de colaboración técnica durante el desarrollo para resolver dudas sobre el comportamiento de Flexbox en pantallas pequeñas, la optimización de selectores para accesibilidad y la estructuración modular del CSS. Las interacciones significativas, junto con sus respectivas evaluaciones, modificaciones y rechazos, se encuentran detalladas en el registro de evidencias.
* **Ubicación de evidencias:** [`evidencias/ia/registro_ia.md`](evidencias/ia/registro_ia.md)
 
## Evidencias 
- [ ] Preguntas manuscritas 
- [ ] Captura desktop 
- [ ] Captura móvil