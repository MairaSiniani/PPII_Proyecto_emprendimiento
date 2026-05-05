# Caso de uso: Calcular precio de producto
## Actores: Sistema, Usuario
## Precondiciones:
Debe existir un producto registrado.
El producto debe tener definido su costo de producción (basado en los materiales).

## Camino Básico:
1. El usuario accede al módulo de productos.
2. El usuario selecciona un producto.
3. El usuario solicita calcular el precio de venta.
4. El sistema obtiene el costo de producción del producto.
5. El sistema aplica el porcentaje de ganancia definido.
6. El sistema calcula el precio final de venta.
7. El sistema muestra el precio calculado al usuario.
8. El sistema permite guardar el precio como precio de venta del producto.

## Caminos Alternativos:

5. 1. Porcentaje no seleccionado
    1. El sistema detecta que no se definió el porcentaje de ganancia.
    2. El sistema solicita seleccionar un porcentaje.
    3. El usuario vuelve al paso 5.

6. 1. Error en el cálculo
        1. El sistema no puede realizar el cálculo.
        2. El sistema muestra un mensaje: "No fue posible calcular el precio".

## Postcondiciones:
1. El precio de venta del producto queda calculado.
2. El precio puede quedar guardado como valor actual del producto.

## Escenarios de Éxito:
1. El sistema calcula correctamente el precio aplicando el porcentaje de ganancia.
2. El usuario obtiene un precio adecuado para no perder dinero.

## Escenarios de Fracaso:
1. Falta información (costo o porcentaje).
2. Ocurre un error en el cálculo.