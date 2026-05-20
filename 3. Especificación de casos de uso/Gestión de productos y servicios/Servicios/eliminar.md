# Caso de uso: Eliminar servicio
## Actores: Usuario (Administrador)
## Precondiciones:
Debe existir al menos un servicio registrado.

## Camino Básico:
1. El usuario accede al módulo de servicios.
2. El sistema muestra la lista de servicios.
3. El usuario selecciona un servicio.
4. El sistema muestra el detalle del servicio.
5. El usuario elige la opción “Eliminar”.
6. El sistema solicita confirmación.
7. El usuario confirma la eliminación.
8. El sistema elimina el servicio, actualiza la lista y muestra un mensaje de confirmación.

## Caminos Alternativos:

7. 1. Cancelación de eliminación
        1. El usuario cancela la operación.
        2. El sistema no elimina el servicio.

8. 1. Error al eliminar
        1. El sistema no puede eliminar el servicio, muestra un mensaje: "No fue posible eliminar el servicio" y mantiene el servicio sin cambios.

## Postcondiciones:
El servicio es eliminado del sistema.

## Escenarios de Éxito:
El usuario elimina correctamente un servicio y el sistema actualiza la lista.
##  Escenarios de Fracaso:
1. Ocurre un error al eliminar el servicio.
2. El sistema muestra el mensaje correspondiente.