<p align="left">
  <a href="https://www.python.org/"><img src="http://ForTheBadge.com/images/badges/made-with-python.svg" alt="Made with Python" height="40"/></a>
  <a href="https://jupyter.org/try"><img src="https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter" alt="Made with Jupyter" height="40"/></a>
  <a href="https://www.mysql.com/"><img src="https://img.shields.io/badge/Made%20with-MySQL-blue?style=for-the-badge&logo=MySQL" alt="Made with MySQL" height="40"/></a>
  <a href="https://azure.microsoft.com/"><img src="https://img.shields.io/badge/Made%20with-Azure-blueviolet?style=for-the-badge&logo=Microsoft-Azure" alt="Made with Azure" height="40"/></a>
  <a href="https://powerbi.microsoft.com/"><img src="https://img.shields.io/badge/Made%20with-PowerBI-yellow?style=for-the-badge&logo=Power-BI" alt="Made with Power BI" height="40"/></a>
  <a href="https://www.microsoft.com/en-us/microsoft-365/excel"><img src="https://img.shields.io/badge/Made%20with-Excel-green?style=for-the-badge&logo=Microsoft-Excel" alt="Made with Excel" height="40"/></a>
</p>

# Covid-19, un análisis de casos y su correlación con vacunación, indicadores de desarrollo y variables ambientales

Se han utilizado varias fuentes de datos de acceso abierto para recopilar información esencial relacionada con la pandemia de COVID-19.

La primera fuente, proporcionada por la **Organización Mundial de la Salud (OMS)**, nos brinda detalles sobre los casos diarios y las muertes a nivel mundial [1]. Además, otra fuente de la OMS ofrece información adicional sobre los casos confirmados, las muertes y las tasas por cada 100,000 habitantes [2]. Para evaluar el progreso de la vacunación, utilizamos datos de la OMS que incluyen la administración de dosis y el número de personas vacunadas parcial o completamente, junto con información sobre los tipos de vacunas utilizadas en cada país [3] [4].

El **Centro Europeo para la Prevención y el Control de Enfermedades (ECDC)** proporciona datos cruciales sobre las pruebas realizadas y la positividad por COVID-19 [5]. Además, hemos recurrido a datos sobre la ocupación hospitalaria y las unidades de cuidados intensivos (UCI) de ECDC para evaluar la capacidad de atención médica [6].

Finalmente, los datos específicos sobre los casos diarios registrados en Estados Unidos se obtuvieron del **Centro para Sistemas de Ciencia e Ingeniería de la Universidad John Hopkins** [7].

Para nuestra investigación, nos propusimos explorar la relación entre los datos relacionados con la pandemia de COVID-19 y diversos indicadores de desarrollo del Banco Mundial. En particular, nos centramos en variables clave, como el porcentaje de individuos que utilizan Internet, la proporción de personas que tienen acceso a servicios básicos de agua potable, la disponibilidad de servicios básicos de saneamiento, la densidad de población (medida en personas por kilómetro cuadrado de superficie terrestre), la proporción de población rural en relación con el total de población y la proporción de población urbana en relación con el total de población. Así mismo, se tendrá en cuenta el PIB.

Además de estos indicadores de desarrollo, también tuvimos en cuenta factores geográficos y meteorológicos, incluyendo la altura promedio sobre el nivel del mar y la temperatura promedio en las regiones de interés. Estos datos complementarios se incorporaron en nuestro análisis para proporcionar una comprensión más completa de cómo la pandemia de COVID-19 se relaciona con diversos aspectos sociodemográficos, geográficos y económicos.

Todo este proceso se automatizó mediante Python para que los conjuntos de datos se actualicen de forma semanal y pasen por todo el preprocesado, utilizando una arquitectura en la nube con Azure.

Finalmente, todo esto se tradujo en una serie de Dashboards elaborados en Power BI.

El presente repositorio es una réplica de toda nuestra estructura de datos, cuadernos de trabajo, dashboards y documentación de cada etapa del proceso.


## Créditos

Este trabajo fue llevado a cabo en el marco del trabajo final del máster de _Business Intelligence and Data Management_ en INESDI en la promoción 2023-2024, el equipo estuvo conformado por:

- [Fabián Ascheri](https://www.linkedin.com/in/fabian-ascheri-26456a2b/)
- [Jose Chavarria](https://www.linkedin.com/in/jose-chavarria-ab911a54/)
- Amaia Miranda
- [Patricia Peña](https://www.linkedin.com/in/patricia-pena-torres/)
- [Juan Carlos Valcuende](https://www.linkedin.com/in/juan-carlos-valcuende-alaez-b5952ba1/)

## Referencias


1. **Organización Mundial de la Salud**. (s. f.). *Datos globales de COVID-19 de la OMS* [Datos en formato CSV]. [acceso aquí](https://covid19.who.int/WHO-COVID-19-global-data.csv).

2. **Organización Mundial de la Salud**. (s. f.). *Tabla global de datos de COVID-19 de la OMS* [Datos en formato CSV]. [acceso aquí](https://covid19.who.int/WHO-COVID-19-global-table-data.csv).

3. **Organización Mundial de la Salud**. (s. f.). *Datos de vacunación de la OMS* [Datos en formato CSV]. [acceso aquí](https://covid19.who.int/who-data/vaccination-data.csv).

4. **Organización Mundial de la Salud**. (s. f.). *Metadatos de vacunación de la OMS* [Datos en formato CSV]. [acceso aquí](https://covid19.who.int/who-data/vaccination-metadata.csv).

5. **European Centre for Disease Prevention and Control**. (s. f.). *Datos de pruebas ECDC* [Página web]. [acceso aquí](https://opendata.ecdc.europa.eu/covid19/testing/).

6. **European Centre for Disease Prevention and Control**. (s. f.). *Datos de hospitalización y ocupación de UCI de ECDC* [Datos en formato CSV]. [acceso aquí](https://www.ecdc.europa.eu/en/publications-data/download-data-hospital-and-icu-admission-rates-and-current-occupancy-covid-19).

7. **Universidad John Hopkins**. (s. f.). *Casos diarios en EE.UU.* [acceso aquí](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data/csse_covid_19_daily_reports_us).
