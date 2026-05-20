# Caso de uso: Calcular precio de producto
## Actores: Sistema, Usuario
## Precondiciones:
Debe existir un producto registrado.
El producto debe tener definido su costo de producción (basado en los materiales).

## Camino Básico:
1. El usuario accede al módulo de productos, selecciona uno y hace click en "Calcular precio".
2. El sistema obtiene el costo de producción del producto y solicita al usuario definir un porcentaje de ganancia.
3. El usuario ingresa el porcentaje y selecciona "Finalizar"
4. El sistema calcula el precio final de venta y lo muestra en pantalla.
5. El usuario selecciona "Guardar".

## Caminos Alternativos:

2. 1. Porcentaje no definido.
    1. El sistema detecta que no se definió el porcentaje de ganancia.
    2. El sistema solicita seleccionar un porcentaje.
    3. El usuario vuelve al paso 2.

4. 1. Error en el cálculo
        1. El sistema no puede realizar el cálculo.
        2. El sistema muestra un mensaje: "No fue posible calcular el precio".

## Postcondiciones:
1. El precio de venta del producto queda calculado y guardado.

## Escenarios de Éxito:
1. El sistema calcula correctamente el precio aplicando el porcentaje de ganancia.
2. El usuario obtiene un precio adecuado para no perder dinero.

## Escenarios de Fracaso:
1. Falta información (costo o porcentaje).
2. Ocurre un error en el cálculo.