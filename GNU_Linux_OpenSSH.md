# OpenSSH

## Preámbulo

**OpenSSH** (Open Secure Shell) o **SSH** es un conjunto de herramientas para la comunicación segura entre computadoras usando el protocolo ssh. **OpenSSH** fue desarrollado como alternativa libre y de código abierto a la implementación SSH propietaria.
**OpenSSH** es en realidad un conjunto de programas que ofrecen una alternativa a los protocolos de comunicación via red no encriptados como FTP.

## Ejercicios

Abre tu emulador de terminal y copia y pega uno por uno los siguientes comandos mientras explico:

Conección con un servidor SSH

```
$ ssh <usuario>@192.168.41.92 -p 344
```

```
$ cd
```

```
$ ls
```

```
$ R
```

```
> install.packages("EcoSimR")
```

```
> q()
```

Arrancar Byobu

```
$ byobu
```

¿Notaron que de lindo es ;¬)


```
$ cd
```

```
$ ls
```

```
$ mkdir ejercicioSSH
```

```
$ cd ejercicioSSH
```

```
$ wget https://raw.githubusercontent.com/hachepunto/GNU_Linux_connecting_tools/master/data/3958.csv
```

Arrancamos R (en amigo de todos los biólogos).

```
$ R
```

```
> library(EcoSimR)
```

```
> alt1 <- read.csv("3958.csv",row.names=1)
```

```
> alt1
```

```
> modAlt1 <- cooc_null_model(alt1, algo="sim9",nReps=10000,burn_in = 500)
```

```
> summary(modAlt1)
```

```
> pdf(file = "modAlt1.pdf")
plot(modAlt1,type="burn_in")
plot(modAlt1,type="hist")
plot(modAlt1,type="cooc")
dev.off()
```

```
> save.image("modAlt1.RData")
```

```
> q()
```

Salimos de Byobu.

```
$ exit
```

Cerramos la coneción SSH

```
$ exit
```

Iniciamos la conección con las X activadas ("C" es de compresión). Los maqueros necesitan arrancar X11 o XQuartz.

```
$ ssh -XC <usuario>@192.168.41.92 -p 344 
```

Arrancamos Rstudio

```
rstudio
```

```
> setwd("~/ejercicioSSH")
```

```
> load("modAlt1.RData")
```

```
> plot(modAlt1,type="burn_in")
```

Desde una terminal parada en nuestra computadora

```
$ cd
```

```
$ mkdir ejercicioSSH
```

```
$ sshfs <usuario>@192.168.41.92 ~/mirmecoleon -p 344 -o local -o volname=mirmecoleon 
```

Busca tu disco mirmecoleon.

Para desmontar:

```
$ fusermount -u mirmecoleon
```

O bien expulsa como siempre haces con un dispositivo externo.