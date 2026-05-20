# Caso de uso: Consultar Historial de Ventas
## Actores: Usuario 
## Precondiciones:
Debee existir al menos una venta registrada.

## Camino Básico:
1. El usuario accede al módulo de ventas.
2. El sistema obtiene el historial de ventas con: fecha, total, medio de pago.
3. El usuario selecciona una venta.
4. El sistema muestra el detalle: ítems, cantidades.

## Caminos Alternativos:

2. 1. Sin ventas registradas
        1. El sistema muestra: "No hay ventas registradas".

    2. Error al cargar datos
        1. El sistema muestra: "No fue posible cargar las ventas".

## Postcondiciones:
-

## Escenarios de Éxito:
El usuario visualiza el historial de las ventas realizadas.

## Escenarios de Fracaso:
No hay ventas 
No pueden visualizarse