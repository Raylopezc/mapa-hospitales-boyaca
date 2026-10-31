# C3 – Mapa de Hospitales de Boyacá

## Descripción
Aplicación cartográfica web desarrollada con Leaflet 1.9.4 y JavaScript para visualizar establecimientos hospitalarios del departamento de Boyacá mediante un servicio geográfico de ArcGIS.

## Funcionalidades implementadas
- Visualización de entidades puntuales sobre el mapa base Esri World Street Map.
- Consulta de entidades mediante ArcGIS FeatureServer.
- Ventanas emergentes con los atributos `Nombre` y `NOM_MPIO`.
- Buscador textual por coincidencias en nombre del hospital o municipio.
- Ajuste de la extensión del mapa a los resultados de búsqueda.
- Control con el total de entidades cargadas.
- Leyenda cartográfica y ficha de información.

## Fuentes y tecnologías
- Servicio de datos: `https://services6.arcgis.com/Ex2fmFOuTOHRZtML/ArcGIS/rest/services/Hospitales_Boyac%C3%A1/FeatureServer/0`
- Consulta GeoJSON: `https://services6.arcgis.com/Ex2fmFOuTOHRZtML/ArcGIS/rest/services/Hospitales_Boyac%C3%A1/FeatureServer/0/query?where=1%3D1&outFields=*&outSR=4326&f=geojson`
- Leaflet 1.9.4: biblioteca de mapas web.
- Esri World Street Map: mapa base.

## Ejecución local
1. Abrir `index.html` en un navegador con conexión a Internet.
2. Permitir la carga de los recursos externos de Leaflet, el mapa base y el servicio ArcGIS.
3. Usar el buscador y seleccionar los marcadores para consultar sus atributos.

## Validaciones realizadas
- Se observaron 464 entidades cargadas en la aplicación.
- Se comprobó la visualización de los marcadores y las ventanas emergentes.
- Se verificó la presencia del buscador, la leyenda y la ficha informativa.
- La búsqueda es textual: compara lo escrito con los campos `Nombre` y `NOM_MPIO`. Por ello, los resultados deben interpretarse como coincidencias de texto, no como una consulta administrativa exacta del municipio.

## Publicación
**URL pública:** pendiente de publicación y verificación.

