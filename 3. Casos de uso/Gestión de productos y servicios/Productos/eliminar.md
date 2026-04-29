# Caso de uso: Eliminar Producto
## Actores: Usuario (Administrador)
## Precondiciones:
Debe existir al menos un producto registrado.

## Camino Básico:
1. El usuario accede al módulo de productos.
2. El sistema muestra la lista de productos.
3. El usuario selecciona un producto.
4. El usuario elige la opción “Eliminar”.
5. El sistema solicita confirmación.
6. El usuario confirma la eliminación.
7. El sistema elimina el producto.
8. El sistema actualiza la lista de productos.
9. El sistema muestra un mensaje de confirmación.

## Caminos Alternativos:

6. 1. Cancelación de eliminación
        1. El usuario cancela la operación.
        2. El sistema no elimina el producto.

7. 1. Error al eliminar
        1. El sistema no puede eliminar el producto.
        2. El sistema muestra un mensaje: "No fue posible eliminar el producto".
        3. El sistema mantiene el producto sin cambios.

## Postcondiciones:
El producto es eliminado del sistema.

## Escenarios de Éxito:
El usuario elimina correctamente un producto y el sistema actualiza la lista.
##  Escenarios de Fracaso:
1. Ocurre un error al eliminar el producto.
2. El sistema muestra el mensaje correspondiente.