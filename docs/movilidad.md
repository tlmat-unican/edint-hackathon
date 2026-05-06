# Caso de Uso 1: Movilidad Inteligente

Conjuntos de datos relacionados con el caso de uso "Movilidad Inteligente" en la ciudad de Santander.

## Información del servicio de bicicletas eléctricas Santander TUeBICI

Listado de endpoints con información relativa al servicio de bicicletas eléctricas de TUeBICI e información relacionada como la situación de los carriles bici en Santander.

??? info "Estado de las estaciones TUeBICI"
    * **Descripción:** Datos de estado e información de las estaciones de bicicletas, incluyendo el identificador, su localización y la capacidad total.
    * **Formato:** JSON (Estándar GBFS)
    * **Acceso:** Abierto
    * **Fuente:** NEXTBIKE / Ayto. Santander
    * **Endpoint:** <https://gbfs.nextbike.net/maps/gbfs/v2/nextbike_ek/es/station_information.json>

??? info "Tipos de bicicletas eléctricas TUeBICI"
    * **Descripción:** Información sobre el tipo de bicicleta eléctrica de TUeBICI.
    * **Formato:** JSON (Estándar GBFS)
    * **Acceso:** Abierto
    * **Fuente:** NEXTBIKE / Ayto. Santander
    * **Endpoint:** <https://gbfs.nextbike.net/maps/gbfs/v2/nextbike_ek/es/vehicle_types.json>

??? info "Estado de las bicicletas libres eléctricas TUeBICI"
    * **Descripción:** Información sobre el estado de cada una de las bicicletas eléctricas de TUeBICI cuando no están ocupadas. Incluye información como la posición, el estado de la carga (current_fuel_percent) o el rango (current_range_meters).
    * **Formato:** JSON (Estándar GBFS)
    * **Acceso:** Abierto
    * **Fuente:** NEXTBIKE / Ayto. Santander
    * **Endpoint:** <https://gbfs.nextbike.net/maps/gbfs/v2/nextbike_ek/es/free_bike_status.json>

??? info "Horario de funcionamiento del servicio de bicicletas eléctricas TUeBICI"
    * **Descripción:** Información sobre el horario de funcionamiento de TUeBICI.
    * **Formato:** JSON (Estándar GBFS)
    * **Acceso:** Abierto
    * **Fuente:** NEXTBIKE / Ayto. Santander
    * **Endpoint:** <https://gbfs.nextbike.net/maps/gbfs/v2/nextbike_ek/es/system_hours.json>

??? info "Planes de precios de las bicicletas TUeBICI"
    * **Descripción:** Planes de precios de TUeBICI. Incluye el coste por periodos de tiempo.
    * **Formato:** JSON (Estándar GBFS)
    * **Acceso:** Abierto
    * **Fuente:** NEXTBIKE / Ayto. Santander
    * **Endpoint:** <https://gbfs.nextbike.net/maps/gbfs/v2/nextbike_ek/es/system_pricing_plans.json>

??? info "Carriles bici de Santander"
    * **Descripción:** Información sobre la localización de los carriles bici de Santander. El parámetro más importante, ayto:WKT describe el objeto geográfico en forma de polilínea con el formato WKT (Well-Known Text).
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/api/rest/datasets/carril_bici.json>

??? info "Datos históricos sobre el estado de las bicicletas"
    * Descripción: Datos históricos (Oct-24 a Feb-25) sobre el estado de las estaciones de bicicletas, incluyendo su identificador, su localización, disponibilidad de bicicletas y capacidad total.
    * Formato: JSON (Estándar GBFS)
    * Acceso: Abierto
    * Fuente: NEXTBIKE / Ayto. Santander
    * Endpoint: https://github.com/Sedimark/hackathon-santander-datasets


## Información del servicio de autobuses de Santander TUS


??? info "Listado de las paradas de autobús"
    * **Descripción:** Este recurso contiene todos los datos de la Red de paradas de Autobus desplegadas en el Municipio de Santander y su posición geográfica. Los campos más importantes son:
        * wgs84_pos:long: longitud de la posición de las paradas.
        * wgs84_pos:lat: latitud de la posición de las paradas.
        * ayto:numero: identificador de la parada.
        * vivo:address1: dirección dónde se encuentra la parada.
        * ayto:sentido: sentido de los autobuses que paran en la parada.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/api/rest/datasets/paradas_bus.json>

??? info "Listado con las líneas de autobús del TUS"
    * **Descripción:** Este recurso contiene la información referente a las líneas de Transporte Urbano en uso dentro del Municipio de Santander. Los campos más importantes son:
        * ayto:numero: identificador de la línea.
        * dc:name: nombre de la línea que incluye parada inicial y final.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/api/rest/datasets/lineas_bus.json>

??? info "Listado de Vehículos que conforman la flota del Servicio de Transporte Urbano de Santander"
    * **Descripción:** Este recurso proporciona información sobre los vehículos de la Flota Municipal de Autobuses. Los campos más importantes son:
        * ayto:PlazasDePie: plazas disponibles por autobús.
        * ayto:longitud: tamaño del autobús.
        * ayto:identifier: identificador único del autobús.
        * ayto:Combustible: tipo de motor que utiliza el autobús (e.g. HIBRIDO, ELECTRICO, DIESEL).
        * dc:modified: última fecha de actualización.
        * uri: endpoint que contiene información únicamente sobre ese elemento.
        Para acceder a las páginas y elegir el número de elementos por página hay que utilizar los parámetros de URL "items" y "page". Por ejemplo, en el endpoint 'http://datos.santander.es/api/rest/datasets/control_flotas_vehiculos.json?items=50&page=1' obtendremos la primera página resultante de de agrupar todos los elementos existentes en grupos de 50. En cada petición se incluye la información del número de páginas así como el total de elementos y la página actual.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/api/rest/datasets/control_flotas_vehiculos.json>

??? info "Pasos por parada de los últimos 10 días"
    * **Descripción:** Este recurso proporciona información sobre el paso por parada de cada vehículo y línea de la Flota Municipal de Autobuses de los últimos 10 días. Se actualiza una vez al dia. Los campos más importantes son:
        * ayto:instante: timestamp del paso por parada.
        * ayto:linea: línea a la que pertenece el vehículo.
        * ayto:descparada: descripción de la localización de la parada.
        * ayto:parada: identificador de la parada.
        Para acceder a las páginas y elegir el número de elementos por página hay que utilizar los parámetros de URL "items" y "page". Por ejemplo, en el endpoint 'http://datos.santander.es/api/rest/datasets/programacionTUS_pasos_parada_10dias.json?items=50&page=1' obtendremos la primera página resultante de de agrupar todos los elementos existentes en grupos de 50. En cada petición se incluye la información del número de páginas así como el total de elementos y la página actual.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/api/rest/datasets/programacionTUS_pasos_parada_10dias.json>
 http://datos.santander.es/api/rest/datasets/paradas_bus.json


## Movilidad eléctrica

??? info "Nuevos puntos de recarga de vehículo eléctrico"
    * **Descripción:** Este dataset contiene el número de nuevos puntos de recarga de vehículo eléctrico con acceso público dados de alta cada mes, con detalle a nivel de municipio. A estos efectos, se consideran como de acceso publico, aquellos puntos de recarga que tengan contratada una tarifa de acceso de vehículo eléctrico.
    * **Formato:** JSON / CSV / EXCEL
    * **Acceso:** Abierto
    * **Fuente:** VIESGO
    * **Endpoint:** <https://redes-spain.opendatasoft.com/explore/dataset/3-nuevos-puntos-de-recarga-de-vehiculo-electrico-viesgo/information/>

??? info "Consumo de puntos de recarga de vehículo eléctrico"
    * **Descripción:** En este dataset se representa el consumo mensual total de energía activa por municipio de los puntos de recarga de acceso publico de vehículo eléctrico. A estos efectos, se consideran como de acceso publico, aquellos puntos de recarga que tengan contratada una tarifa de acceso de vehículo eléctrico.
    * **Formato:** JSON / CSV / EXCEL
    * **Acceso:** Abierto
    * **Fuente:** VIESGO
    * **Endpoint:** <https://redes-spain.opendatasoft.com/explore/dataset/5-consumo-mensual-de-puntos-de-recarga-de-ve-viesgo/information/>

??? info "Puntos de recarga de vehículo eléctrico"
    * **Descripción:** Este dataset muestra la ubicación y potencia máxima admisible de la instalación del total de puntos de recarga de vehículo eléctrico de acceso publico por municipio. A estos efectos, se consideran como de acceso publico, aquellos puntos de recarga que tengan contratada una tarifa de acceso de vehículo eléctrico. 
    * **Formato:** JSON / CSV / EXCEL
    * **Acceso:** Abierto
    * **Fuente:** VIESGO
    * **Endpoint:** <https://redes-spain.opendatasoft.com/explore/dataset/4-puntos_publicos_de_recarga_de_vehiculos_electricos-viesgo/information/>

## Otra información sobre movilidad en Santander

??? info "Plazas para Personas con Movilidad Reducida"
    * **Descripción:** Este recurso proporciona información sobre las plazas de aparcamiento para personas con movilidad reducida en el municipio de Santander. Entre otros datos se incluye la posición Geográfica de cada plaza.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/resource/?ds=plazas-pmr&id=12eac87c-bf46-48aa-bcc4-20fcf60ffdd2&ft=JSON>

??? info "Zona 30"
    * **Descripción:** Este conjunto de datos contiene datos geográficos referentes a las calles de Santander definidas como Zonas 30 (dónde los vehículos tienen como límite de velocidad 30 Km/h). Las geometrías usan como sistema de referencia ED50 y están proyectadas en coordenadas UTM.
    * **Formato:** JSON
    * **Acceso:** Abierto
    * **Fuente:** TUS / Ayto. Santander
    * **Endpoint:** <http://datos.santander.es/resource/?ds=zonas-30&id=092414a7-d54a-44fb-a97b-96341b381f93&ft=JSON>


## Información geográfica de Santander y Cantabria

Información geográfica de Cantabria. La descripción detallada del API y cómo acceder a través de programas gratuitos como ArcGIS se encuentra en <https://www.territoriodecantabria.es/rest-api>, y el API REST puede encontrarse directamente en `
<https://geoservicios.cantabria.es/inspire/rest/service>`. Se puede encontrar en formato GIS el siguiente ejemplo:

??? info "Información geográfica relacionada con la movilidad ciclista"
    * **Descripción:** Información sobre movilidad ciclista en el municipio de Santander.
    * **Formato:** JSON/SOAP (Estándar GIS)
    * **Acceso:** Abierto
    * **Fuente:** Gobierno de Cantabria / Ayto. Santander
    * **Endpoint:** <https://geoservicios.cantabria.es/inspire/rest/services/Movilidad/MapServer>
