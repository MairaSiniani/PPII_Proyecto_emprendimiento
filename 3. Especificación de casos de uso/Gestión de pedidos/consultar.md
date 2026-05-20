## Caso de uso: Consultar Pedidos
# Actores: Usuario
## Precondiciones:

Debe existir al menos un pedido. 

## Camino Básico:
1. El usuario accede al módulo de pedidos.
2. El sistema obtiene la lista de pedidos y muestra fecha,estado y total.
4. El usuario puede seleccionar un pedido.
5. El sistema muestra el detalle.

## Caminos Alternativos:

5. No hay detalles agregados.
    1. El sistema muestra un mensaje "No hay detalles registrados".
    2. El usuario puede elegir añadir pedidos y sale del módulo pedidos.

## Postcondiciones:
El usuario visualiza los pedidos y sus detalles.