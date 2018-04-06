
**Mancilla Rojano Jetsi Viridiana**

*Avance 1. Proyecto final* 


Para el desarrollo del proyecto final, trabajaré con datos que forman parte de mi proyecto de maestría, el cual tiene por título:**Tipificación molecular de aislados de *Acinetobacter baumannii**.


### Descripción del proyecto :

*Acinetobacter baumanni* es una bacteria Gram negativa asociada a infecciones nosocomiales, principalmente, neumonía, infecciones en torrente sanguíneo, meningitis e infecciones de vías urinarias. *Acinetobacter baumannii* ha tomado relevancia clínica debido a que presenta resistencia a diferentes grupos de antibióticos, principalmente a carbapenémicos, por lo que las opciones terapéuticas se han reducido; aunado a esto, tiene la capacidad de sobrevivir en ambientes con baja disponibilidad de agua, lo que contribuye a su persistencia en entornos hospitalarios. Debido a lo anterior es importante implementar métodos que permitan una identificación más certera y por tanto una mejor vigilancia y control de brotes causados por esta bacteria; uno de los métodos de tipificación más utilizados es el MLST  (Multilocus Sequence Typing) , el cual se basa en la secuenciación de fragmentos de 7 genes conservados o *housekeeping*, las variaciones en las secuencias de estos genes permiten diferenciar distintas cepas de la misma especie.


Basándome en lo anterior la opción de trabajo final que realizaría es: **Análisis de datos propios**.


#### ¿Qué tipos de análisis realizaré?


Cuento con una colección de 69 cepas, aisladas de pacientes del Hospital Infantil de México Federico Gómez; para llevar a cabo el método de MLST, seleccioné 7 genes constitutivos y a través de la técnica de PCR amplifiqúe dichos genes, los productos fueron purificados y secuenciados mediante secuenciación masiva , utilizando la plataforma Illumina. Así mismo, de mi colección de cepas, seleccioné un aislado con base en los resultados que obtuve a través de otras técnicas de tipificación molecular y se mandó a secuenciar el genoma, utilizando la plataforma de PacBio e Illumina.  Con base en lo anterior, los análisis que realizaré serán **ensamblado de novo**.


#### Ensamblado de novo.

Los pasos que estoy considerando son los siguientes:

- Los datos que nos fueron proporcionados se encuentran en formato **FASTQ**; por lo que, el primer paso dentro de mi análisis debe ser el determinar la calidad de las secuencias; considerando el score, eliminaré las secuencias que presenten una baja calidad.

- Ensamblaje de secuencias. Se realizará la unión de los fragmentos de DNA para generar secuencias contiguas de un mayor tamaño y entonces poder reconstruir la secuencia. El software que pretendo utilizar es **Velvet**.

- Evaluación del ensamblaje. Una vez que se realice el ensamblado de las secuencias, se debe corroborar la calidad de las mismas ; la herramienta que estoy considerando utilizar es:  **QUAST** y **IMetAMOS** (se utiliza generalmente en el caso de bacterias).

- Tipificación de las cepas. A partir de las secuencias obtenidas, se realizará la tipificación de las cepas; para el caso de la técnica que estos utilizando (MLST) los datos son cargados en una base de datos: (http://pubmlst.org/) donde se van determinando nuevas secuencias para cada locus,asignando un número (el cual corresponde al orden de descubrimiento), al final obtendré un patrón de números de todos los loci para poder asignar un perfil alélico y por lo tanto una secuencia tipo.

- Análisis del genoma. Para el caso del aislado que se mandó a secuenciar el genoma, después de realizar el ensamblaje, se emplearan diferentes algoritmos para analizar el fenotipo de la cepa. En el caso de la bacteria con la que trabajo una de las características más importantes de identificar  es la presencia de genes de resistencia a antibióticos, para lo cuál podría emplear **ResFinder 2.0**; asi mismo, pretendo realizar una búsqueda de genes de virulencia y presencia de plásmidos , a través de los softwares **VirulenceFinder 1.2** y **PlasmidFinder 1.2**, respectivamente.



