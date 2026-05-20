# Caso de uso: Modificar Material
## Actores: Usuario (Administrador)
## Precondiciones:
Debe existir al menos un material registrado en el sistema.

## Camino Básico:
1. El usuario accede al listado de materiales.
2. El sistema muestra los materiales disponibles.
3. El usuario selecciona un material y elige la opción “Modificar”.
4. El sistema muestra los datos actuales del material.
5. El usuario edita los campos (nombre, tipo, característica, cantidad, precio, categoría) y confirma los cambios.
6. El sistema valida los datos ingresados, actualiza la información del material y muestra un mensaje de confirmación.

## Caminos Alternativos:

7. 1. Cancelación de modificación
        1. El usuario cancela la operación.
        2. El sistema no guarda cambios y vuelve al listado.

8. 1. Datos inválidos
        1. El sistema detecta datos incorrectos.
        2. El sistema muestra un mensaje de error.
        3. El usuario corrige los datos y vuelve al paso 6.

## Postcondiciones:
El material queda actualizado en el sistema.

## Escenarios de Éxito:
El usuario modifica correctamente un material y los cambios se guardan.

## Escenarios de Fracaso:
1. El usuario ingresa datos inválidos
2. El sistema impide la modificación y muestra error.