# FOODTEX · Propuesta digital actual

Sitio estático en HTML, CSS y JavaScript. El código editable está directamente en `dist/`; el nombre de esa carpeta no implica que exista una compilación previa.

## Uso local

Desde esta carpeta:

```sh
cd dist
python3 -m http.server 8080
```

Abrir http://localhost:8080/. Servir por HTTP permite que los recursos se carguen correctamente.

## Archivos principales

- `dist/index.html`: entrada y orden de carga de estilos y scripts.
- `dist/app.js`: vistas, navegación e interacciones.
- `dist/data.js`: productos, publicaciones y contenido inicial.
- `dist/*.css`: estilos y ajustes de la dirección visual actual.
- `dist/assets/`: fotografías, logos, catálogos PDF y videos.
- `docs/`: reportes de diseño, capturas y validación responsive.

Mantener el orden de las hojas de estilo definido en `index.html`.

## Rutas

Inicio `#/`, productos `#/productos`, nosotros `#/nosotros`, novedades `#/novedades`, contacto `#/contacto`, cotización `#/cotizacion` y administrador `#/admin`.

## Administrador y formularios

El panel administra una copia local de los datos mediante `localStorage`. No tiene autenticación ni almacenamiento compartido y no es un CMS de producción. Los cambios de un navegador no se sincronizan con otros usuarios. Los formularios registran consultas locales; no envían emails. Para producción se requiere implementar servicios de autenticación, persistencia y envío de consultas.

## Procedencia

La información de productos y novedades procede de https://foodtex.com.ar/ y sus catálogos. Se incluyen los recursos empleados en la propuesta actual y la documentación de sus mejoras. Se conserva el diseño y la funcionalidad existentes.
