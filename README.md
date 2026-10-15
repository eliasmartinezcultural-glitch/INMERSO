# INMERSO — San Patricio del Chañar

Proyecto de exploración cartográfica e inmersiva del casco urbano y el entorno rural de San Patricio del Chañar, Neuquén.

## Estado

- **Fase 1 — Investigación:** inventario inicial de fuentes y requisitos consolidado; la cobertura real de capas específicas sigue pendiente de inspección.
- **Fase 2 — Construcción:** iniciada con una primera interfaz web interactiva.
- **Fase 3 — Auditoría:** pendiente.

## Qué contiene la versión 0.1

- Mapa base interactivo con OpenStreetMap.
- Búsqueda manual de lugares mediante Nominatim.
- Atajos para cambiar el encuadre y volver a la vista inicial.
- Avisos explícitos sobre las capas locales aún no integradas.
- Atribución visible de OpenStreetMap.
- Diseño adaptable a computadora y teléfono.

## Qué NO contiene todavía

- Una base geográfica local completa.
- Un inventario validado de calles, parcelas, edificios o caminos rurales.
- Polígonos verificados de chacras, viñedos o arboledas.
- Modelos de edificios o terreno en 3D.
- Un modo totalmente offline.
- Una auditoría real de funcionamiento en todos los navegadores y dispositivos.

Las coordenadas iniciales del mapa son un **encuadre aproximado para comenzar la exploración**, no un límite administrativo oficial ni una declaración de precisión geodésica.

## Fuentes de investigación

### OpenStreetMap
- Mapa: https://www.openstreetmap.org/
- Licencia y atribución: https://www.openstreetmap.org/copyright
- Descargas Argentina (Geofabrik): https://download.geofabrik.de/south-america/argentina.html
- Uso previsto: calles, caminos, objetos etiquetados y puntos de interés, sujetos a comprobación de cobertura y licencia ODbL.
- Precaución: el mapa base y el servicio de búsqueda son servicios externos; pueden fallar, limitar solicitudes o entregar datos incompletos. No copiar imágenes de otros proveedores sin revisar sus condiciones.

### IDENEU / Catálogo geoespacial provincial
- Portal: https://catalogo.neuquen.gov.ar/portal/
- Catálogo IDENEU: https://ideneu.neuquen.gov.ar/geonetwork/srv/eng/catalog.search
- Sistema de geovisualización SiGGeS: https://optic.neuquen.gov.ar/sigges/
- Uso de investigación: localizar capas y metadatos relacionados con recursos hídricos, vialidad, catastro, educación, producción e infraestructura.
- Pendiente: identificar capas que cubran específicamente San Patricio del Chañar, registrar metadatos, formatos, fecha y permiso de reutilización. La presencia de un geoservicio no equivale automáticamente a permiso para descargar, redistribuir o empaquetar sus datos.

### Catastro provincial
- Mapoteca Digital: https://dpc.neuquen.gov.ar/Mapa
- Uso de investigación: referencia cartográfica.
- Restricción: el sitio informa condiciones restrictivas sobre reproducción de mapas. No integrar mapas, imágenes o datos derivados sin aclarar autorización y condiciones aplicables.

### Datos abiertos provinciales
- Catálogo geoespacial de Estadística y Censos: https://www.estadisticaneuquen.gob.ar/apps/catalogo_geoespacial/
- Portal de datos abiertos: https://portaldatosabiertos.neuquen.gov.ar/
- Uso de investigación: buscar capas descargables y metadatos; revisar la licencia en cada conjunto por separado.

### GitHub Pages
- Qué es: https://docs.github.com/es/pages/getting-started-with-github-pages/what-is-github-pages
- Límites: https://docs.github.com/es/pages/getting-started-with-github-pages/github-pages-limits
- Decisión provisional: mantener una web estática, sin backend propio, mientras los requisitos y el volumen de datos lo permitan.

## Registro de capas pendientes

| Capa | Qué se necesita | Estado |
|---|---|---|
| Calles y cruces urbanos | Geometrías, nombres, conectividad y fecha | Pendiente de medir cobertura |
| Manzanas y parcelas | Fuente autorizada y geometría utilizable | Pendiente; no dibujar por inferencia |
| Edificios | Huellas, nombres, alturas si existen y permiso | Pendiente |
| Rutas y caminos rurales | Trazados, accesos y conectividad | Pendiente de comparar fuentes |
| Río y drenajes | Capa hidrográfica con procedencia y fecha | Pendiente |
| Chacras, viñedos y arboledas | Datos autorizados y delimitación verificable | Pendiente |
| Instituciones y puntos de interés | Nombre, ubicación, tipo y fuente | Pendiente |
| Elevación/terreno 3D | Datos de elevación, resolución y licencia | Pendiente |
| Fotografías/texturas | Autoría, licencia y área representada | Pendiente |

## Reglas de calidad

1. No presentar un lugar como confirmado solo porque aparece en un buscador.
2. Cada capa debe tener fuente, fecha de consulta, licencia y observaciones.
3. Marcar por separado: **verificado**, **parcial**, **pendiente** y **descartado**.
4. No afirmar que edificios, parcelas o caminos son exactos sin cotejarlos.
5. Mantener visible la atribución de fuentes cartográficas.
6. No guardar credenciales, datos personales sensibles ni secretos en el repositorio.
7. No prometer modo offline hasta empaquetar y probar los recursos necesarios.

## Pruebas pendientes para v0.1

- Abrir la página publicada en computadora y móvil.
- Confirmar que Leaflet y los mosaicos cartográficos cargan.
- Probar búsqueda con resultados, sin resultados y sin conexión.
- Revisar atribución visible y enlaces.
- Comprobar el diseño a 320, 390, 680 px y escritorio.
- Evaluar tiempos de carga, errores de consola y respuesta de los servicios externos.

## Próximos pasos de fase 2

1. Verificar la publicación de GitHub Pages.
2. Probar la base interactiva y corregir errores de interfaz.
3. Inspeccionar y seleccionar datos concretos de OSM y catálogos provinciales.
4. Incorporar únicamente capas autorizadas y con procedencia registrada.
5. Evaluar el 3D después de tener una base cartográfica verificable.

**Créditos:** INMERSO es un proyecto independiente. Mapa base y datos cartográficos sujetos a la atribución indicada por OpenStreetMap. La disponibilidad de fuentes externas no implica afiliación institucional.
