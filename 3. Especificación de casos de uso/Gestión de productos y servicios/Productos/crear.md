# Caso de uso: Crear producto
## Actores: Usuario (Administrador)
## Precondiciones:

El usuario debe haber iniciado sesión en el sistema. Debe haber registrado al menos un material.

##  Camino Básico:

1. El usuario accede al módulo de productos y selecciona la opción “Nuevo producto”.
2. El sistema muestra el formulario de carga.
3. El usuario ingresa los datos (nombre, costo de producción, precio de venta, categoría, materiales) y confirma el registro.
4. El sistema valida los datos ingresados, guarda el producto y muestra un mensaje de confirmación.

## Caminos alternativos:

3. 1.  Cancelación del registro
        1. El usuario cancela la operación.
        2.  El sistema no guarda el producto y vuelve al menú.

   2. Datos incompletos
        1. El sistema detecta campos obligatorios vacío y muestra un mensaje: "Debe completar todos los campos obligatorios".
        3. El usuario corrige los datos y vuelve al paso 2.

    2. Datos inválidos
        1. El sistema detecta valores incorrectos.
        2. El sistema muestra un mensaje: "Datos inválidos".
        3. El usuario vuelve al paso 2.

## Postcondiciones:
El producto queda registrado en el sistema.

## Escenarios de Éxito:
El usuario registra correctamente un producto y el sistema lo almacena.

## Escenarios de Fracaso:
1. El usuario ingresa datos incompletos o inválidos.