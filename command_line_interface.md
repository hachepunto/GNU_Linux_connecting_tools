# Interface de línea de comandos


## Preámbulo

La **[Interaface de línea de comandos](http://en.wikipedia.org/wiki/Command-line_interface)** (CLI) es un **método para interactual** con con un programa de computadora que permite al usuario dar órdenes al programa **en forma de lineas de texto** sucesivas (líneas de comando). 

La **CLI** es menos usada por el usuario de computadoras promedio que prefiere usar una **[Interface Gráfica de Usuario](http://en.wikipedia.org/wiki/Command-line_interface)** (GUI) que ofrece una estética mejorada y una mayor simplificación, a costa de un mayor consumo de recursos computacionales, y, en general, de una reducción de la funcionalidad alcanzable.

La **CLI**, sin embargo, es preferida por los usuarios avanzados de cómputo dado que ofrece medios más concisos y poderosos para controlar porgramas o sistemas operativos.


## Ejercicios [^1]

[^1]: Datos descargados de [este sitio web](https://daac.ornl.gov/VEGETATION/guides/niklas_plant_biomass.html)

Abre tu emulador de terminal y copia y pega uno por uno los siguientes comandos mientras explico:

***ls*** (list) es un programa para listar el contenido de la carpeta en la que estamos "parados".

```
$ ls
```
```
$ ls -la
```
***cd*** (change directory) es un programa para cambiar de directorio dentro del arbol de directorios del sistema.

```
$ cd
```
***mkdir*** (make directory) crea carpetas.

```
$ mkdir datos
```
```
$ cd datos
```
```
$ ls
```
***wget*** (www get) Es un programa para descargar archivos de internet.

```
$ wget https://raw.githubusercontent.com/hachepunto/GNU_Linux_connecting_tools/master/niklas_biomass_20040122.txt
```
```
$ ls
```
***cat*** (concatenate) sirve para concatenar archivos uno tras.

```
$ cat niklas_biomass_20040122.txt
```

***less*** es un paginador para ver archivos.

```
$ less niklas_biomass_20040122.txt
```
***man*** (manual) es un programa que muestra los manuales de los programas.

```
$ man less
```
```
$ less -S niklas_biomass_20040122.txt
```
***cut*** Corta por columnas un archivo.

```
$ cut -f1 niklas_biomass_20040122.txt
```
***pipeline*** ( **|** ) es un método para encadenar programas de tal modo que la salida de uno es la entrada del que sigue. Se usa una barra vertical para separar los programas a usar.

```
$ cut -f1 niklas_biomass_20040122.txt | less
```
***sort*** ordena listas.

``` 
$ cut -f1 niklas_biomass_20040122.txt | sort | less
```
***uniq*** busca repetidos en una lista ordenada.

```
$ cut -f1 niklas_biomass_20040122.txt | sort | uniq |less
```

```
$ cut -f1,5 niklas_biomass_20040122.txt | sort | uniq |less
```
***wc*** (word count) cuenta el número de palabras y de renglones.

```
$ cut -f1,5 niklas_biomass_20040122.txt | sort | uniq | wc -l
```
```
$ cut -f1,5 niklas_biomass_20040122.txt | sort | wc -l
```
***>*** salva a alrchivo la salida estándar.

``` 
$ cut -f1,5 niklas_biomass_20040122.txt | sort | uniq > niklas_col_1_5_uniq.txt
```
```
$ less niklas_col5.txt
```

***grep*** (get all lines matching the regular expression and print (g/re/p)) es un programa para buscar cadenas de texto dentro de un archivo.

```
$ grep Abies niklas_col5.txt | less
```
```
$ grep Abies niklas_col5.txt > abies.txt`
```

[Lista de comandos de UNIX en la Wikipedia](http://en.wikipedia.org/wiki/List_of_Unix_commands)




***
***

Si quieres explorar algunas otras bases de datos disponibles en la web puedes comenzar por este par de ligas:    
    
```
https://www.nceas.ucsb.edu/scicomp/data
```

```
http://ecologicaldata.org/
```