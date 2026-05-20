# Caso de uso: Eliminar Pedido
## Actores: Usuario 
## Precondiciones:
Debe existir un pedido registrado.

## Camino Básico:
1. El usuario accede al listado de pedidos.
2. El sistema obtiene la lista de pedidos registrados.
3. El usuario selecciona un pedido y elige "Eliminar"
4. El sistema solicita confirmación.
5. EL usuario confirma la acción.
6. El sistema elimina el pedido.

## Caminos Alternativos:

5. 1. El usuario cancela la eliminación.
        1. El sistema no realiza ninguna operación y retira la solicitud de confirmación.
        2. El usuario vuelve al paso 1.

## Postcondiciones:
El pedido es eliminado.

## Escenarios de écito: 

1. EL usuario puede eliminar el pedido.
## Escenarios de Fracaso:
1. Error del sistema al eliminar el pedido.