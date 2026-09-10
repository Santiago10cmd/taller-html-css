# Registro de Uso de Inteligencia Artificial (IA)

## Resumen del Apoyo Recibido
Durante el desarrollo del taller, la Inteligencia Artificial fue utilizada como una herramienta de apoyo para la estructuración de maquetación HTML/CSS, resolución de dudas teóricas y optimización del código.

## Prompts Utilizados y Resultados

### 1. Formulario y Estructura HTML
* **Prompt/Consulta:** *Generar código HTML limpio, semántico y accesible para un formulario de contacto con campos de nombre, correo, teléfono, asunto, mensaje y términos.*
* **Sugerencia de la IA:** Uso de etiquetas `<form>`, `<label>`, `<input>` y `<textarea>` con validación nativa (`required`).
* **Acción tomada:** Se aceptó la propuesta e integró directamente en la sección `#contacto` de la página.

### 2. Estilos CSS y Responsividad
* **Prompt/Consulta:** *Cómo organizar 4 tarjetas usando Flexbox para que se vean 3 en escritorio y se reorganicen en móvil.*
* **Sugerencia de la IA:** Uso de `.cards { display: flex; gap: 1rem; flex-wrap: wrap; }` y `.card { flex: 1 1 280px; }`.
* **Acción tomada:** Se aplicó la propuesta para garantizar un maquetado responsivo sin scroll horizontal.

### 3. Modificaciones y Criterios Propios
* **Sugerencia rechazada/modificada:** La IA sugirió aplicar selectores de ID específicos para dar estilo a los botones del formulario.
* **Criterio aplicado:** Se modificó la propuesta creando una clase global y reutilizable (`.btn`) para mantener la modularidad y no sobrecargar la especificidad del CSS.

## Declaración de Autoría
El código final, las respuestas al cuestionario teórico y la integración del proyecto fueron revisados, probados y adaptados por el estudiante para cumplir con los requisitos académicos exigidos.