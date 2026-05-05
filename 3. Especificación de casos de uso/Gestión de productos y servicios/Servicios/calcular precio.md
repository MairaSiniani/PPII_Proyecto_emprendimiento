# Caso de uso: Calcular precio de servicio
## Actores: Sistema, Usuario
## Precondiciones:
Debe existir un servicio registrado.
El servicio debe tener definido su costo (basado en tarifas oficiales).

## Camino Básico:
1. El usuario accede al módulo de servicios.
2. El usuario selecciona un servicio.
3. El usuario solicita calcular el precio.
4. El sistema obtiene el costo del servicio.
5. El usuario ingresa la cantidad de horas de trabajo estimadas.
6. El sistema calcula costo * cantidad de horas.
7. El sistema muestra el precio calculado al usuario.
8. El sistema permite guardar el precio como precio de venta del servicio.

## Caminos Alternativos:

6. 1. Datos incompletos
        1. Falta precio por hora o cantidad de horas.
        2. El sistema solicita completar los datos.

    2. Datos inválidos
        1. Valores negativos o incorrectos.
        2. El sistema muestra error.

    3. Error en cálculo
        1. El sistema no puede calcular.
        2. Muestra mensaje de error.

## Postcondiciones:
1. El precio del servicio queda calculado.

## Escenarios de Éxito:
1. El sistema calcula correctamente el precio.
2. El usuario obtiene un precio adecuado para no perder dinero.

## Escenarios de Fracaso:
1. Falta información (costo o cantidad de horas).
2. Ocurre un error en el cálculo.