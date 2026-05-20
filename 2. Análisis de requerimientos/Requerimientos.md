# Requerimientos funcionales del sistema

## 1. Stock
1. El sistema debe permitir registrar materiales (nombre, tipo, característica, cantidad disponible, precio, categoría).
2. El sistema debe permitir modificar y eliminar materiales.
3. El sistema debe permitir consultar el stock disponible.
4. El sistema debe permitir filtrar el stock por nombre, tipo, categoría.
5. El sistema debe generar alertas de stock bajo.
6. El sistema debe mantener un historial de precios de los materiales.

## 2. Gestión de productos y servicios
1. El sistema debe permitir crear productos (nombre, costo de producción, precio de venta, categoría).
2. El sistema debe permitir crear servicios (nombre, costo de servicio).
3. El sistema debe permitir modificar y eliminar productos.
4. El sistema debe permitir modificar y eliminar servicios.
5. El sistema debe permitir calcular automáticamente el precio de venta del producto, considerando: costo de materiales y porcentaje de ganancia (30% o 40%).
6. El sistema debe permitir calcular automáticamente el precio de un servicio considerando precio por hora, cantidad de horas.
7. El sistema debe permitir consultar productos y servicios.

## 3. Gestión de Pedidos
1. El sistema debe permitir registrar pedidos.
2. El sistema debe permitir agregar uno o más ítems al pedido, donde cada ítem puede ser un producto (con cantidad) y/o un servicio.
3. El sistema debe calcular automáticamente el total del pedido y el 50% del total como seña.
4. El sistema debe permitir registrar el pago de la seña.
5. El sistema debe confirmar el pedido solo si la seña fue pagada. En caso contrario, el pedido no debe registrarse como válido.
6. El sistema debe permitir modificar pedidos (si no están entregados).
7. El sistema debe permitir eliminar pedidos.
8. El sistema debe permitir cambiar el estado del pedido, con los siguientes estados: pendiente, en proceso, terminado, entregado.
10. El sistema debe permitir consultar la lista de pedidos.
11. El sistema debe permitir visualizar el detalle de cada pedido.
12. El sistema debe registrar la fecha del pedido

## 4. Gestión de Ventas
1. El sistema debe generar automáticamente una venta cuando un pedido cambia al estado “entregado”.
2. El sistema debe registrar en la venta los ítems del pedido (productos/servicios), las cantidades, el total, la fecha de fecha de entrega y el medio de pago.
3. El sistema debe permitir consultar el historial de ventas.
4. El sistema debe permitir visualizar el detalle de cada venta.
5. El sistema debe permitir utilizar la información de ventas para reportes.

## 5. Gestión Financiera
1. El sistema debe permitir registrar gastos.
2. El sistema debe permitir visualizar ingresos y egresos.
3. El sistema debe calcular automáticamente: costos totales, ganancias.
4. El sistema debe permitir diferenciar dinero disponible y dinero para reinversión.

## 6. Reportes
1. El sistema debe generar reportes gráficos de: ventas, gastos, ganancias.
2. El sistema debe permitir consultar estadísticas generales del negocio.

## 7. Proveedores
1. El sistema debe permitir registrar proveedores (nombre, contacto, materiales).
2. El sistema debe permitir modificar y eliminar proveedores.
3. El ss debe permitir consultar proveedores


## 8. Usuarios 
1. El sistema debe permitir crear, consultar, modificar y eliminar usuarios.
2. El sistema debe permitir gestionar múltiples usuarios.
3. El sistema debe permitir definir roles (ej: administrador).
4. El sistema debe permitir adaptarse a múltiples sucursales en el futuro.

## 9. Materiales
1. El sistema debe permitir crear, consultar, modificar y eliminar materiales. 