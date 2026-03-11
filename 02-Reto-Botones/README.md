# 🎯 Reto 02: Diseñando Botones (Box Model)

¡Hora de practicar! Todo lo que aprendiste sobre márgenes, rellenos (padding) y bordes lo vas a aplicar aquí. Los botones son el elemento más interactivo de cualquier página web.

## 🎯 El Objetivo

Darle estilo a 3 botones distintos utilizando únicamente las propiedades del Modelo de Caja y pseudo-clases como `:hover`.

### 👀 Referencia Visual (Resultado Esperado)

_(Profe: Reemplaza esta línea con tu captura de los botones terminados)_
![Vista previa de los botones](assets/preview.png)

---

## 📝 Instrucciones

Abre el archivo `index.html`. Verás que hay 3 botones con diferentes clases dentro de un contenedor. Tu misión es ir al archivo vacío `style.css` y darles estilo hasta que se vean como en la imagen de arriba.

**Lo que debes lograr visualmente:**

**1. Los 3 botones en general:**

- Se deben ver limpios, sin el borde cuadrado gris que el navegador les pone por defecto.
- Al pasar el mouse por encima, el cursor debe cambiar a una manito.
- Debe haber espacio entre ellos para que no estén pegados.
- Cualquier cambio al hacer hover debe sentirse suave, no brusco.

**2. Botón Primario (`.btn-primario`):**

- Se ve como un botón azul sólido con texto blanco y esquinas redondeadas.
- Al pasar el mouse, el azul se oscurece un poco.

**3. Botón Secundario / Outline (`.btn-outline`):**

- El fondo es transparente. Se ve solo el borde y el texto, ambos en color verde.
- Al pasar el mouse, el efecto se invierte: el fondo se vuelve verde y el texto blanco.

**4. Botón Peligro (`.btn-peligro`):**

- Fondo rojo con texto blanco. A diferencia de los otros, sus esquinas son completamente rectas (sin redondear).
- Al pasar el mouse, no cambia de color, pero aparece una sombra rojiza debajo que da la sensación de que el botón se eleva.
