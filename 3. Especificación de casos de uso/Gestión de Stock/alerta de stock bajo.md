# Caso de uso: generar alerta de stock bajo
## Actores: sistema

## Precondiciones:

Deben existir al menos un material registrado en el sistema. Cada material debe tener definido un nivel mínimo de stock.

# Camino Básico:
1. El sistema monitorea periódicamente el stock de materiales.
2. El sistema compara la cantidad disponible de cada material con su nivel mínimo.
3. El sistema detecta materiales con stock menor o igual al mínimo establecido.
4. El sistema genera una alerta de stock bajo.
5. El sistema muestra la alerta al usuario (notificación o indicador visual).
6. El usuario visualiza los materiales con bajo stock.

## Caminos Alternativos:

3. 1. Sin materiales con stock bajo
        1. El sistema no detecta materiales por debajo del mínimo.
        2. El sistema no genera alertas.

    2. Error en la verificación
        1. El sistema no puede verificar los niveles de stock.
        2. El sistema registra el error.
        3. El sistema muestra un mensaje: "No fue posible verificar el stock".

    3. Material sin stock mínimo definido
        1. El sistema detecta materiales sin nivel mínimo configurado.
        2. El sistema ignora esos materiales.

## Postcondiciones:
El usuario es informado sobre materiales con bajo stock.

## Escenarios de Éxito:
1. El sistema detecta correctamente materiales con bajo stock y alerta al usuario.
2. El usuario puede actuar a tiempo para reponer materiales.

## Escenarios de Fracaso:
1. El sistema no puede verificar el stock.
2. No se generan alertas cuando deberían.