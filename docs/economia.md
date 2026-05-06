# Caso de Uso 3: Actividad Económica Local

Conjuntos de datos relacionados con el caso de uso "Actividad Económica Local" en la ciudad de Santander.

## Información sobre los comercios, empresas y restaurantes de Santander

Información sobre los comercios, empresas y restaurantes de Santander.

??? info "Listados de comercios, empresas y restaurantes"
    * **Descripción:** Listados de las empresas, restaurantes y comercios (por tipología) de Santander, incluyendo su descripción, localización, horarios, teléfonos o redes sociales.
    * **Formato:** JSON
    * **Acceso:** Restringido
    * **Fuente:** Diario Montañés
    * **Endpoint:** <https://drive.google.com/file/d/1rNFL0eMOTt3lDP-Vu3i25SfvtbstGf31/view?usp=drive_link>
    

## Información sobre la actividad turística

Información sobre la actividad turística en la región, como el número de turistas por provincia.

??? info "Turismo interno interprovicial"
    * **Descripción:** Número de turistas por municipio de origen y destino. Medición del turismo interno interprovincial a partir de la posición de los teléfonos móviles.
    * **Formato:** CSV
    * **Acceso:** Abierto
    * **Fuente:** Instituto Nacional de Estadística (INE)
    * **Endpoint:** <https://www.ine.es/jaxiT3/files/t/csv_bdsc/53464.csv>

??? info "Turistas por Comunidad Autónoma"
    * **Descripción:** Número de turistas mensuales por CCAA de origen desagregados por municipio de destino.
    * **Formato:** CSV
    * **Acceso:** Abierto
    * **Fuente:** Instituto Nacional de Estadística (INE)
    * **Endpoint:** <https://www.ine.es/jaxiT3/files/t/csv_bdsc/53464.csv>

??? info "Turistas por Provincia"
    * **Descripción:** Número de turistas mensuales por Provincia de origen desagregados por municipio de destino.
    * **Formato:** CSV
    * **Acceso:** Abierto
    * **Fuente:** Instituto Nacional de Estadística (INE)
    * **Endpoint:** <https://www.ine.es/jaxiT3/files/t/csv_bdsc/53465.csv>

## Otros conjuntos de datos sobre actividad económica

Es posible encontrar información pública en los portales de información del SEPE (Servicio de Empleo Público Estatal), o el INE (Instituto Nacional de Estadística), o en los servicios de estadística de organismos oficiales (p. ej. Seguridad Social). A continuación os dejamos algunas fuentes de consulta para obtener estos datos:

* INE: <https://www.ine.es/dyngs/DAB/es/index.htm?cid=1722>
* SEPE: <https://sede.sepe.gob.es/portalSede/es/datos-abiertos/catalogo-de-datos-del-SEPE>
* Seguridad Social: <https://www.seg-social.es> (Servicio de Estadísticas)

También es posible obtener información geográfica de Cantabria y Santander. La descripción detallada del API y cómo acceder a través de programas gratuitos como ArcGIS se encuentra en <https://www.territoriodecantabria.es/rest-api>, y el API REST puede encontrarse directamente en <https://geoservicios.cantabria.es/inspire/rest/services>. Se puede encontrar en formato GIS el siguiente ejemplo:

??? info "Información geográfica relacionada con el turismo, como los alojamientos hoteleros, los campings, hostales, pensiones o viviendas turísticas, entre otros"
    * **Descripción:** Información sobre movilidad ciclista en el municipio de Santander.
    * **Formato:** JSON/SOAP (Estándar GIS)
    * **Acceso:** Abierto
    * **Fuente:** Gobierno de Cantabria / Ayto. Santander
    * **Endpoint:** <https://geoservicios.cantabria.es/inspire/rest/services/Turismo_Infraestructura_Turistica/FeatureServer>