# Caso de uso: Consultar Stock
## Actores: Usuario (Administrador)
## Precondiciones:
El usuario debe haber iniciado sesión en el sistema.
Deben existir al menos un material registrado en el sistema.

## Camino Básico:

1. El usuario accede al módulo de stock.
2. El sistema obtiene la lista de materiales registrados.
3. El sistema muestra el stock disponible con sus datos (nombre, tipo, característica, cantidad, precio y categoría).
4. El usuario visualiza la información del stock.

## Caminos Alternativos:

3. 1. Sin materiales registrados
        1. El sistema no encuentra materiales en el stock y muestra un mensaje: "No hay materiales registrados".
        2. El usuario puede optar por registrar un nuevo material.

     2. Error al cargar el stock
        1. El sistema no puede obtener los datos del stock, muestra un mensaje de error: "No fue posible cargar el stock" y ofrece la opción de reintentar la operación.

## Postcondiciones:
-

## Escenarios de Éxito:
El usuario accede al stock y visualiza correctamente todos los materiales disponibles.

## Escenarios de Fracaso:
1. No existen materiales registrados en el sistema.
2. Ocurre un error al cargar los datos del stock.