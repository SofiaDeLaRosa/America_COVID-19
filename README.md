<h1 align="center"> LATAM COVID-19 </h1> <br>

<p align="center">
    <img src="https://github.com/SofiaDeLaRosa/LATAM_COVID-19/blob/main/escudos.png" alt="escudos">
</p>

<h3 align="center"> Universidad Nacional Autónoma de México (National Autonomous University of Mexico | UNAM) </h3> 
<h3 align="center"> Escuela Nacional de Estudios Superiores Unidad Morelia (National School of Superior-Level Studies, Morelia Campus | ENES) </h3> 

<h3 align="center"> Licenciatura en Tecnologías para la Información en Ciencias (information technologies in science | TICS) </h3> 
<h3 align="center"> Digital Repositories (2024-2) </h3> 

<h3 align="center"> LATAM COVID-19 Project </h3> 

<h4 align="center"> Student: Sofía García De La Rosa </h4> 
<h4 align="center"> No. de student account: 421099803 </h4>

<h4 align="center"> Teacher: Dr. Arturo López Pineda </h4> 

<h4 align="center"> Date: May 23, 2024 </h4> 

## Summary

## Table of Contents
Summary <br>
Table of Contents <br>
[1. Introduction](#introduction)
[2. Materials and Methods](#materials_methods)
   [2.1. Databases](#Databases)
   [2.2. Variables](#Variables)
   [2.3. Unification](#unification)
[3. Results](#results)
[4. Reflections](#reflections)
[5. Recommendations](#recommendations)
[6. Conclusions](#conclusions)
[7. Bibliography](#bibliography)

## 1. Introduction
The COVID-19 pandemic has had a profound and unprecedented impact on public health, economies, and societies worldwide, revealing various challenges and responses in managing the health crisis. In this context, data analysis is crucial for understanding the evolution of the pandemic and its effects, even five years later, when interest in its tracking has waned.

## 2. Materials and Methods
For data cleaning, integration, and unification, pandas was used. For visualization, Power BI was employed.

### 2.1. Databases
COVID-19 data were sought from 37 countries in the Americas from health ministries, health-related centers and departments, open data platforms, and statistics platforms.

The decision was made to work with Colombia, Mexico, and Peru, as the other countries had:

* Data not available
* Non-individual data in PDF format
* Data that are no longer available
* Servers with unavailable data

| # | País | Fuente | Link Oficial | Comentario |
|--|------|------------|------------|------------|
| 1 | Antigua y Barbuda | The Statistics Division in the Ministry of Finance and Corporate Governance | https://statistics.gov.ag/covid-19-dashboard/ | Datos no disponibles |
| 2 | Argentina | Datos Abiertos del Ministerio de Salud de Argentina | http://datos.salud.gob.ar/dataset/covid-19-casos-registrados-en-la-republica-argentina | |
| 3 | Bahamas | Ministry of Health | https://healthytogether.gov.bs/combatting-covid-19/covid-19-data/ | Datos no disponibles |
| 4 | Barbados | Ministry of Health | https://gisbarbados.gov.bb/covid-19/ | Datos no individuales en formato PDF |
| 5 | Bélice | Ministry of Health | https://www.health.gov.bz/covid-19/ | Datos ya no están disponibles |
| 6 | Bolivia | Sistema Nacional de Información en Salud - Vigilancia Epidemiológica | https://datos.gob.bo/dataset/casos-covid-19-acumulado-por-municipios https://datos.gob.bo/group/salud | Datos agregados no individuales |
| 7 | Brasil | Datos Abiertos Brasi | https://dados.gov.br/dados/conjuntos-dados/registro-de-ocupacao-hospitalar-covid-19 | |
| 8 | Canadá | | https://health-infobase.canada.ca/covid-19/ https://open.canada.ca/data/en/dataset/261c32ab-4cfd-4f81-9dea-7b64065690dc | |  
| 9 | Chile | Ministerio de Ciencia | https://observa.minciencia.gob.cl/datos-abiertos/datos-del-repositorio-covid-19 | Última actualización 30 de agosto del 2023 |
| 10 | Colombia | Instituto Nacional de Salud | https://www.ins.gov.co/Noticias/Paginas/Coronavirus.aspx | |
| 11 | Costa Rica | Ministerio de Salud | https://www.ministeriodesalud.go.cr/index.php/vigilancia-de-la-salud/41-lineamientos-coronavirus/527-situacion-nacional-covid-19 | Información no disponible en formato descargable |
| 12 | Cuba | Ministerio de Salud | https://salud.msp.gob.cu/category/covid-19/ | Información no disponible en formato descargable |
| 13 | Dominica | Ministry of Health | https://covid19.dominica.gov.dm/ | Información no disponible en formato descargable |
| 14 | Ecuador | Datos Abiertos del Ministerio de Salud Pública | https://www.salud.gob.ec/datos-abiertos/ | Información no disponible en formato descargable |
| 15 | El Salvador | | https://tableros.mspas.gob.gt/covid/ https://elsalvador.un.org/sites/default/files/2020-05/ElSalvador-COVID-19-InformedesituaciónNo.9-Al26demayo2020.pdf Puede leer también: https://www.google.com/url?q=https://www.elsalvador.com/noticias/nacional/oms-coronavirus-fallecidos-por-covid-19/953482/2022/&sa=D&source=docs&ust=1715455787991936&usg=AOvVaw37Gzm5R3fyKgA13kwq2HBs | Información no disponible en formato descargable |
| 16 | Estados Unidos | Centers for Disease Control and Prevention | https://www.cdc.gov/coronavirus/2019-ncov/covid-19-data-and-surveillance.html | |
| 17 | Granada | Ministry of Health | NA | No website for MoH | 
| 18 | Guatemala | Ministerio de Salud y Asistencia Social | https://tableros.mspas.gob.gt/covid/ https://www.reuters.com/graphics/world-coronavirus-tracker-and-maps/es/countries-and-territories/guatemala/ https://github.com/ncovgt2020/ncovgt2020 | Información no disponible en formato descargable | 
| 19 | Guayana Francesa | | | Información no disponible | 
| 20 | Guyana | Ministry of Health | https://www.health.gov.gy/ | Información no disponible en formato descargable | 
| 21 | Haití | | | Información no disponible |
| 22 | Honduras | | | Información no disponible |
| 23 | Jamaica | Ministry of Health | https://www.moh.gov.jm/updates/coronavirus/ | Información no disponible en formato descargable |
| 24 | México | Dirección General de Epidemiología Secretaría de Salud | https://www.gob.mx/salud/documentos/datos-abiertos-152127 | | 
| 25 | Nicaragua | | | Información no disponible |
| 26 | Panamá | Ministerio de Salud | https://www.minsa.gob.pa/destacado/coronavirus-covid-19 | Información no disponible en formato descargable |
| 27 | Paraguay | Ministerio de Salud Publica de Paraguay | https://www.mspbs.gov.py/institucion.html https://dgvs.mspbs.gov.py/mapa-de-riesgo-covid-19/ https://www.mspbs.gov.py/reportes-covid19.html | | 
| 28 | Perú | Plataforma Nacional de Datos Abiertos | https://www.datosabiertos.gob.pe/group/datos-abiertos-de-covid-19 | | 
| 29 | Puerto Rico | Centers for Disease Control and Prevention | https://data.cdc.gov/browse?tags=puerto+rico | 
| 30 | República Dominicana | Ministerio de Salud | https://coronavirusrd.gob.do/ | Información no disponible en formato descargable |
| 31 | San Cristóbal y Nieves | | | Información no disponible |
| 32 | San Vicente y las Granadinas | Ministerio de Salud | https://health.gov.vc/health/index.php/c?start=732 | Información no disponible en formato descargable |
| 33 | Santa Lucía | Ministerio de Salud | https://www.covid19response.lc/ | Información no disponible en formato descargable |
| 34 | Surinam | Ministerio de Salud | https://gov.sr/covid-19-update-suriname/ | Información no disponible |
| 35 | Trinidad y Tobago | Ministerio de Salud | https://health.gov.tt/covid-19/covid-19-news-and-updates/update-trinidad-and-tobago |Información no disponible en formato descargable |
| 36 | Uruguay | | https://www.gub.uy/ministerio-salud-publica/comunicacion/noticias/informe-epidemiologico-covid-19-actualizado-18-enero-2021 https://www.gub.uy/sistema-nacional-emergencias/pagina-embebida/visualizador-casos-coronavirus-covid-19-uruguay https://www.gub.uy/ministerio-salud-publica/comunicacion/publicaciones/semana-epidemiologica-17-del-240422-300422-casos-covid19-0 | Datos no individuales |
| 37 | Venezuela | | https://mppre.gob.ve/coronavirus/ | Información no disponible en formato descargable |

### 2.2. Variables
Colombia had 23 variables: 'fecha reporte web' (web report date), 'ID de caso' (case ID), 'Fecha de notificación' (notification date), 'Código DIVIPOLA departamento' (DIVIPOLA department code), 'Nombre departamento' (department name), 'Código DIVIPOLA municipio' (DIVIPOLA municipality code), 'Nombre municipio' (municipality name), 'Edad' (age), 'Unidad de medida de edad' (age unit), 'Sexo' (sex), 'Tipo de contagio' (type of contagion), 'Ubicación del caso' (case location), 'Estado' (status), 'Código ISO del país' (ISO country code), 'Nombre del país' (country name), 'Recuperado' (recovered), 'Fecha de inicio de síntomas' (symptoms onset date), 'Fecha de muerte' (death date), 'Fecha de diagnóstico' (diagnosis date), 'Fecha de recuperación' (recovery date), 'Tipo de recuperación' (type of recovery), 'Pertenencia étnica' (ethnic affiliation), 'Nombre del grupo étnico' (ethnic group name).

Mexico had 40 variables: 'FECHA_ACTUALIZACION' (update date), 'ID_REGISTRO' (record ID), 'ORIGEN' (origin), 'SECTOR' (sector), 'ENTIDAD_UM' (UM entity), 'SEXO' (sex), 'ENTIDAD_NAC' (birth entity), 'ENTIDAD_RES' (residence entity), 'MUNICIPIO_RES' (residence municipality), 'TIPO_PACIENTE' (patient type), 'FECHA_INGRESO' (admission date), 'FECHA_SINTOMAS' (symptoms date), 'FECHA_DEF' (death date), 'INTUBADO' (intubated), 'NEUMONIA' (pneumonia), 'EDAD' (age), 'NACIONALIDAD' (nationality), 'EMBARAZO' (pregnancy), 'HABLA_LENGUA_INDIG' (speaks indigenous language), 'INDIGENA' (indigenous), 'DIABETES' (diabetes), 'EPOC' (COPD), 'ASMA' (asthma), 'INMUSUPR' (immunosuppressed), 'HIPERTENSION' (hypertension), 'OTRA_COM' (other conditions), 'CARDIOVASCULAR' (cardiovascular), 'OBESIDAD' (obesity), 'RENAL_CRONICA' (chronic kidney disease), 'TABAQUISMO' (smoking), 'OTRO_CASO' (another conmorbility), 'TOMA_MUESTRA_LAB' (lab sample taken), 'RESULTADO_LAB' (lab result), 'TOMA_MUESTRA_ANTIGENO' (antigen sample taken), 'RESULTADO_ANTIGENO' (antigen result), 'CLASIFICACION_FINAL' (final classification), 'MIGRANTE' (migrant), 'PAIS_NACIONALIDAD' (nacionality country), 'PAIS_ORIGEN' (origin country), 'UCI' (ICU).

On the other hand, Peru had only 10 variables: 'FECHA_CORTE' (update date), 'DEPARTAMENTO' (department), 'PROVINCIA' (province), 'DISTRITO' (district), 'METODODX' (method), 'EDAD' (age), 'SEXO' (sex), 'FECHA_RESULTADO' (result date), 'UBIGEO' (UBIGEO), 'id_persona' (person id).


In Colombia, there were null values in: symptom onset date, death date, and diagnosis date, with no repeated records (not even just the IDs). In Mexico, only 0.28% of the IDs were repeated. Since it was a low percentage, it was decided to delete them. In Peru, there were null values in all columns (ID, AGE, and result date) except for cut date, 95.23% of the records and 99.73% of the IDs were repeated. However, these records were not deleted since it was concluded that many people could have the same data because there were only 10 columns, and several are very general.


| Country | Variables | N after cleaning | Men | Women | Age 0-19 (junior) | Age 20-40 (young_adult) | Age 40-59 (middle_aged_adult) | Age 60-79 (older_adult)| Age 80+ (elderly) | 
|------|---------------|----------|------|------|------|------|------|------|------|
| Colombia | 6,390,972 (2020-2021) | 5,882,932 (2020-2021) | 2,733,631 (2020-2021) | 3, 149,301 (2020-2021) | 640,852 (2020-2021) | 2,507,905 (2020-2021) | 1,780,560 (2020-2021) | 789,190 (2020-2021) | 164,425 (2020-2021) |
| México | 8,281,058 (2020-2024) | 3,320,238 (2020-2024) | 1,547,970 (2020-2024) | 1,772,268 (2020-2024) | 198,312 (2020-2024) | 1,354,517 (2020-2024) | 1,211,793 (2020-2024) | 477,462 (2020-2021) | 78,154 (2020-2024) |
| Perú | 4,585,360 (2020-2023) | 4,585,360 (2020-2023)| 2,208,480 (2020-2023)| 2,376,880 (2020-2023)| 417,192 (2020-2023)| 1,953,968 (2020-2023)| 1,486,732 (2020-2023)| 620,248 (2020-2023)| 106,867 (2020-2023)|
| Total | | 19,257,390 | 13,788,530 | 6,490,081 | 7,298,449 | 1,256,356 | 5,816,390 | 4,479,085 | 1,886,900 | 349,446 |

## 2.3 Unification
We merged the databases based on the age and sex columns, as these were the common attributes across all datasets. For the sex attribute, we transformed the data using the codes from The Observational Medical Outcomes Partnership (OMOP):
* f, Female → '8532'
* M, Male → '8507'
  
We classified age into 5 groups:
* [0-19] → 'junior'
* [20-39] → 'young_adult'
* [40-59] → 'middle_aged_adult'
* [60-79] → 'older'
* 80+ → 'elderly'

To merge the databases, we used the 'concat' function from pandas, and by using the 'FINAL_CLASSIFICATION' column, we only retained confirmed COVID-19 cases from Mexico, as the records from Peru and Colombia represented positive COVID-19 cases.

## 4. Results

An important variable we considered was the death date, to understand what percentage of people with COVID-19 did not die. Only Mexico and Colombia had it, as Peru had a different dataset exclusively for deceased individuals due to COVID-19.

% WITHOUT DEATH DATE IN COLOMBIA:
* 97.11% (2020 - 2021)
* 
% WITHOUT DEATH DATE IN MEXICO:
* 94.53% (2020)
* 96.02% (2021)
* 98.86% (2022)
* 99.24% (2023)
* 99.08% (2024)

The percentage of null values for death_date was always quite high and increased over time.

As we can see in the previous table, there were generally more positive COVID-19 cases in Colombia compared to Mexico and Peru, considering the period from 2020 to 2021. Additionally, there were more positive COVID-19 cases among women in all countries. Furthermore, young adults were the most affected, while older adults were the least affected.

The created dashboard shows the distribution of positive COVID-19 cases based on age groups, as well as their proportion according to sex.

<p align="center">
    <img src="https://github.com/SofiaDeLaRosa/LATAM_COVID-19/blob/main/covid.PNG" alt="graficas">
</p>

## 5. Reflections
Reasons why some countries lack data could be: limited technological infrastructure, lack of financial resources, lack of priority, and/or lack of transparency.

## 6. Recommendations
* Invest in technology
* Adopt appropriate standards and formats
* Ensure data quality, availability, and updates on web portals
* Create real-time interactive dashboards
* Educate on the importance of COVID-19 monitoring
* Document data collection, management, and dissemination processes
* Maintain a history and version control of changes made
* Promote collaboration with institutions

## 7. Conclusions
COVID-19 is still present, making it crucial to maintain its monitoring. To achieve this, countries should have the appropriate technology, be transparent, maintain and update servers, meet quality criteria and standards like OMOP, thus facilitating the search, analysis, and visualization of data globally. In this way, the data will serve not only as a reliable and up-to-date source of information for the general public but also enable governments, businesses, and health institutions to make better decisions and formulate more effective public health policies for managing COVID-19.

## 5. Bibliography
Ministerio de Salud Argentina. (s.f.). Ministerio de Salud Argentina. Obtained from http://datos.salud.gob.ar/dataset/covid-19-casos-registrados-en-la-republica-argentina/archivo/fd657d02-a33a-498b-a91b-2ef1a68b8d16

Observational Health Data Sciences and Informatics. (2024). Observational Health Data Sciences and Informatics. Obtenido de https://www.ohdsi.org/data-standardization/
Plataforma Nacional de Datos Abiertos. (s.f.). Obtained from https://www.datosabiertos.gob.pe/dataset/casos-positivos-por-covid-19-ministerio-de-salud-minsa

Salud, S. d. (2024). Gobierno de México. Obtained from https://www.gob.mx/salud/documentos/datos-abiertos-152127


