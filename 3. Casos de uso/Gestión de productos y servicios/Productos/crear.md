# Caso de uso: Crear producto
## Actores: Usuario (Administrador)
## Precondiciones:

El usuario debe haber iniciado sesión en el sistema. Debe haber al menos un material registrado.

##  Camino Básico:

1. El usuario accede al módulo de productos.
2. El usuario selecciona la opción “Nuevo producto”.
3. El sistema muestra el formulario de carga.
4. El usuario ingresa los datos: nombre, costo de producción, precio de venta, categoría.
5. El usuario confirma el registro.
6. El sistema valida los datos ingresados.
7. El sistema guarda el producto en el sistema.
8. El sistema muestra un mensaje de confirmación.

## Caminos Alternativos:

5. 1.  Cancelación del registro
        1. El usuario cancela la operación.
        2.  El sistema no guarda el producto y vuelve al menú.

6. 1. Datos incompletos
        1. El sistema detecta campos obligatorios vacíos.
        2. El sistema muestra un mensaje: "Debe completar todos los campos obligatorios".
        3. El usuario corrige los datos y vuelve al paso 4.

    2. Datos inválidos
        1. El sistema detecta valores incorrectos.
        2. El sistema muestra un mensaje: "Datos inválidos".
        3. El usuario vuelve al paso 4.

## Postcondiciones:
El producto queda registrado en el sistema.

## Escenarios de Éxito:
El usuario registra correctamente un producto y el sistema lo almacena.

## Escenarios de Fracaso:
1. El usuario ingresa datos incompletos o inválidos.
2. El sistema impide el registro y muestra un mensaje de error.