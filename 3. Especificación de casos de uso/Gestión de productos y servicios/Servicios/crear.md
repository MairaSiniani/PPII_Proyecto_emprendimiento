# Caso de uso: Crear servicio
## Actores: Usuario (Administrador)
## Precondiciones:

El usuario debe haber iniciado sesión en el sistema.
##  Camino Básico:

1. El usuario accede al módulo de Servicios
2. El sistema muestra los servicios registrados y los botones para realizar operaciones.
3. El usuario selecciona la opción “Nuevo servicio".
4. El sistema muestra el formulario de creación de servicios.
5. El usuario ingresa los datos: nombre, detalles, costo y confirma el registro.
6. El sistema valida los datos ingresados, guarda el servicio y muestra un mensaje de confirmación.

## Caminos Alternativos:

5. 1.  Cancelación del registro
        1. El usuario cancela la operación.
        2.  El sistema no guarda el servicio y vuelve al paso 2.

6. 1. Datos incompletos
        1. El sistema detecta campos obligatorios vacíos y muestra un mensaje: "Debe completar todos los campos obligatorios".
        3. El usuario vuelve al paso 5.

    2. Datos inválidos
        1. El sistema detecta valores incorrectos y muestra un mensaje: "Datos inválidos".
        3. El usuario vuelve al paso 4.

## Postcondiciones:
El servicio queda registrado en el sistema.

## Escenarios de Éxito:
El usuario registra correctamente un servicio y el sistema lo almacena.

## Escenarios de Fracaso:
1. El usuario ingresa datos incompletos o inválidos.
2. El sistema impide el registro y muestra un mensaje de error.