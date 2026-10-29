# Atlas CDMX 1911 a 2026

Prototipo de atlas histórico interactivo de la Ciudad de México.

- `index.html`: mapa (Leaflet + OpenStreetMap).
- `data/zm_main_roads.geojson`: 23,528 tramos de vialidad principal de la zona metropolitana, geometría de OpenStreetMap (ODbL), con año, tipo, quién y confianza cuando ya están fechados.
- `data/polanco_streets.geojson`: 1,086 tramos de Polanco y alrededores, fechados por sección de fraccionamiento (por verificar con planos).

Publicar: subir esta carpeta a un repositorio de GitHub y activar Pages (Settings, Pages, Deploy from branch, main, root).

## Datos

- `data/mancha.geojson`: límite urbano de 1911 (trazado a mano sobre el plano de 1911 georreferenciado, 27.4 km², coincide con los 27 km² que da Unikel para 1910; aproximado a 100 o 200 m) y de 1990, 2000 y 2014 (Atlas of Urban Expansion 2016, NYU, Lincoln Institute, UN-Habitat), reproyectados a WGS84 y simplificados.

- `data/plano_1911.webp` y `.json`: Plano de la Ciudad de México de 1911 (Compañía Litográfica y Tipográfica), colección David Rumsey, georreferenciado con cuatro puntos de control (Zócalo, Castillo de Chapultepec, Columna de la Independencia, Alameda; error de 2 a 26 m) y reproyectado norte arriba con transparencia fuera del plano.
- `data/polanco_verificacion.csv`: tabla de trabajo para fechar Polanco calle por calle contra los planos de 1911, 1929, 1941 y 1952.

- `data/colonias.json`: 78 colonias, conjuntos y equipamientos con coordenada, año, tipo, quién, por qué y cronología local (texto del expediente del periodo; por contrastar con fuentes primarias).

## Pendientes

- Mancha urbana de 1930, 1950 y 1970: trazar sobre los planos de 1929, 1941 y 1952 cuando estén, igual que se hizo con el de 1911.
- Fechar el resto de las vías principales (10,176 de 23,528 al 29 oct 2026; lo que falta son sobre todo avenidas de municipios conurbados y nombres repetidos).
- Polanco: verificar fechas por calle contra los planos de 1929, 1941 y 1952 (Mapoteca Orozco y Berra; no accesible desde el entorno de Claude, hay que descargarlos a mano). El de 1911 ya está en el mapa.
- Mapa base propio dibujado con la red de OSM.
