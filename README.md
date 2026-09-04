# Catálogo Ferretería (estático)

`productos.json`: catálogo completo de productos (código de barras, código interno, descripción, precio) que usa la app del scanner para buscar productos, sin depender de un servidor que se pueda dormir.

Se sirve gratis y siempre disponible via GitHub (raw.githubusercontent.com) — sin costo de hosting.

## Cómo actualizar
Cuando cambien precios o se agreguen productos:
1. Subir el Excel actualizado en https://ferreteria-backend-tk8o.onrender.com/importar.html (esto actualiza la base de datos real).
2. Descargar el catálogo actualizado: `GET https://ferreteria-backend-tk8o.onrender.com/api/productos`
3. Reemplazar `productos.json` acá y hacer `git push`.

(Por ahora este paso 2-3 lo hace Claude a pedido; se puede automatizar más adelante.)
