# Proyectos FOODTEX

Código de la versión actual de la propuesta digital de FOODTEX.

## Organización

- `foodtex/dist/`: código fuente estático y todos los recursos del sitio. No requiere compilación.
- `foodtex/docs/`: documentación de diseño y validación visual.
- `foodtex/README.md`: instrucciones y alcance funcional.

El segundo proyecto se incorporará en una carpeta independiente cuando esté identificado.

## Ejecutar FOODTEX

Con Python 3 instalado:

```sh
git clone https://github.com/lihuensg/foodtex.git
cd foodtex/foodtex/dist
python3 -m http.server 8080
```

Abrir http://localhost:8080/ en el navegador. En Windows también se puede usar `py -m http.server 8080`.

## Publicar

La carpeta pública es `foodtex/dist`. Puede alojarse en cualquier servicio de hosting estático. Las rutas utilizan hash (`#/productos`, `#/nosotros`, etc.). No necesita un servidor de aplicaciones.

## Alcance

El administrador es una demostración sin autenticación: guarda cambios en `localStorage` del navegador, no en una base de datos compartida. Los formularios guardan consultas de demostración; no envían correos. Los enlaces de contacto y cotización mantienen el comportamiento de la propuesta.

No se incluye una licencia abierta para el código ni para las fotografías, videos, logos o catálogos. La visibilidad pública del repositorio no modifica los derechos sobre esos materiales.
