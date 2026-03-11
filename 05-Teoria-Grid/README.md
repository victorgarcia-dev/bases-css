# 🍱 Teoría 05: CSS Grid (El Arquitecto 2D)

¡Bienvenido al nivel Dios de la maquetación!

- **Flexbox** es increíble para alinear elementos en una sola línea (una fila de botones, un navbar). Es unidimensional.
- **CSS Grid** nació para estructurar páginas enteras. Te permite controlar **filas y columnas al mismo tiempo**. Es bidimensional.

## 🧠 El Concepto Base: La Cuadrícula

Al igual que en Flexbox, Grid se aplica al **Padre (Contenedor)**. Al encenderlo, creas una cuadrícula invisible y le dices a los elementos hijos en qué "celdas" deben ubicarse.

---

## 🛠️ Las Propiedades Mágicas del Padre

1. **`display: grid;`** Enciende el motor Grid. Por defecto, solo apila los elementos uno sobre otro.
2. **`grid-template-columns:`**
   - Define cuántas columnas quieres y de qué tamaño.
   - _Ejemplo:_ `grid-template-columns: 100px 200px 100px;` (Crea 3 columnas fijas).
3. **La Unidad Mágica (`fr` - Fracción):**
   - CSS Grid introdujo una unidad nueva. `1fr` significa "una fracción del espacio libre".
   - _Ejemplo:_ `grid-template-columns: 1fr 1fr 1fr;` (Crea 3 columnas exactamente iguales, sin importar el tamaño de la pantalla).
4. **La Función `repeat()`:**
   - Para no escribir `1fr 1fr 1fr 1fr`, los programadores somos flojos y usamos: `grid-template-columns: repeat(4, 1fr);`.
5. **`gap:`**
   - Crea el espacio (hueco) perfecto entre las celdas, tanto vertical como horizontalmente.

---

## 🏗️ Modificando al Hijo (Ocupar más espacio)

A veces quieres que un elemento sea el "destacado" y ocupe más de una celda (como una noticia principal en un diario). Eso se lo aplicas al elemento hijo:

- **`grid-column: span 2;`** Le dice al elemento: "Estírate y ocupa 2 columnas".

---

## 🏆 El Santo Grial: Responsive sin Media Queries

CSS Grid tiene un truco que Flexbox envidia. Puedes hacer que tu cuadrícula se adapte a cualquier tamaño de pantalla automáticamente usando la combinación de `repeat`, `auto-fit` y `minmax()`.

```css
.contenedor {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}
```

---

## 🥕 Práctica Extra: ¡Planta tu Jardín!

La mejor forma de memorizar estas propiedades no es leyendo, ¡es jugando!

Te recomendamos encarecidamente que, antes de pasar al siguiente reto, entres a **[Grid Garden](https://cssgridgarden.com/)**.

Es un minijuego gratuito donde tendrás que usar código CSS Grid (`grid-column`, `grid-template-columns`, etc.) para regar tus zanahorias y envenenar la maleza. Si logras pasar los 28 niveles, ¡ya te puedes considerar un cinturón negro en CSS Grid!
