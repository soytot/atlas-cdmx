# Atlas CDMX 1911 a 2026

Prototipo de atlas histórico interactivo de la Ciudad de México.

- `index.html`: mapa (Leaflet + OpenStreetMap).
- `data/zm_main_roads.geojson`: 23,528 tramos de vialidad principal de la zona metropolitana, geometría de OpenStreetMap (ODbL), con año, tipo, quién y confianza cuando ya están fechados.
- `data/polanco_streets.geojson`: 1,086 tramos de Polanco y alrededores, fechados por sección de fraccionamiento (por verificar con planos).

Publicar: subir esta carpeta a un repositorio de GitHub y activar Pages (Settings, Pages, Deploy from branch, main, root).

## Datos

- `data/mancha.geojson`: límite urbano de 1990, 2000 y 2014, Atlas of Urban Expansion 2016 (NYU, Lincoln Institute, UN-Habitat), reproyectado a WGS84 y simplificado.

## Pendientes

- Mancha urbana antes de 1990 (planos históricos o el dataset histórico del Atlas 2012, cuyo enlace público no aparece).
- Fechar el resto de las vías principales (8,843 de 23,528 al 29 oct 2026).
- Polanco: verificar fechas por calle contra los planos de 1929, 1941 y 1952.
- Mapa base propio dibujado con la red de OSM.
