# Caso de uso: Registrar Pedido
## Actores: Usuario 
## Precondiciones: 
El usuario debe haber iniciado sesión. Debe existir al menos un un material y un producto o servicio registrado.

## Camino Básico:
1. El usuario accede al módulo de pedidos y selecciona “Registrar pedido”.
2. El sistema crea un nuevo pedido.
3. El usuario agrega uno o más ítems: selecciona producto y cantidad, o
selecciona el servicio (puede agregar notas de especificación y fecha de entrega) y selecciona "Siguiente".
4. El sistema calcula el total del pedido, el 50% del total como seña y muestra los montos en pantalla.
5. El usuario registra el pago de la seña.
6. El sistema confirma el pedido solo si la seña fue registrada y guarda el pedido con estado, fecha de creación y fecha de entrega (si fue ingresada).

## Caminos Alternativos:

4. 1. Pedido sin ítems
        1. El usuario no agrega productos ni servicios.
        2. El sistema muestra: "Debe agregar al menos un ítem".
        3. El usuario vuelve al paso 3.

   2. Error en cálculo
        1. El sistema no puede calcular el total y muestra error.
        2. EL usuario vuelve al paso 3.

5. 1. Seña no pagada
        1. El usuario no registra el pago de la seña.
        2. El sistema no confirma el pedido.

## Postcondiciones:
El pedido queda registrado con su detalle, total y estado inicial.

## Escenarios de Éxito:
El usuario logra que el pedido se registre correctamente con seña confirmada.

## Escenarios de Fracaso:
1. No se registra el pedido.