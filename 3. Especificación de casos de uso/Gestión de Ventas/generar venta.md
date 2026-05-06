# Caso de uso: Generar Venta
## Actores: Sistema 
## Precondiciones:
Debe existir un pedido registrado.
El pedido debe cambiar a estado “entregado”.
El pago debe estar completo.

## Camino Básico:
1. El usuario cambia el estado del pedido a “entregado”.
2. El sistema detecta el cambio de estado.
3. El sistema genera automáticamente una venta.
4. El sistema copia los datos del pedido: ítems, cantidades, total.
5. El sistema registra la fecha de entrega.
6. El sistema guarda la venta en el historial.

## Caminos Alternativos:

3. 1. Error al generar venta
        1. El sistema no puede generar la venta.
        2. El sistema muestra un mensaje de error.

## Postcondiciones:
La venta queda registrada automáticamente en el sistema.

## Escenarios de Éxito:
El sistema genera la venta correctamente al marcar el pedido como entregado.

## Escenarios de Fracaso:
Ocurre un error del sistema al generar la venta.