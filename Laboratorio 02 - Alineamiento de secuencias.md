Laboratorio 02 - Alineamiento de secuencias.

### Parte 1: Colectar genes homólogos


**1.** ¿Qué función cumple el gen SRY?
Según la base de datos de la NCBI este gen codifica un factor de transcripción que es un tipo de proteínas de unión a ADN del grupo de alta movilidad (HMG). Esta proteína es el factor determinante de los testículos (TDF), que inicia la determinación del sexo masculino. [NCBI](https://www.ncbi.nlm.nih.gov/gene/6736)

**2.** ¿Cuántos genes ortólogos están anotados en esa base de datos?
Según la NBCI el gen SRY consta de 29 genes ortólogos en distintas especies. [NCBI](https://www.ncbi.nlm.nih.gov/gene/6736#general-gene-info)

https://github.com/YarabiConchaVillagran/Informe-2./blob/master/Secuencia.FASTA.txt



### Parte 2: Alineamiento múltiple

**3.** ¿Qué es el EMBL-EBI?
Por lo encontrado en la NCBI el EML-EBI es una colección completa de secuencias de nucleótidos primarios mantenidas en el Instituto Europeo de Bioinformática (EBI). [NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC102461/)

**4.** ¿Cuál es el programa que ellos ofrecen que funciona mejor para secuencias de proteínas? Según la plataforma de EMBL-EBI, el mejor programa para secuencias de proteína es MUSCLE. [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/)

**5.** ¿Qué otros tipo de herramientas ofrece EMBL-EBI?
. Según lo visto en el portal de EMBL-EBI se ofrece una variedad de herramientas de alineacion ya sea de proteinas, alineamiento multiple y alineamiento de una sola linea grande, medianas y pequeñas tomando así conceptos como la filogenia y la información evolutiva. [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/)

---

**6.** ¿Cuál es el costo de abrir un gap?
Según EMBL-EBI un Gap tiene un costo de 1,53. [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/mafft/)

**7.** ¿Cuál es el costo de extender un gap? [1]
Según EMBL-EBI el costo de extender un Gap es de 0,123 [EMBL-EBI](https://www.ebi.ac.uk/Tools/msa/mafft/)

**8.** ¿Cuál es la longitud total del alineamiento?

Segú lo visto en el programa utilizado para realizarel alineamiento este tiene una longitud de 1902.

![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Captura%201.PNG)

![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Filogenia.PNG)

---

**9.** ¿Cuál es la especie cuyo gen SRY está más relacionado con el gen SRY de humanos?

Segun la base de datos de EMBL-EBI usando la herramienta MAFFT la especie cuyo gen SRY más esta relacionado con el SRY en humanos es "Piliocolobus tephrosceles" [EMBL-EBI](https://www.ebi.ac.uk/Tools/services/web/toolresult.ebi?jobId=mafft-I20180815-023649-0836-34616339-p1m&analysis=phylotree)

**10.** ¿Cuál es el más lejano?

Segun la base de datos de EMBL-EBI usando la herramienta MAFFT el gen más lejano son de las especies "Bos indicus" y "Bison bison" [EMBL-EBI](https://www.ebi.ac.uk/Tools/services/web/toolresult.ebi?jobId=mafft-I20180815-023649-0836-34616339-p1m&analysis=phylotree)

**11.** ¿Cuál es la especie cuyo gen SRY es más cercana a la del burro?

Segun la base de datos de EMBL-EBI usando la herramienta MAFFT "Equus przewalskii" [EMBL-EBI](https://www.ebi.ac.uk/Tools/services/web/toolresult.ebi?jobId=mafft-I20180815-023649-0836-34616339-p1m&analysis=phylotree)

---

**12.** ¿Cómo esperas que sea el alineamiento si el costo de abrir un gap aumenta? ¿Y si disminuye?

Segun lo observado en el caso de aumentar el costo de abrir un Gap se veran muchas mas extenciones de él en coparacion de cuando el Gap tiene un costo menor como se puede ver en la siguientes imagenes. 

![Gap 1,53](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/1%2C53.PNG)

![Gap 2,0](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/2%2C0.PNG)



**13.** ¿Cómo esperas que sea el alineamiento si el costo de extender un gap aumenta? ¿Y si disminuye?

Como se observa se aument el costo de exterder un Gap se pueden visualizar menos extenciones de él, por el contrario cuando dsiminuye su valor se ven mas extenciones como se ve en las siguientes imagenes.

![Extencion Gap 0,123](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/0%2C123.PNG)

![Extencion Gap 0,300](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/0%2C300.PNG)

---

**14.** ¿Cuál fue el efecto de aumentar el costo de abrir un gap en la longitud total del alineamiento?

Al aumentar al máximo el costo del Gap se puede ver que existen mas extenciones comparandola con la que esta por defecto en la herramienta MAFFT.

![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/Gap%203.PNG)

**15.** Prueba lo mismo, pero esta vez **disminuyendo al mínimo el costo de extender un gap**. Describe cómo cambia el alineamiento. 

En este caso, al disminuir al minimo el costo de extender un Gap se puede visualizar que exiten mucho mas extenciones si la compamos con los valores por defecto que tiene la herraimenta utilizada.

![](https://raw.githubusercontent.com/YarabiConchaVillagran/Informe-2./master/ext%200%2C001.PNG)



#### Parte 3: Diseño de partidores



**16.** Agrega a tu informe una lista de los "_LEFT PRIMER_" y "_RIGHT PRIMER_" que obtuviste usando Primer3.

LEFT PRIMER: TTACAGGCCATGCACAGAGA, GGATAGAGTGAAGCGACCCA, AGATGCTGCCGAAGAATTGC, CGAAGATGCTGCCGAAGAAT.

RIGHT PRIMER: CTTGAGTGTGTGGCTTTCGT, TTTCTCTCTGTGCATGGCCT, GCTTTGTCCAGTGGCTGTAG, CTACAGCTTTGTCCAGTGGC. [Primer3](http://primer3.ut.ee/cgi-bin/primer3/primer3web_results.cgi)

**17.** Indica los partidores _forward_ y _reverse_ que escogiste y explica por qué son la mejor opción para amplificar el gen SRY de humano.

Por lo analizado en el programa "AmplifX" se puede decir que los partidores (forward y reverse) que son la mejor opcion son los siguientes: AGATGCTGCCGAAGAATTGC, GCTTTGTCCAGTGGCTGTAG y CGAAGATGCTGCCGAAGAAT, CTACAGCTTTGTCCAGTGGC. debido a que estos secuencian un mayor porcentaje de bases nitrogenadas Guanina y Citosina (56%) lo cual hace la secuencia mucho más estable, ya que estas tienen 3 puntes de hidrógeno.

**18.** ¿Cuál es el largo del amplicón? ¿Y la temperatura de _annealing_ sugerida?

El largo del primero nombrado es de 204 pb y su temperatura de alineamiento sugerida es de 55°C. En cuanto al segundo primer nombrado, este tiene un largo de 212 pb y su temperatura de alineamiento sugerida es de 55°C siendo asi igual que el anterior.

​	