# Caso de uso: Registrar Pedido
## Actores: Usuario 
## Precondiciones: 
El usuario debe haber iniciado sesión. 

## Camino Básico:
1. El usuario accede al módulo de pedidos.
2. El usuario selecciona “Registrar pedido”.
3. El sistema crea un nuevo pedido.
4. El usuario agrega uno o más ítems: selecciona producto y cantidad, o
selecciona el servicio. Puede agregar notas de especificación y fecha de entrega.
5. El sistema calcula el total del pedido.
6. El sistema calcula el 50% del total como seña.
7. El sistema muestra el monto de la seña.
8. El usuario registra el pago de la seña.
9. El sistema confirma el pedido solo si la seña fue registrada.
10. El sistema guarda el pedido con estado “pendiente”, fecha de creación y fecha de entrega (si fue ingresada).

## Caminos Alternativos:

4. 1. Pedido sin ítems
        1. El usuario no agrega productos ni servicios.
        2. El sistema muestra: "Debe agregar al menos un ítem".

5. 1. Error en cálculo
        1. El sistema no puede calcular el total.
        2. El sistema muestra error.

8. 1. Seña no pagada
        1. El usuario no registra el pago de la seña.
        2. El sistema no confirma el pedido.
        3. El pedido no se registra como válido.

## Postcondiciones:
El pedido queda registrado con su detalle, total y estado inicial.

## Escenarios de Éxito:
El pedido se registra correctamente con seña confirmada.

## Escenarios de Fracaso:
1. No se paga la seña.
2. No hay ítems en el pedido.
3. Error del sistema.