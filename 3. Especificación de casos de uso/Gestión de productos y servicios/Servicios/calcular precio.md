# Caso de uso: Calcular precio de servicio
## Actores: Sistema, Usuario
## Precondiciones:
Debe existir un servicio registrado.
El servicio debe tener definido su costo (basado en tarifas oficiales).

## Camino Básico:
1. El usuario accede al módulo de servicios.
2. El sistema muestra los servicios registrados.
3. El usuario selecciona uno y solicita calcular el precio.
4. El sistema obtiene el costo del servicio y solicita al usuario ingresar la cantidad de horas de trabajo requeridas.
5. El usuario ingresa la cantidad de horas de trabajo estimadas.
6. El sistema calcula costo * cantidad de horas.
7. El sistema muestra el precio calculado al usuario.
8. El usuario selecciona "Guardar".
9. El sistema guarda el precio del servicio.

## Caminos Alternativos:

6. 1. Datos incompletos
        1. El sistema solicita completar los datos.
        2. El usuario vuelve al paso 5.

    2. Datos inválidos
        1. El sistema detecta valores negativos o incorrectos y muestra error.
        2. El usuario vuelve al paso 5.

8. 1. El usuario no selecciona guardar.
        1. El sistema no guarda el precio del servicio.

## Postcondiciones:
1. El precio del servicio queda calculado y registrado.

## Escenarios de Éxito:
1. El sistema calcula correctamente el precio.
2. El usuario obtiene un precio adecuado para no perder dinero.

## Escenarios de Fracaso:
1. Falta información (costo o cantidad de horas).
2. No se guarda el precio calculado. 