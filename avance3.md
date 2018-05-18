
## Mancilla Rojano Jetsi Viridana 

*Avance 2. Proyecto Final*

Hasta el momento he realizado la limpieza de mis secuencias.Los datos que nos fueron proporcionados se encuentraban en formato FASTQ; por lo que, el primer paso dentro de mi análisis era determinar la calidad de las secuencias. Al realizar este análisis, y revisar la calidad y las coberturas de cada cepa, me encontré con que estos presentan profundidades superioes a 1000X. Además, hubo secuencias que presentan errores en la corrida reversa, lo que supongo es debido a un problema en los reactivos o el equipo que se utilizó para la secuenciación. 

Con los datos que he obtenido hasta el momento he generado una base de datos que incluye tablas en donde señaló datos como:

- Longitud de la región que se secuenció y presenta una profundidad mayor a 20X
- El porcentaje del gen completo que se cubrió. En este punto tengo muchas dudas, debido a que observó que hay cepas en las que practicamente se logró secuenciar nada de algunos genes. 
-Profundidad de la región secuenciada. 

Con base en lo anterior, y debido a que hay secuencias que no cumplen con la profundidad necesaria para ensamblar las secuencias o bien la longitud necesaria, he eliminado 10 de mis cepas. 

Por ahora , me encuentro  profundizando más sobre como se lleva a cabo la secuenciación en Illumina, para poder identificar correctamente si los errrores en la secuenciación si se deben al método que se utilizó o bien puede haber otros factores externos, como el protocolo que utilicé para la amplificación de genes; lo anterior lo mencionó, porque para el caso de bacterias y de esta técnica de tipificación (MLST) existen bases de datos y por lo tanto protocolos ya establecidos; en donde utilizas iniciadores que ya se encuentran diseñados, de los cuales yo hicé un análisis previó para confirmar que estos se estuvieran "alineando o pegando" en las secuencias de los genes de interes.

La base de datos en la cuál se puede consultar la secuencias tipo y los protocolos que se deben seguir para la técnica del MLST , es la siguiente: https://pubmlst.org/abaumannii/
