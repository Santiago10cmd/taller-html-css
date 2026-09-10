Taller HTML5 + CSS
Objetivo
Se construyó una página web institucional de una sola página (Landing Page) que incluye secciones de Inicio, Servicios, Sobre Nosotros y un Formulario de Contacto interactivo, accesible y adaptativo (responsive).

Variante asignada
Contexto: Sitio web corporativo con secciones informativas y recolección de datos de contacto para la captación de usuarios.
Restricción visual: Uso de paleta de colores corporativa mediante un azul primario (#17365D) y un naranja de acento (#ED7D31), manteniendo una cuadrícula flexible de tarjetas.
Requisito técnico: HTML5 semántico sin frameworks externos, uso de variables CSS (:root), diseño fluido con Flexbox (flex-wrap) y manejo de accesibilidad mediante :focus-visible.
Tecnologías
HTML5, CSS3, Git y GitHub.

Cómo ejecutar
Clonar este repositorio o descargar el archivo .zip del proyecto.
Navegar a la carpeta raíz del proyecto.
Abrir el archivo index.html en cualquier navegador web moderno (Chrome, Firefox, Edge).
Decisiones de diseño
Uso de Flexbox para la sección de tarjetas (.cards): Se implementó display: flex con flex-wrap: wrap y flex: 1 1 280px para lograr que los servicios se reorganicen solos según el tamaño de la pantalla sin romper la estructura.
Sistema de Variables en CSS (:root): Se definieron colores, espaciados y radios de borde globales (--color-primary, --space, --border-radius) para asegurar coherencia visual y facilitar cambios de diseño futuros en un solo lugar.
Accesibilidad e interacción en el formulario: Se asociaron estrictamente las etiquetas <label> con sus respectivos <input> mediante los atributos for/id, y se configuró :focus-visible con el color de acento para usuarios que navegan mediante el teclado.
Uso de IA
Se utilizó Inteligencia Artificial como un apoyo colaborativo para maquetar el código HTML5 semántico, verificar propiedades de Flexbox, escribir reglas de accesibilidad CSS y estructurar las respuestas teóricas.

Registro de evidencias: evidencias/ia/registro_ia.md
Evidencias
Preguntas manuscritas: Fotografía adjunta de las preguntas del taller resueltas a mano.
Captura desktop: Imagen de la interfaz mostrada en pantalla ancha (mínimo 3 tarjetas en una fila y formulario centrado).
Captura móvil: Imagen de la interfaz en resolución de 390 px mostrando la reorganización vertical sin scroll horizontal.
