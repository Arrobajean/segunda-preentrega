
El código proporcionado implementa un carrito de compras básico en JavaScript, utilizando el DOM y SweetAlert para la interacción con el usuario. Aquí hay una breve descripción de lo que hace el código:

Inicialización:

Se inicializa la variable carrito llamando a la función cargarCarrito(), que verifica si existen valores en el almacenamiento local (localStorage) y devuelve un array vacío o el carrito existente.
Manipulación del DOM:

Se obtienen referencias a las secciones relevantes del HTML, como sectionProductos y sectionCarrito.
Se crea dinámicamente la sección del carrito con elementos como el total de la compra, la cantidad de productos y un botón para finalizar la compra.
Renderizado de Productos:

Se recorre la lista de productos (productos) y se crean elementos de tarjetas para cada uno, que incluyen una imagen, nombre, precio y un botón para agregar al carrito.
Se asigna un evento a cada botón para agregar el producto correspondiente al carrito al hacer clic.
Funciones del Carrito:

agregarAlCarrito(id): Agrega un producto al carrito utilizando su ID, lo busca en la lista de productos y lo añade al carrito. También actualiza el almacenamiento local y recalcula el total del carrito.
calcularTotalCarrito(): Calcula el precio total del carrito sumando los precios de todos los productos en el carrito y actualiza la visualización en el DOM.
vaciarCarrito(): Vacía el carrito, actualiza la visualización en el DOM, limpia el almacenamiento local y reinicia la variable carrito.
cargarCarrito(): Carga el carrito desde el almacenamiento local, devolviendo un array vacío si no hay datos.
Evento de Finalización de Compra:

Se añade un evento al botón "Finalizar compra" que muestra un cuadro de diálogo de confirmación (utilizando SweetAlert) con el total a pagar. Si el usuario confirma, se vacía el carrito.

# segunda-preentrega
