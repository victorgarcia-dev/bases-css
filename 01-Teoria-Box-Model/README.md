# 📦 Teoría 01: El Modelo de Caja (Box Model) y Selectores

¡Bienvenido a tu primer apunte de CSS!

Antes de empezar a mover cosas por la pantalla, necesitas entender la regla de oro del diseño web: **Absolutamente todo en una página web es un rectángulo (una caja)**. Incluso si ves un botón redondo, el navegador lo calcula como una caja.

## 🔍 El Modelo de Caja (Box Model)

Para darle estilo a un elemento, debes entender las 4 capas que lo componen, de adentro hacia afuera:

1. **Content (Contenido):** Es el corazón de la caja. El texto, la imagen o el video real. Sus dimensiones se controlan con `width` (ancho) y `height` (alto).
2. **Padding (Relleno interno):** Es el espacio transparente entre el contenido y el borde de la caja. Si le pones color de fondo a la caja, el padding se pintará de ese color. Sirve para que el texto "respire" y no esté pegado a las paredes.
3. **Border (Borde):** La pared de la caja. Puedes elegir su grosor, estilo (sólido, punteado) y color.
4. **Margin (Margen externo):** Es el espacio invisible _fuera_ del borde. Sirve para empujar a los elementos vecinos y separarlos entre sí.

> 🚨 **El truco de la vida (`box-sizing`):** Por defecto, si a una caja de 100px de ancho le agregas 20px de padding, la caja crecerá a 140px. ¡Esto rompe los diseños! Para evitarlo, siempre ponemos `box-sizing: border-box;` al inicio de nuestro CSS. Esto obliga a la caja a encoger su contenido en lugar de agrandarse hacia afuera.

---

## 🎯 Selectores: ¿A quién le damos estilo?

Para pintar algo, primero debemos "seleccionarlo". CSS tiene 3 formas principales de apuntar a un elemento:

- **Por Etiqueta (`h1`, `p`, `button`):** Afecta a _todos_ los elementos de ese tipo en la página. Es muy general.
- **Por Clase (`.mi-clase`):** Se usa un punto al inicio. Afecta a cualquier elemento que tenga el atributo `class="mi-clase"`. Es la forma más usada y recomendada (¡se puede repetir!).
- **Por ID (`#mi-id`):** Se usa un numeral al inicio. Afecta a un _único_ elemento con el atributo `id="mi-id"`. Como un DNI, no puede haber dos elementos con el mismo ID.

---

## 🛠️ ¿Cómo usar esta carpeta?

1. Abre el archivo `index.html` con Live Server.
2. Abre el archivo `style.css` y lee los comentarios del profesor.
3. Abre las herramientas de desarrollador de tu navegador (F12 o Clic derecho -> Inspeccionar) y busca la pestaña "Computed" o "Estilos" para ver el Modelo de Caja en vivo de cada elemento.
