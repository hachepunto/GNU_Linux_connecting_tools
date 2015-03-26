# Herramientas para uso a distancia de sistemas GNU/Linux

![linux preacher](https://raw.github.com/hachepunto/GNU_Linux_connecting_tools/master/linux_preacher.jpg)

**[GNU/Linux](https://www.gnu.org/gnu/linux-and-gnu.html)** es un sistema operativo profesional y muy versátil.  Una de sus cualidades más socorridas, dada su estabilidad, poder y al mismo tiempo ligereza, es poder someter trabajos a distancia via internet o intranet y dejarlos corriendo en un servidor remoto. Por sus características multiproceso, multiusuario, este proceso se da de forma muy eficiente y transparente para el usuario. Este taller se enfocará en una serie de herramientas ([ssh](http://www.openssh.com/), [sshfs](http://fuse.sourceforge.net/sshfs.html), [Byobu](http://byobu.co/) y [X11](http://www.x.org/wiki/) via ssh) que permitirán maximizar estas cualidades. Éstas nos permitirán trabajar con un servidor remoto con el fin de someter trabajos y consultar resultados. El taller se originó con el objetivo de ayudar a [Carlos y sus alumnos](http://www.fciencias.unam.mx/investigacion/grupos/biologia/ecologia/ambientesl) con su servidor **[Debian](https://www.debian.org/)** pero, dado que vamos a hablar de [linea de comandos](http://es.wikipedia.org/wiki/L%C3%ADnea_de_comandos), muy probablemente a más personas les interese aprender algo más de estas herramientas o, simplemente, tenga curiosidad acerca de como son estos sistemas operativos. Conmigo me acompañarán entusiastas de este sistemas operativo y nos ayudarán a echar a andar las herramientas de forma más personalizada. Además ellos tienen un *[taller en el INMEGEN de instalación de GNU/Linux](http://lc3-inmegen.github.io/2015/02/27/installfest_permanente.html)* y seguramente les darán información si es que quieren [acercarse a estos sistemas operativos](http://www.getgnulinux.org/es/) de trabajo profesional.

## Herramientas que hay que instalar para el taller
#####En Mac:

+ **[XQuartz](http://xquartz.macosforge.org/landing/)** Manejador de ventanas de sistemas GNU/Linux para Mac.

+ **[OSXFuse](https://osxfuse.github.io/)** Monta sistemas de archivos remotos via sshfs.

#####En Windows:

+ **[PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/)** Emulador de terminal para Windows

+ **[CygWin](https://cygwin.com/index.html)** Una gran colección de herramientas de GNU y Open Source que proveen funcionalidad similar a una distribución Linux en Windows

+ **[win-sshfs](https://code.google.com/p/win-sshfs/)** sshfs para montar sistemas de archivos remotos en Win


#####En Linux:

+ **[ssh](http://www.openssh.com/)** Secure Shell es un protocolo para conecciones de red seguras y encriptadas. [Tutorial](http://blog.desdelinux.net/como-crear-un-tunel-ssh-entre-un-servidor-linux-y-un-cliente-windows/)

+ **[sshfs](http://fuse.sourceforge.net/sshfs.html)** Un cliente de sistema de archivos basado en el protocolo de transferencia de SSH. [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-use-sshfs-to-mount-remote-file-systems-over-ssh)

+ **[Byobu](https://www.digitalocean.com/community/tutorials/how-to-use-sshfs-to-mount-remote-file-systems-over-ssh)** Byobu es un entorno con esteroides para los multiplexotes de terminal GNU [Screen](https://www.gnu.org/software/screen/) o [tmux](http://tmux.sourceforge.net/). [Manual](http://manpages.ubuntu.com/manpages/oneiric/en/man1/byobu.1.html)


## Ligas de interes para Mac

+ **[HomeBrew](http://brew.sh/)**

+ **[Como instalar las Apple "commandline tools"](http://railsapps.github.io/xcode-command-line-tools.html)**

+ **[Como instalar las GNU command line tools con Brew](https://www.topbug.net/blog/2013/04/14/install-and-use-gnu-command-line-tools-in-mac-os-x/)**

## Liga de interes para Windows

+ **[Say goodbye to Microsoft. Now.](http://goodbye-microsoft.com/)**

