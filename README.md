# Examen práctico — Herramientas de Software en la Nube

## Objetivo del proyecto

Desplegar una aplicación web utilizando Docker y Docker Compose, administrar el código mediante Git y GitHub, y elaborar un dashboard para visualizar datos de ventas, clientes y pedidos.

## Imagen utilizada

La imagen personalizada del proyecto es:

`examen:217O03055`

Se construye a partir de `Dockerfile` utilizando Nginx como servidor web.

## Puertos

La aplicación se publica en tres servicios:

- Servicio 1: http://localhost:8081
- Servicio 2: http://localhost:8082
- Servicio 3: http://localhost:8083

## Cómo levantar los servicios

Desde la carpeta principal del proyecto, ejecutar:

```bash
docker compose up -d
```

Para comprobar su estado:

```bash
docker compose ps
```

Para detener los servicios:

```bash
docker compose down
```

## Estructura del proyecto

- `web/`: archivos de la aplicación web.
- `Dockerfile`: instrucciones para construir la imagen.
- `compose.yaml`: definición de los tres servicios.
- `visualizacion/`: datos y archivos del dashboard.
- `evidencias/`: capturas del examen.

## Visualización

El proyecto incluirá un dashboard con las ventas por mes, los clientes por mes, las ventas totales, el promedio de pedidos y el mes con mayores ventas. La herramienta utilizada se documentará cuando se complete esta actividad.