# Caso de uso: Eliminar Material

# Actores: Usuario (administrador)

# Precondiciones:

El usuario debe haber iniciado sesión. Debe existir al menos un material registrado.

## Camino básico:
1. El usuario accede al listado de materiales.
2. El sistema muestra los materiales disponibles.
3. El usuario selecciona un material.
4. EL usuario elige la opción "Eliminar".
5. El sistema solicita confirmación.
6. EL usuaruo confirma la eliminación
7. EL sistema elimina el material.
8. El sistema actualiza el listado.
9. El sistema muestra un mensaje de confirmación.

## Caminos Alternativos:

6. 1. Cancelación de la eliminación
        1. El usuario cancela la operación.
        2. El sistema no elimina el material.

## Postcondiciones:
El material es eliminado del sistema.

## Escenarios de Éxito:
El usuario elimina correctamente un material y el sistema actualiza el stock.

## Escenarios de Fracaso:
1. El sistema no puede eliminar el material.
2. Ocurre un error y se muestra un mensaje al usuario.