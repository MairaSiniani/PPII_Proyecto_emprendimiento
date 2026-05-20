# Caso de uso: Registrar Material
## Actores: Usuario (Administrador)
## Precondiciones: 

El usuario debe haber iniciado sesión en el sistema.

## Camino Básico:
1. El usuario accede a la opción “Registrar material”.
2. El sistema muestra el formulario de carga de material.
3. El usuario ingresa los datos requeridos: nombre, tipo, característica, cantidad disponible, precio y categoría, y selecciona "Registrar".
4. El sistema valida los datos ingresados, guarda el material en el stock y muestra un mensaje de confirmación.

## Caminos Alternativos:

3. 1.  Cancelación del registro
        1. El usuario cancela la operación.
        2. El sistema no guarda datos y regresa al menú principal.

4. 1.  Datos incompletos

        1. El sistema detecta campos obligatorios vacíos y muestra un mensaje: "Debe completar todos los campos obligatorios".
        2. El usuario corrige los datos y vuelve al paso 3.

    2. Datos inválidos

        1. El sistema detecta datos incorrectos (por ejemplo: cantidad o precio negativos) y muestra un mensaje: "Datos inválidos".
        2. El usuario corrige los datos y vuelve al paso 3.


## Postcondiciones:

1. El material queda registrado en el sistema.
2. El material está disponible en el listado de stock.

## Escenarios de Éxito:
1. El usuario registra correctamente un material y el sistema lo almacena sin errores.
2. El sistema confirma el registro y actualiza el stock.

## Escenarios de Fracaso:
1. El usuario ingresa datos incompletos o inválidos.
2. El sistema impide el registro y muestra un mensaje de error.
3. El usuario cancela la operación antes de finalizar.