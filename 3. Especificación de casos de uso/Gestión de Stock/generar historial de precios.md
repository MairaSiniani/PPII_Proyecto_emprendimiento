# Caso de uso: Mantener historial de precios de los materiales
## Actores: Sistema (principal)
## Precondiciones:

Debe existir al menos un material registrado en el sistema.
El material debe tener un precio definido.

## Caminos Básicos:

1. El sistema monitorea los cambios en los datos de los materiales.
2. El usuario modifica el precio de un material.
3. El sistema detecta que el precio fue modificado.
4. El sistema registra automáticamente el precio anterior junto con la fecha del cambio en el historial.
5. El sistema actualiza el precio actual del material.
6. El sistema guarda la información.
7. El sistema muestra un mensaje de confirmación al usuario.

## Caminos Alternativos:

3. 1. Precio inválido
        1. El sistema detecta que el nuevo precio es incorrecto (negativo o vacío).
        2. El sistema muestra un mensaje: "Precio inválido".
        3. El usuario vuelve al paso 2.

6. 1. Error al guardar historial
        1. El sistema no puede registrar el cambio de precio.
        2. El sistema muestra un mensaje: "No fue posible guardar el historial".
        3. El sistema no actualiza el precio hasta resolver el error.

## Postcondiciones:
1. El historial de precios queda actualizado automáticamente.
2. El nuevo precio del material queda registrado como precio actual.

## Escenarios de Éxito:
El sistema detecta correctamente cambios de precio y los registra sin intervención manual.

## Escenarios de Fracaso:
1. El sistema no puede registrar el historial.
2. Se intenta ingresar un precio inválido.