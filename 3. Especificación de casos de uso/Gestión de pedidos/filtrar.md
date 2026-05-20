# Caso de uso: Filtrar Pedidos
## Actores: Usuario 
## Precondiciones:
Deben existir pedidos registrados.

## Camino Básico:
1. El usuario accede al módulo de pedidos.
2. El sistema muestra la lista completa de pedidos.
3. El usuario ingresa uno o más criterios de filtrado: estado (pendiente, en proceso, terminado, entregado) o fecha y aplica el filtro.
4. El sistema muestra los pedidos que cumplen con las condiciones.
5. El usuario visualiza los resultados filtrados.

## Caminos Alternativos:
4. 1. Filtros vacíos
        1. El usuario no ingresa ningún filtro.
        2. El sistema muestra la lista completa de pedidos.

5. 1. Sin resultados
        1. El sistema no encuentra pedidos que coincidan y muestra un mensaje "No se encontraron pedidos".
        2. El usuario vuelve al paso 3.

## Postcondiciones:
Se muestra una lista filtrada de pedidos según los criterios seleccionados.

## Escenarios de Éxito:
El usuario encuentra rápidamente los pedidos que necesita gestionar.

## Escenarios de Fracaso:
1. No hay coincidencias.
2. No hay filtros