# Caso de uso: Consultar Productos
## Actores: Usuario (Administrador)
## Precondiciones:
Deben existir productos registrados en el sistema.

## Camino Básico:
1. El usuario accede al módulo de productos.
2. El sistema obtiene la lista de productos registrados con sus datos (nombre, costo de producción, precio de venta, categoría y disponibilidad).
3. El usuario visualiza la información de los productos.

## Caminos Alternativos:

2. 1. Sin productos registrados
        1. El sistema no encuentra productos registrados y muestra un mensaje: "No hay productos registrados".
        2. El usuario puede optar por crear un nuevo producto.

    2. Error al cargar los productos
        1. El sistema no puede obtener los datos, muestra un mensaje: "No fue posible cargar los productos" y ofrece la opción de reintentar la operación.

## Postcondiciones:
El usuario visualiza el listado de productos disponibles.

## Escenarios de Éxito:
El usuario accede correctamente y visualiza todos los productos registrados.

## Escenarios de Fracaso:
1. No existen productos en el sistema.
2. Ocurre un error al cargar los datos.