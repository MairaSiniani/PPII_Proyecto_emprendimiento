# Caso de uso: Generar Venta
## Actores: Sistema 
## Precondiciones:
Debe existir un pedido registrado.
El pedido debe tener como estado “entregado”.
El pago debe estar completo.

## Camino Básico:
1. El usuario cambia el estado del pedido a “entregado”.
2. El sistema detecta el cambio de estado y registra la venta con los datos: ítems, cantidades, total, fecha de entrega.
3. El usuario selecciona "Guardar".
4. El sistema guarda los datos.

## Caminos Alternativos:

3. 1. Error al generar venta
        1. El sistema no puede generar la venta y muestra un mensaje de error.

## Postcondiciones:
La venta queda registrada automáticamente en el sistema.

## Escenarios de Éxito:
El sistema genera la venta correctamente al marcar el pedido como entregado.

## Escenarios de Fracaso:
Ocurre un error del sistema al generar la venta.