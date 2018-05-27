
## Ensamble de las secuencias


1.	Descargar el ensamblador Velvet:

$ wget –b http://www.ebi.ac.uk/~zerbino/velvet/velvet_1.2.09.tgz

2.	Para descomprimir el paquete:

$ tar –xvf velvet_1.2.09.tgz 
$ cd velvet_1.2.09.


3.	Para instalar: 

$ make “OPENMP=1” “CATEGORIES=4” “MAXKMERLENGTH=65”

Es importante mencionar que los parámetros anteriores consideran que las variables que vamos asignar a nuestro trabajo. OPENMP, considera las CPUs con la que cuenta la máquina en la que vamos a trabajar; CATEGORIES, permite que el ensamblador pueda diferenciar las categorías que vamos a utilizar; MAXKMERLENGTH, considera el valor máximo de K que se puede asignar. Así mismo, es importante mencionar también que se tienen que ejecutar otras librerías como ShuffleSequences_fastq.pl, velveth y velvetg, para determinar y observar otros parámetros adicionales al ensamble. 
