# 🗺️ pba-educacion: Interfaz Cartográfica Interactiva de la Dimensión Educativa (PBA)

¡Bienvenidos al repositorio oficial de **pba-educacion**! Este espacio aloja la capa de presentación visual para la exploración, visualización y análisis geoespacial del nivel educativo predominante a nivel municipal dentro de la Provincia de Buenos Aires, República Argentina.

El objetivo de esta herramienta es transformar matrices complejas de datos tabulares en una representación coroplética analítica de alta precisión, facilitando la identificación de patrones de desarrollo humano y educativo mediante una experiencia de usuario fluida, estática e interactiva.

---

## 📊 Fuentes de Datos Certificadas

Para garantizar la máxima rigurosidad y validez metodológica, la base de información se nutre exclusivamente de registros públicos y capas vectoriales oficiales de la República Argentina:

* **Dirección Provincial de Estadística (DPE - Buenos Aires):** Cartografía base y delimitaciones vectoriales oficiales correspondientes a los 135 municipios bonaerenses, asegurando la correspondencia geométrica y la integridad territorial histórica.
* **INDEC (Instituto Nacional de Estadística y Censos):** Registros consolidados que incluyen poblaciones totales, códigos jurisdiccionales y estructuras de gobiernos locales.

---

## 🛠️ Procesamiento y Pipeline Tecnológico (Backend Privado)

Aunque este repositorio almacena únicamente el entregable estático final para su consumo web, la suite de datos subyacente ha sido compilada nativamente mediante ingeniería de datos en Python:

* **GeoPandas:** Procesamiento y re-proyección analítica desde el sistema métrico oficial de origen (**POSGAR 94 Faja 5 / EPSG:22185**) hacia la proyección web estándar (WGS84 / EPSG:4326).
* **Pandas & Unicodedata:** Motor analítico encargado del cruce de datos (*merge*), normalización de nomenclaturas y estandarización lingüística distribuida para mitigar fallas de consistencia en los 135 partidos.
* **Folium:** Renderizado geoespacial basado en la biblioteca JavaScript Leaflet, optimizado sobre capas base de alta legibilidad (*CartoDB Positron*).

---

## 🔍 Características Principales de la Interfaz

* **Mapeo Temático Cualitativo:** Visualización coroplética que diferencia los municipios según su *Nivel Educativo Predominante* (distinguiendo entornos de educación secundaria de los grandes nodos universitarios y superiores).
* **Tooltips Multicapa Premium:** Cuadros flotantes interactivos de alta densidad informativa con estilos CSS personalizados. Al desplazar el cursor sobre cualquier municipio, el tablero despliega instantáneamente:
    1. **Identificación:** Nombre Oficial del Municipio y Código INDEC Único.
    2. **Dimensión Territorial:** Superficie real calculada vectorialmente ($km^2$) y coordenadas geográficas de su centroide de precisión.
    3. **Indicadores Urbanos:** Configuración territorial (mixto, urbano, rural) y estado de inserción en el Área Metropolitana (AMBA).
    4. **Métricas Demográficas:** Población Total, Densidad Poblacional (hab/km²) y acceso al Sitio Web Oficial de la jurisdicción.

---

## 🌐 Despliegue

La capa de presentación visual de este proyecto se encuentra configurada para su compilación estática nativa (`index.html`), permitiendo su alojamiento automático en entornos distribuidos como **GitHub Pages** para una accesibilidad multiplataforma óptima.

---
*Desarrollado bajo criterios de rigor técnico y automatización de pipelines de datos territoriales.*
