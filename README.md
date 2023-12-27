<h1 align="center"> Proyecto Integrador Data Analysis - PIDA <br> Siniestros Viales </h1>

![Alt text](src/image.png)

## Introducción

El Observatorio de Movilidad y Seguridad Vial (OMSV), organismo de la Ciudad Autónoma de Buenos Aires, solicita la elaboración de un proyecto de anális de datos, con el fin de generar información que le permita a las autoridades locales tomar medidas para disminuir la cantidad de víctimas fatales de los siniestros viales.

Para este estudio, disponibiliza un dataset sobre homicidios en siniestros viales acaecidos en la Ciudad de Buenos Aires durante el periodo 2016-2021. Se puede encontrar en https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales

## Planteamiento del problema

Los siniestros viales, como accidentes de tráfico, engloban colisiones entre vehículos, peatones o objetos fijos en vías públicas. En urbes densamente pobladas como Buenos Aires, son preocupaciones cruciales debido al alto tráfico. Pueden causar desde daños materiales hasta lesiones graves o fatales.

Las tasas de mortalidad por estos eventos indican la seguridad vial y su reducción es clave para proteger a quienes transitan la ciudad. La prevención implica educación vial, cumplimiento de normas, seguridad en la infraestructura vial y promoción de vehículos más seguros. El seguimiento estadístico y políticas efectivas son esenciales para abordar este problema.

Cada año en Argentina, alrededor de 4.000 personas pierden la vida en incidentes viales, una cifra alarmante que continúa siendo la principal causa de muertes violentas en el país, a pesar de los esfuerzos por reducir los accidentes de tránsito. Informes del Sistema Nacional de Información Criminal (SNIC) del Ministerio de Seguridad de la Nación revelan que entre 2018 y 2022 se registraron 19.630 muertes por siniestros viales en todo el territorio argentino. Esto significa un promedio de 11 víctimas fatales diarias debido a accidentes de tráfico.

Solo en el año 2022, se reportaron 3.828 muertes fatales por este tipo de incidentes. Los expertos señalan que en Argentina la probabilidad de morir en un siniestro vial es dos o tres veces mayor que en un acto delictivo de inseguridad.

## Desarrollo

###  ETL

se realiza la extraccíon y limpieza de los datos de los dos dataset HECHOS y VICTIMAS, a tráves de la utilización de Pandas y Jupyter Netbook.Eliminando nulos, duplicados, con transformaciones necesarias como cambio en los tipos de datos, eliminación de columnas y unión de las tablas en un archivo siniestros_viales.csv archivo.

### EDA

una vez que los datos están limpios, es momento de revisar las relaciones que existen entre las variables numéricas y categóricas de los datasets, encontrar si hay presencia de outliers o anomalías (que no tienen que ser errores necesariamente), y se verificó si hay algún patrón o conocimiento que sirva en un análisis posterior.

### Indicadores de Rendimiento Clave - KPI

- **KPI 1 - Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior**

Se define la tasa de homicidios en siniestros viales como el número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico. Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000

- **KPI 2 - Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior**

Se define la cantidad de accidentes mortales de motociclistas en siniestros viales como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal. Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100


## Conclusiones

Tras un análisis exhaustivo y su representación en un panel de control en PowerBi, se determina que entre 2016 y 2021, hubo 717 fallecidos por accidentes de tráfico. Se identificaron momentos críticos durante las horas de entrada laboral (5-9 a.m.), almuerzo (12-2 p.m.) y regreso a casa (5-6 p.m.). Durante los fines de semana (sábado y domingo), los accidentes se concentran en horarios nocturnos (3-7 a.m.). El 76% de las víctimas fueron hombres, mayormente entre 20 y 40 años, y predominantemente en el rol de conductor en accidentes masculinos. Las motocicletas son los vehículos más frecuentes entre las víctimas, seguidas por los peatones; en los acusados, los autos, los autobuses y los vehículos de carga son los más comunes. Los accidentes ocurren mayormente en avenidas y en intersecciones. Se observa un patrón notable en relación con la edad, hora y género, donde los hombres de 20 a 40 años están implicados en accidentes durante las horas laborales o, en el caso de los fines de semana, en horarios nocturnos.

Entonces, se sugiere la mejora de la señalización y la implementación de controles más efectivos en las avenidas, especialmente en las comunas 1 y 4 de la Ciudad Autónoma de Buenos Aires. Además, se plantea la posibilidad de lanzar campañas preventivas específicamente orientadas a hombres de entre 20 y 40 años.

## Tecnologías utilizadas

Para llevar a cabo este procedimiento, utilizamos Visual Studio Code (VSCODE) localmente junto con Jupyter Notebook como nuestra plataforma principal. Empleamos un conjunto de herramientas tecnológicas que involucra Python como lenguaje de programación principal, respaldado por librerías fundamentales como numpy y pandas para la manipulación eficiente de datos. Además, hicimos uso de matplotlib y seaborn para generar visualizaciones gráficas que destacaron patrones y tendencias ocultas en los datos de forma efectiva.

Para el desarrollo del Dashboard, se hizo uso de PowerBi.


