# Caso de uso: generar alerta de stock bajo
## Actores: sistema

## Precondiciones:

Deben existir al menos un material registrado en el sistema. Cada material debe tener definido un nivel mínimo de stock.

# Camino Básico:
1. El sistema monitorea periódicamente el stock de materiales.
2. El usuario hace uso de los materiales cuando registra algún pedido. 
3. El sistema resta los materiales usados del stock, detecta los materiales con stock menor o igual al mínimo establecido y genera una alerta de stock bajo (notificación o indicador visual).
4. El usuario visualiza los materiales con bajo stock.

## Caminos Alternativos:

3. 1. Sin materiales con stock bajo
        1. El sistema no detecta materiales por debajo del mínimo y no genera alertas.

    3. Material sin stock mínimo definido
        1. El sistema detecta materiales sin nivel mínimo configurado y solicita al usuario agregarlo. 
        
## Postcondiciones:
El usuario es informado sobre materiales con bajo stock.

## Escenarios de Éxito:
1. El sistema detecta correctamente materiales con bajo stock y alerta al usuario.
2. El usuario puede actuar a tiempo para reponer materiales.

## Escenarios de Fracaso:
1. El sistema no puede verificar el stock.
2. No se generan alertas cuando deberían.