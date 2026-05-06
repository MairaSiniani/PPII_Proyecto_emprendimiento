# Caso de uso: Eliminar Pedido
## Actores: Usuario 
## Precondiciones:
Debe existir un pedido.

## Camino Básico:
1. El usuario accede al listado de pedidos.
2. Selecciona un pedido.
3. Elige “Eliminar”.
4. El sistema solicita confirmación.
5. Confirma la acción.
6. El sistema elimina el pedido.

## Caminos Alternativos:

5. 1. Cancelación
        1. El usuario cancela la operación.

## Postcondiciones:
El pedido es eliminado.

## Escenarios de Fracaso:
1. Error del sistema al eliminar el pedido.