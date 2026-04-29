# Caso de uso: Eliminar servicio
## Actores: Usuario (Administrador)
## Precondiciones:
Debe existir al menos un servicio registrado.

## Camino Básico:
1. El usuario accede al módulo de servicio.
2. El sistema muestra la lista de servicio.
3. El usuario selecciona un servicio.
4. El usuario elige la opción “Eliminar”.
5. El sistema solicita confirmación.
6. El usuario confirma la eliminación.
7. El sistema elimina el servicio.
8. El sistema actualiza la lista de servicios.
9. El sistema muestra un mensaje de confirmación.

## Caminos Alternativos:

6. 1. Cancelación de eliminación
        1. El usuario cancela la operación.
        2. El sistema no elimina el servicio.

7. 1. Error al eliminar
        1. El sistema no puede eliminar el servicio.
        2. El sistema muestra un mensaje: "No fue posible eliminar el servicio".
        3. El sistema mantiene el servicio sin cambios.

## Postcondiciones:
El servicio es eliminado del sistema.

## Escenarios de Éxito:
El usuario elimina correctamente un servicio y el sistema actualiza la lista.
##  Escenarios de Fracaso:
1. Ocurre un error al eliminar el servicio.
2. El sistema muestra el mensaje correspondiente.