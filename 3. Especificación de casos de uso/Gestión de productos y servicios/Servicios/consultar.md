# Caso de uso: Consultar servicio
## Actores: Usuario (Administrador)
## Precondiciones:
Deben existir servicios registrados en el sistema.

## Camino Básico:
1. El usuario accede al módulo de servicios.
2. El sistema obtiene la lista de servicios registrados con sus datos (nombre, costo).
3. El usuario visualiza los servicios y selecciona uno.
4. El sistema muestra los detalles del servicio.

## Caminos Alternativos:

3. 1. Sin servicios registrados
        1. El sistema no encuentra servicios registrados y muestra un mensaje: "No hay servicios registrados".
        3. El usuario puede optar por crear un nuevo servicio.

    2. Error al cargar los servicios
        1. El sistema no puede obtener los datos, muestra un mensaje: "No fue posible cargar los servicios" y ofrece la opción de reintentar la operación.

## Postcondiciones:
El usuario visualiza el detalle del producto elegido.

## Escenarios de Éxito:
El usuario accede correctamente y visualiza todos los servicios registrados y el detalle de los seleccionados.

## Escenarios de Fracaso:
1. No existen servicios en el sistema.
2. Ocurre un error al cargar los datos.