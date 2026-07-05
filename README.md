# 🗺️ pba-map: Tablero Geográfico Interactivo de la Provincia de Buenos Aires

¡Bienvenidos al repositorio oficial de **pba-map**! Este proyecto constituye una interfaz cartográfica interactiva y dinámica diseñada para la visualización, exploración y análisis de variables estructurales, socioeconómicas y sociodemográficas a nivel municipal dentro de la Provincia de Buenos Aires, República Argentina.

El objetivo de esta herramienta es transformar matrices de datos tabulares en representaciones geoespaciales analíticas de alta precisión, facilitando la identificación de patrones territoriales mediante una experiencia de usuario fluida e informativa.

---

## 📊 Fuentes de Datos Certificadas

Para garantizar la máxima rigurosidad y validez metodológica, la base de información del mapa se nutre exclusivamente de registros públicos de organismos oficiales e institucionales de la República Argentina:

* **INDEC (Instituto Nacional de Estadística y Censos):** Datos definitivos provenientes del *Censo Nacional de Población, Hogares y Viviendas 2022*, incluyendo poblaciones totales por municipio, códigos jurisdiccionales y estructuras de gobiernos locales.
* **IGN (Instituto Geográfico Nacional):** Cartografía base y delimitaciones vectoriales oficiales para asegurar la correspondencia geométrica del territorio bonaerense.
* **DAMI (Desarrollo de Áreas Metropolitanas del Interior - Ministerio de Economía):** Criterios institucionales y normativos para la delimitación técnica precisa de las variables asociadas a la inserción urbana y funcional en el AMBA.

---

## 🛠️ Arquitectura y Tecnologías Utilizadas

Este ecosistema geográfico ha sido desarrollado e integrado de forma nativa utilizando herramientas de programación avanzadas de la suite de Ciencia de Datos de **Python**:

* **GeoPandas:** Procesamiento, proyección métrica oficial (Faja 4 / EPSG:5346) y manipulación analítica de capas vectoriales en formato GeoJSON.
* **Pandas:** Motor de backend encargado del cruce de datos (*merge*), limpieza textual distribuida (`unicodedata`) y estandarización de nomenclaturas municipales.
* **Folium:** Renderizado cartográfico interactivo basado en la biblioteca JavaScript Leaflet, configurado sobre capas estéticas optimizadas (*CartoDB Positron*).
* **OpenPyXL:** Sincronización automatizada en caliente con matrices complejas de hojas de cálculo.

---

## 🔍 Características Principales de la Interfaz

* **Mapeo Temático Coroplético:** Visualización de áreas diferenciadas por rangos cromáticos basados en variables clave como el *Nivel Educativo Predominante*.
* **Tooltips Multicapa Premium:** Cuadros flotantes interactivos de alta densidad informativa con estilos CSS personalizados. Al desplazar el cursor sobre cualquier municipio, el tablero despliega instantáneamente:
    1.  **Identificación:** Nombre Oficial del Municipio y Código INDEC Único.
    2.  **Dimensión Territorial:** Superficie calculada vectorialmente y coordenadas geográficas de su centroide.
    3.  **Indicadores Urbanos:** Estado de inserción institucional en el Área Metropolitana (AMBA) y enlaces a Sitios Web Oficiales.
    4.  **Métricas Demográficas:** Población Total y cálculo matemático derivado de la *Densidad Poblacional (hab/km²)*.

---

## 🌐 Despliegue

La capa de presentación visual de este proyecto se encuentra configurada para su compilación estática nativa (`index.html`), permitiendo su alojamiento automático en entornos distribuidos como **GitHub Pages** para una accesibilidad multiplataforma óptima.

---
*Desarrollado bajo criterios de rigor técnico y automatización de pipelines de datos territoriales.*
