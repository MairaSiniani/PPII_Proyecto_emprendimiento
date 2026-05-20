# Caso de uso: Modificar Producto
## Actores: Usuario (Administrador)
## Precondiciones:
Debe existir al menos un producto registrado.

## Camino Básico:
1. El usuario accede al módulo de productos.
2. El sistema muestra la lista de productos.
3. El usuario selecciona un producto y luego selecciona “Modificar”.
4. El sistema muestra los datos actuales del producto.
5. El usuario edita los campos (nombre, costo de producción, precio de venta, categoría) y confirma los cambios.
6. El sistema valida los datos ingresados, actualiza la información del producto y muestra un mensaje de confirmación.

## Caminos Alternativos:
5. 1. Cancelación de modificación
        1. El usuario cancela la operación.
        2. El sistema no guarda cambios.

6. 1. Datos inválidos
        1. El sistema detecta valores incorrectos y muestra un mensaje: "Datos inválidos".
        3. El usuario vuelve al paso 6.

## Postcondiciones:
El producto queda actualizado en el sistema.

## Escenarios de Éxito:
El usuario modifica correctamente un producto y los cambios se guardan.

## Escenarios de Fracaso:
1. El usuario ingresa datos inválidos.
2. El sistema impide la modificación y muestra error.