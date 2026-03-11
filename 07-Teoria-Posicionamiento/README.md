# 📍 Teoría 07: Posicionamiento (Rompiendo el flujo)

Hasta ahora, hemos maquetado siguiendo el "flujo normal" del documento: las cosas se apilan de arriba hacia abajo, y si usamos Flexbox o Grid, se acomodan en su celda.

Pero, ¿qué pasa si queremos un botón flotante de WhatsApp en la esquina inferior que nunca se mueva, o un cartelito de "Oferta" superpuesto en la esquina de una foto? Ahí entra la propiedad `position`.

## 🛠️ Los 5 Valores de `position`

1. **`static` (Por defecto):**
   - Es el comportamiento normal. El elemento fluye con el resto del contenido. Propiedades como `top`, `bottom`, `left` y `right` **NO** funcionan aquí.

2. **`relative` (Relativo a sí mismo):**
   - El elemento se mueve _en relación a dónde debería haber estado originalmente_.
   - **Ojo:** Aunque lo muevas, su "fantasma" sigue ocupando el espacio original, por lo que no empuja a los demás elementos.
   - Es **CRUCIAL** porque se usa como ancla para el posicionamiento Absoluto.

3. **`absolute` (Absoluto - El rebelde):**
   - El elemento se "arranca" del flujo de la página. Ya no ocupa espacio y los demás elementos actúan como si no existiera.
   - Se posiciona en relación a su **ancestro más cercano que tenga un `position` distinto a `static`** (generalmente le ponemos `position: relative;` al padre). Si no encuentra ninguno, se posiciona en relación a la página entera.

4. **`fixed` (Fijo a la cámara):**
   - Se saca del flujo normal (como absolute), pero se posiciona en relación a la **ventana del navegador (viewport)**.
   - Aunque hagas scroll hacia abajo, el elemento no se mueve de la pantalla. Ideal para botones de WhatsApp o menús.

5. **`sticky` (Pegajoso - El híbrido):**
   - Se comporta como `relative` hasta que haces scroll y llegas a su posición. En ese momento, se "pega" a la pantalla y empieza a comportarse como `fixed`. Ideal para encabezados de tablas o barras de navegación secundarias.
