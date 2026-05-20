# Caso de uso: Cambiar Estado de Pedido
## Actores: Usuario 
## Precondiciones:

Debe existir un pedido registrado.

## Camino Básico:
1. El usuario accede al listado de pedidos.
2. EL sistema despliega la lista de pedidos registrados.
3. El usuario elige cambiar estado (pendiente, en proceso, terminado, entregado).
4. El sistema actualiza el estado y guarda el cambio.

## Caminos Alternativos:

3. 1. El usuario no cambia el estado del pedido
    1. El sistema no hace ningún cambio

## Postcondiciones:
El pedido queda registrado con el nuevo estado.