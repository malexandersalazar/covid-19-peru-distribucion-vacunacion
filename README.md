# Distribución de vacunados contra COVID-19 en Perú

## Antecedentes

Con la llegada del primer lote de vacunas contra la COVID-19 al país, se inició la [Campaña Nacional de Vacunación, Pongo el hombro por el Perú](https://www.gob.pe/institucion/minsa/campa%C3%B1as/3451-campana-nacional-de-vacunacion-contra-la-covid-19 "Gobierno del Perú"), con el fin de proteger a la población y disminuir el riesgo de enfermar o fallecer.

## Métodos

### Fuentes de Datos

Obtuve las cifras de vacunados contra COVID-19 actualizadas a la fecha **2021-03-01** de la Plataforma Nacional de Datos Abiertos del Gobierno de Perú. Los conjuntos de datos utilizados están disponibles en el repositorio Vacunación contra COVID-19 del Ministerio de Salud [[1]].

### Análisis Estadístico

Para realizar el análisis se agruparon las cifras de vacunados por departamento, sexo, edad y grupo de riesgo. Los registros que no tenian valores numéricos para edad o sexo fueron descartados.

Los grupos etáreos se definieron tomando como base lo expuesto en el repositorio ["Gráficos comparativos de distribuciones poblacionales por grupo etáreo, para todo el Perú y por departamento"](https://github.com/jmcastagnetto/covid-19-peru-distribucion-poblacion-positivos-fallecidos) de Jesus M. Castagnetto.

Los grupos de riesgo se abreviaron según la siguiente tabla para que puedan caber en el gráfico:

Grupo de Riesgo | Abreviación
--- | --- 
PERSONAL DE SALUD | P. SALUD
TRABAJADOR Ó PERSONAL DE LIMPIEZA | T. LIMP.
PERSONAL DE SEGURIDAD | P. SEG.
PERSONAL MILITAR Ó FF AA | FF.AA.
POLICIA NACIONAL DEL PERU | P.N.P.
ESTUDIANTES DE CIENCIAS DE LA SALUD | E. SALUD
BRIGADISTAS | BRIG.

Este proyecto se desarrolló en Python 3.8.5 usando los paquetes **numpy**, **pandas**, **matplotlib**, **seaborn**, **datetime** y **os**. Todos los datos usados están disponibles públicamente [[1]].

## Resultados

![alt text](dist/20210303_PERÚ.png "PERÚ")

El Ministerio de Salud ha reportado **297 667** vacunados por COVID-19 al **2021-03-01** [[1]]. En el caso de los hombres, la mayoría de los vacunados fueron personas de 30 a 39 años (10.39%), seguidas de las personas de 40 a 49 años (8.63%) y de 50 a 59 años (6,26%). Encuentro un patrón similar para las mujeres.

![alt text](dist/20210303_AMAZONAS.png "AMAZONAS")

![alt text](dist/20210303_ANCASH.png "ANCASH")

![alt text](dist/20210303_APURIMAC.png "APURIMAC")

![alt text](dist/20210303_AREQUIPA.png "AREQUIPA")

![alt text](dist/20210303_AYACUCHO.png "AYACUCHO")

![alt text](dist/20210303_CAJAMARCA.png "CAJAMARCA")

![alt text](dist/20210303_CALLAO.png "CALLAO")

![alt text](dist/20210303_CUSCO.png "CUSCO")

![alt text](dist/20210303_HUANCAVELICA.png "HUANCAVELICA")

![alt text](dist/20210303_HUANUCO.png "HUANUCO")

![alt text](dist/20210303_ICA.png "ICA")

![alt text](dist/20210303_JUNIN.png "JUNIN")

![alt text](dist/20210303_LA_LIBERTAD.png "LA LIBERTAD")

![alt text](dist/20210303_LAMBAYEQUE.png "LAMBAYEQUE")

![alt text](dist/20210303_LIMA.png "LIMA")

![alt text](dist/20210303_LORETO.png "LORETO")

![alt text](dist/20210303_MADRE_DE_DIOS.png "MADRE DE DIOS")

![alt text](dist/20210303_MOQUEGUA.png "MOQUEGUA")

![alt text](dist/20210303_PASCO.png "PASCO")

![alt text](dist/20210303_PIURA.png "PIURA")

![alt text](dist/20210303_PUNO.png "PUNO")

![alt text](dist/20210303_SAN_MARTIN.png "SAN MARTIN")

![alt text](dist/20210303_TACNA.png "TACNA")

![alt text](dist/20210303_TUMBES.png "TUMBES")

![alt text](dist/20210303_UCAYALI.png "UCAYALI")

La proporción de vacunados femeninos es superior en todos los grupos de edad y departamentos, excepto para algunos de los grupos de 60 a 69 años. No encontré diferencias estadísticamente significativas para los grupos de 10 a 19 años y los de 70 a 79 años. 

La proporción de vacunados masculinos es superior en el grupo de riesgo de personal de seguridad de todos los departamentos, con excepción del departamento de Puno.

## Conclusión

**2021-03-03** Utilizando los datos de vacunación contra COVID-19, encontré que la población femenina tiene una cuota dominante en el **sistema de salud**, mientras que la masculina tiene una cuota dominante en el oficio de **personal de seguridad**.

## Disponibilidad de datos y materiales 

Los conjuntos de datos utilizados en el presente proyecto están disponibles en el repositorio [Vacunación contra COVID-19](https://www.datosabiertos.gob.pe/dataset/vacunaci%C3%B3n-contra-covid-19-ministerio-de-salud-minsa "[Ministerio de Salud - MINSA] | Plataforma Nacional de Datos Abiertos")

## Referencias

1. Ministerio de Salud - MINSA. (s.f.). _[Vacunación contra COVID - 19 - [Ministerio de Salud - MINSA] | Plataforma Nacional de Datos Abiertos_. Gobierno del Perú. Recuperado el 3 de marzo de 2021 de https://www.datosabiertos.gob.pe/dataset/vacunaci%C3%B3n-contra-covid-19-ministerio-de-salud-minsa

[1]: https://www.datosabiertos.gob.pe/dataset/vacunaci%C3%B3n-contra-covid-19-ministerio-de-salud-minsa

2. Jesus M. Castagnetto. (s.f.). _GitHub - jmcastagnetto/covid-19-peru-distribucion-poblacion-positivos-fallecidos: Gráficos comparativos de distribuciones poblacionales por grupo etáreo, para todo el Perú y por departamento_. Github. Recuperado el 1 de marzo de 2021 de https://github.com/jmcastagnetto/covid-19-peru-distribucion-poblacion-positivos-fallecidos   

