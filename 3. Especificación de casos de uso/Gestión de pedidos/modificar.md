# Caso de uso: Modificar Pedido
## Actores: Usuario 
## Precondiciones:
Debe existir un pedido registrado. El pedido no debe estar en estado “entregado”.

## Camino Básico:
1. El usuario accede al listado de pedidos.
2. El sistema muestra los pedidos.
3. El usuario selecciona un pedido y modifica ítems, cantidades o fechas.
4. El sistema recalcula el total y la seña.
5. El usuario confirma los cambios.
6. El sistema guarda la actualización.

## Caminos Alternativos:

4. 1. Pedido entregado
        1. El sistema detecta estado “entregado” y no permite modificaciones.
        2. El usuario vuelve al paso 1.

5. 1. Datos inválidos
        1. El sistema muestra error.
        2. EL usuario vuelve al paso 3.

## Postcondiciones:
El pedido queda actualizado y se recalculan el total y la seña.

## Escenarios de éxito:
El usuario puede modificar el pedido y se actualizan los datos.

## Escenarios de fracaso:
1. No se puede modificar el pedido
2. Los datos son inválidos