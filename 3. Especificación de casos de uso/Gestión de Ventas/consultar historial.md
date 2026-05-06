# Caso de uso: Consultar Historial de Ventas
## Actores: Usuario 
## Precondiciones:
Debee existir al menos una venta registrada.

## Camino Básico:
1. El usuario accede al módulo de ventas.
2. El sistema obtiene el historial de ventas.
3. El sistema muestra la lista con: fecha, total, medio de pago.
4. El usuario selecciona una venta.
5. El sistema muestra el detalle: ítems, cantidades.

## Caminos Alternativos:

2. 1. Sin ventas registradas
        1. El sistema muestra: "No hay ventas registradas".

    2. Error al cargar datos
        1. El sistema muestra: "No fue posible cargar las ventas".

## Postcondiciones:
El usuario visualiza el historial de ventas.

## Escenarios de Éxito:
El usuario consulta correctamente las ventas realizadas.

## Escenarios de Fracaso:
No hay ventas o error del sistema.