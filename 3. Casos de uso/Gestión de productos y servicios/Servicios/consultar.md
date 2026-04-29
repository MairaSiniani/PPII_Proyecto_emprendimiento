# Caso de uso: Consultar servicio
## Actores: Usuario (Administrador)
## Precondiciones:
Deben existir servicios registrados en el sistema.

## Camino Básico:
1. El usuario accede al módulo de servicios.
2. El sistema obtiene la lista de servicios registrados.
3. El sistema muestra los servicios con sus datos (nombre, costo).
4. El usuario visualiza la información de los servicios.

## Caminos Alternativos:

3. 1. Sin servicios registrados
        1. El sistema no encuentra servicios registrados.
        2. El sistema muestra un mensaje: "No hay servicios registrados".
        3. El usuario puede optar por crear un nuevo servicio.

    2. Error al cargar los servicios
        1. El sistema no puede obtener los datos.
        2. El sistema muestra un mensaje: "No fue posible cargar los servicios".
        3. El sistema ofrece la opción de reintentar la operación.

## Postcondiciones:
El usuario visualiza el listado de servicios disponibles.

## Escenarios de Éxito:
El usuario accede correctamente y visualiza todos los servicios registrados.

## Escenarios de Fracaso:
1. No existen servicios en el sistema.
2. Ocurre un error al cargar los datos.