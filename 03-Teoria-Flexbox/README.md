# 📦 Teoría 03: Flexbox (El Arte de Alinear)

¡Olvídate de sufrir para centrar un elemento! Antes de Flexbox, los desarrolladores usaban trucos oscuros con tablas y `float` para poner una cosa al lado de la otra. Hoy, `display: flex` hace toda la magia por nosotros.

## 🧠 La Regla de Oro de Flexbox

Flexbox funciona bajo una regla estricta de **Padre e Hijos**.
Para usar Flexbox, **NO** se lo aplicas al elemento que quieres mover, se lo aplicas a la **caja contenedora (El Padre)**. Automáticamente, todos sus hijos directos se vuelven "elementos flexibles".

## 🛠️ Las 4 Propiedades Mágicas (Se aplican al PADRE)

1. **`display: flex;`** \* Enciende el motor Flexbox. Por defecto, pone a todos los hijos en una sola fila (uno al lado del otro).
2. **`flex-direction:`**
   - Elige la dirección del flujo.
   - `row` (fila, por defecto) o `column` (columna, apilados hacia abajo).
3. **`justify-content:`** \* Alinea los elementos en el **Eje Principal** (Horizontal si es `row`).
   - Valores estrella: `center`, `space-between` (los separa a los extremos), `space-around`.
4. **`align-items:`** \* Alinea los elementos en el **Eje Cruzado** (Vertical si es `row`).
   - Valores estrella: `center` (los centra verticalmente), `stretch` (los estira).

> 🚨 **El Secreto del Centrado Perfecto:** Si a una caja padre le pones `display: flex; justify-content: center; align-items: center;`, cualquier cosa que esté adentro quedará exactamente en el medio de la pantalla. ¡Magia!

---

## 🐸 Práctica Extra: ¡Salva a las Ranas!

La mejor forma de memorizar estas propiedades no es leyendo, ¡es jugando!

Te recomendamos encarecidamente que, antes de pasar al siguiente reto, entres a **[Flexbox Froggy](https://flexboxfroggy.com/#es)**.

Es un minijuego gratuito donde tendrás que usar código CSS real (`justify-content`, `align-items`, etc.) para llevar a unas ranitas hacia sus hojas. **Si logras pasar los 24 niveles, ¡ya te puedes considerar un cinturón negro en Flexbox!**
