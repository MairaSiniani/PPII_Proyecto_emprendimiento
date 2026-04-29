# Caso de uso: filtrar Stock
## Actores: Usuario (Administrador)
## Precondiciones:
El usuario debe haber iniciado sesión en el sistema. Deben existir materiales registrados en el sistema.

# Camino Básico:

1. El usuario accede al módulo de stock.
2. El sistema muestra la lista de materiales disponibles.
3. El usuario ingresa uno o más criterios de filtrado (nombre, tipo o categoría).
4. El usuario aplica el filtro.
5. El sistema procesa los criterios ingresados.
6. El sistema muestra la lista de materiales que cumplen con los filtros aplicados.
7. El usuario visualiza los resultados filtrados.

## Caminos Alternativos:

5. 1. Sin resultados
        1. El sistema no encuentra materiales que coincidan con los criterios ingresados.
        2. El sistema muestra un mensaje: "No se encontraron materiales".
        3. El usuario puede modificar o limpiar los filtros.

    2. Error al aplicar filtros
        1. El sistema no puede procesar los criterios ingresados.
        2. El sistema muestra un mensaje de error: "No fue posible aplicar el filtro".
        3. El sistema ofrece la opción de reintentar.

## Postcondiciones:
El sistema muestra una lista de materiales filtrada según los criterios ingresados.

## Escenarios de Éxito:
El usuario aplica filtros correctamente y visualiza los resultados esperados.

## Escenarios de Fracaso:
1. No existen materiales que coincidan con los filtros.
2. Ocurre un error al procesar la búsqueda.
