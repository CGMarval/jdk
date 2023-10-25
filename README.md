



# Instalación de JDK en el Ubuntu

Java sin dudas es un lenguaje de programación que es utilizado para diversos propósitos y es un complemento casi esencial para la ejecución y funcionamiento de diversas herramientas, la instalación de java es prácticamente una tarea esencial después de haber realizado la instalación de este.

Es por ello que en esta ocasión compartiré con ustedes un sencillo tutorial de como instalar Java en nuestro sistema con el JDK el cual es un entorno de desarrollo y el entorno de ejecución JRE.


**indice**

1. [¿Cómo instalar Java en Ubuntu desde repositorios?](#id1)

2. [¿Cómo instalar una versión específica de Java?](#id2)

3. [Configuración de las variables de entorno](#id3)


## ¿Cómo instalar Java en Ubuntu desde repositorios? <a name="id1"></a>

Lo primero debemos de actualizar el sistema con:

```code
  sudo apt-get update
```
e instalamos Java con este comando:

```code
  sudo apt-get install default-jdk
```  
comprobamos que tenemos instalado Java en nuestro sistema solo debemos de ejecutar:

```code
  java --version
```

<details><summary>Salida</summary>
 sudo apt-get update

```code
esteban@esteban-VirtualBox:~$ sudo apt-get update
[sudo] contraseña para esteban:       
Obj:1 http://packages.microsoft.com/repos/code stable InRelease
Obj:2 http://archive.ubuntu.com/ubuntu jammy InRelease                         
Ign:3 http://packages.linuxmint.com victoria InRelease                         
Obj:4 http://security.ubuntu.com/ubuntu jammy-security InRelease               
Obj:5 http://archive.ubuntu.com/ubuntu jammy-updates InRelease                 
Obj:6 https://dl.google.com/linux/chrome/deb stable InRelease                  
Obj:7 http://packages.linuxmint.com victoria Release                           
Obj:8 http://archive.ubuntu.com/ubuntu jammy-backports InRelease
Leyendo lista de paquetes... Hecho
```
sudo apt-get install default-jdk
```code
esteban@esteban-VirtualBox:~$ sudo apt-get install default-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
Se instalarán los siguientes paquetes adicionales:
  default-jdk-headless libice-dev libpthread-stubs0-dev libsm-dev libx11-dev
  libxau-dev libxcb1-dev libxdmcp-dev libxt-dev openjdk-11-jdk x11proto-dev
  xorg-sgml-doctools xtrans-dev
Paquetes sugeridos:
  libice-doc libsm-doc libx11-doc libxcb-doc libxt-doc openjdk-11-demo
  openjdk-11-source visualvm
Se instalarán los siguientes paquetes NUEVOS:
  default-jdk default-jdk-headless libice-dev libpthread-stubs0-dev libsm-dev
  libx11-dev libxau-dev libxcb1-dev libxdmcp-dev libxt-dev openjdk-11-jdk
  x11proto-dev xorg-sgml-doctools xtrans-dev
0 actualizados, 14 nuevos se instalarán, 0 para eliminar y 6 no actualizados.
Se necesita descargar 3.356 kB de archivos.
Se utilizarán 8.618 kB de espacio de disco adicional después de esta operación.
¿Desea continuar? [S/n] s
Des:1 http://archive.ubuntu.com/ubuntu jammy/main amd64 default-jdk-headless amd64 2:1.11-72build2 [942 B]
Des:2 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 openjdk-11-jdk amd64 11.0.20.1+1-0ubuntu1~22.04 [1.331 kB]
Des:3 http://archive.ubuntu.com/ubuntu jammy/main amd64 default-jdk amd64 2:1.11-72build2 [908 B]
Des:4 http://archive.ubuntu.com/ubuntu jammy/main amd64 xorg-sgml-doctools all 1:1.11-1.1 [10,9 kB]
Des:5 http://archive.ubuntu.com/ubuntu jammy/main amd64 x11proto-dev all 2021.5-1 [604 kB]
Des:6 http://archive.ubuntu.com/ubuntu jammy/main amd64 libice-dev amd64 2:1.0.10-1build2 [51,4 kB]
Des:7 http://archive.ubuntu.com/ubuntu jammy/main amd64 libpthread-stubs0-dev amd64 0.4-1build2 [5.516 B]
Des:8 http://archive.ubuntu.com/ubuntu jammy/main amd64 libsm-dev amd64 2:1.2.3-1build2 [18,1 kB]
Des:9 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxau-dev amd64 1:1.0.9-1build5 [9.724 B]
Des:10 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxdmcp-dev amd64 1:1.1.3-0ubuntu5 [26,5 kB]
Des:11 http://archive.ubuntu.com/ubuntu jammy/main amd64 xtrans-dev all 1.4.0-1 [68,9 kB]
Des:12 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxcb1-dev amd64 1.14-3ubuntu3 [86,5 kB]
Des:13 http://archive.ubuntu.com/ubuntu jammy-updates/main amd64 libx11-dev amd64 2:1.7.5-1ubuntu0.3 [744 kB]
Des:14 http://archive.ubuntu.com/ubuntu jammy/main amd64 libxt-dev amd64 1:1.2.1-1 [396 kB]
Descargados 3.356 kB en 2s (2.126 kB/s)
Seleccionando el paquete default-jdk-headless previamente no seleccionado.
(Leyendo la base de datos ... 603972 ficheros o directorios instalados actualmente.)
Preparando para desempaquetar .../00-default-jdk-headless_2%3a1.11-72build2_amd64.deb ...
Desempaquetando default-jdk-headless (2:1.11-72build2) ...
Seleccionando el paquete openjdk-11-jdk:amd64 previamente no seleccionado.
Preparando para desempaquetar .../01-openjdk-11-jdk_11.0.20.1+1-0ubuntu1~22.04_amd64.deb ...
Desempaquetando openjdk-11-jdk:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
Seleccionando el paquete default-jdk previamente no seleccionado.
Preparando para desempaquetar .../02-default-jdk_2%3a1.11-72build2_amd64.deb ...
Desempaquetando default-jdk (2:1.11-72build2) ...
Seleccionando el paquete xorg-sgml-doctools previamente no seleccionado.
Preparando para desempaquetar .../03-xorg-sgml-doctools_1%3a1.11-1.1_all.deb ...
Desempaquetando xorg-sgml-doctools (1:1.11-1.1) ...
Seleccionando el paquete x11proto-dev previamente no seleccionado.
Preparando para desempaquetar .../04-x11proto-dev_2021.5-1_all.deb ...
Desempaquetando x11proto-dev (2021.5-1) ...
Seleccionando el paquete libice-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../05-libice-dev_2%3a1.0.10-1build2_amd64.deb ...
Desempaquetando libice-dev:amd64 (2:1.0.10-1build2) ...
Seleccionando el paquete libpthread-stubs0-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../06-libpthread-stubs0-dev_0.4-1build2_amd64.deb ...
Desempaquetando libpthread-stubs0-dev:amd64 (0.4-1build2) ...
Seleccionando el paquete libsm-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../07-libsm-dev_2%3a1.2.3-1build2_amd64.deb ...
Desempaquetando libsm-dev:amd64 (2:1.2.3-1build2) ...
Seleccionando el paquete libxau-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../08-libxau-dev_1%3a1.0.9-1build5_amd64.deb ...
Desempaquetando libxau-dev:amd64 (1:1.0.9-1build5) ...
Seleccionando el paquete libxdmcp-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../09-libxdmcp-dev_1%3a1.1.3-0ubuntu5_amd64.deb ...
Desempaquetando libxdmcp-dev:amd64 (1:1.1.3-0ubuntu5) ...
Seleccionando el paquete xtrans-dev previamente no seleccionado.
Preparando para desempaquetar .../10-xtrans-dev_1.4.0-1_all.deb ...
Desempaquetando xtrans-dev (1.4.0-1) ...
Seleccionando el paquete libxcb1-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../11-libxcb1-dev_1.14-3ubuntu3_amd64.deb ...
Desempaquetando libxcb1-dev:amd64 (1.14-3ubuntu3) ...
Seleccionando el paquete libx11-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../12-libx11-dev_2%3a1.7.5-1ubuntu0.3_amd64.deb ...
Desempaquetando libx11-dev:amd64 (2:1.7.5-1ubuntu0.3) ...
Seleccionando el paquete libxt-dev:amd64 previamente no seleccionado.
Preparando para desempaquetar .../13-libxt-dev_1%3a1.2.1-1_amd64.deb ...
Desempaquetando libxt-dev:amd64 (1:1.2.1-1) ...
Configurando libpthread-stubs0-dev:amd64 (0.4-1build2) ...
Configurando xtrans-dev (1.4.0-1) ...
Configurando default-jdk-headless (2:1.11-72build2) ...
Configurando openjdk-11-jdk:amd64 (11.0.20.1+1-0ubuntu1~22.04) ...
update-alternatives: utilizando /usr/lib/jvm/java-11-openjdk-amd64/bin/jconsole para proveer /usr/bin/jconsole (jconsole) en modo automático
Configurando xorg-sgml-doctools (1:1.11-1.1) ...
Configurando default-jdk (2:1.11-72build2) ...
Procesando disparadores para sgml-base (1.30) ...
Configurando x11proto-dev (2021.5-1) ...
Configurando libxau-dev:amd64 (1:1.0.9-1build5) ...
Configurando libice-dev:amd64 (2:1.0.10-1build2) ...
Configurando libsm-dev:amd64 (2:1.2.3-1build2) ...
Procesando disparadores para man-db (2.10.2-1) ...
Configurando libxdmcp-dev:amd64 (1:1.1.3-0ubuntu5) ...
Configurando libxcb1-dev:amd64 (1.14-3ubuntu3) ...
Configurando libx11-dev:amd64 (2:1.7.5-1ubuntu0.3) ...
Configurando libxt-dev:amd64 (1:1.2.1-1) ...
```

java --version
```code
esteban@esteban-VirtualBox:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)
```
</details>

## ¿Cómo instalar una versión específica de Java? <a name="id2"></a>
Para instalar Ubuntu Java Open JDK ("la que utilizaremos en 1º").

- OpenJDK:
  - 11Configuración de las variables de entorno

```code
sudo apt install openjdk-11-jdk
```
<details><summary>Salida</summary>
sudo apt install openjdk-11-jdk

```code
esteban@esteban-VirtualBox:~$ sudo apt install openjdk-11-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
openjdk-11-jdk ya está en su versión más reciente (11.0.20.1+1-0ubuntu1~22.04).
fijado openjdk-11-jdk como instalado manualmente.
0 actualizados, 0 nuevos se instalarán, 0 para eliminar y 6 no actualizados.
```
</details>

  - 13

```code
sudo apt install openjdk-13-jdk
```

<details><summary>Salida</summary>
sudo apt install openjdk-13-jdk

```code
esteban@esteban-VirtualBox:~$ sudo apt install openjdk-13-jdk
Leyendo lista de paquetes... Hecho
Creando árbol de dependencias... Hecho
Leyendo la información de estado... Hecho
E: No se ha podido localizar el paquete openjdk-13-jdk
```
</details>
  - 8

```code
sudo apt install openjdk-8-jdk
```
<details><summary>Salida</summary>
sudo apt install openjdk-8-jdkConfiguración de las variables de entorno
  openjdk-8-demo openjdk-8-source visualvm fonts-nanum fonts-ipafont-gothic
  fonts-ipafont-mincho fonts-wqy-microhei fonts-wqy-zenhei
Se instalarán los siguientes paquetes NUEVOS:
  fonts-dejavu-extra libatk-wrapper-java libatk-wrapper-java-jni openjdk-8-jdk
  openjdk-8-jdk-headless openjdk-8-jre openjdk-8-jre-headless
0 actualizados, 7 nuevos se instalarán, 0 para eliminar y 6 no actualizados.
Se necesita descargar 45,8 MB de archivos.
Se utilizarán 156 MB de espacio de disco adicional después de esta operación.
¿Desea continuar? [S/n] s
Des:1 http://archive.ubuntu.com/ubuntu jammy/main amd64 fonts-dejavu-extra all 2.37-2build1 [2.041 kB]
Des:2 http://archive.ubuntu.com/ubuntu jammy/main amd64 libatk-wrapper-java all 0.38.0-5build1 [53,1 kB]
Des:3 http://archive.ubuntu.com/ubuntu jammy/main amd64 libatk-wrapper-java-jni amd64 0.38.0-5build1 [49,0 kB]
Des:4 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jre-headless amd64 8u382-ga-1~22.04.1 [30,8 MB]
Des:5 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jre amd64 8u382-ga-1~22.04.1 [75,4 kB]
Des:6 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jdk-headless amd64 8u382-ga-1~22.04.1 [8.851 kB]
Des:7 http://archive.ubuntu.com/ubuntu jammy-updates/universe amd64 openjdk-8-jdk amd64 8u382-ga-1~22.04.1 [3.943 kB]
Descargados 45,8 MB en 4s (12,6 MB/s)   Configuración de las variables de entornojava-jni:amd64 previamente no selecciona
do.
Preparando para desempaquetar .../2-libatk-wrapper-java-jni_0.38.0-5build1_amd64
.deb ...
Desempaquetando libatk-wrapper-java-jni:amd64 (0.38.0-5build1) ...
Seleccionando el paquete openjdk-8-jre-headless:amd64 previamente no seleccionad
o.Configuración de las variables de entornodk-8-jdk-headless_8u382-ga-1~22.04.1_am
d64.deb ...
Desempaquetando openjdk-8-jdk-headless:amd64 (8u382-ga-1~22.04.1) ...
Seleccionando el paquete openjdk-8-jdk:amd64 previamente no seleccionado.
Preparando para desempaquetar .../6-openjdk-8-jdk_8u382-ga-1~22.04.1_amd64.deb .
..
Desempaquetando openjdk-8-jdk:amd64 (8u382-ga-1~22.04.1) ...
Configurando openjdk-8-jre-headless:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/orbd p
ara proveer /usr/bin/orbd (orbd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/server
tool para proveer /usr/bin/servertool (servertool) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/tnames
erv para proveer /usr/bin/tnameserv (tnameserv) en modo automático
Configurando fonts-dejavu-extra (2.37-2build1) ...
Configurando libatk-wrapper-java (0.38.0-5build1) ...
Configurando libatk-wrapper-java-jni:amd64 (0.38.0-5build1) ...
Configurando openjdk-8-jdk-headless:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/clhsdb par
a proveer /usr/bin/clhsdb (clhsdb) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/extcheck p
ara proveer /usr/bin/extcheck (extcheck) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/hsdb para 
proveer /usr/bin/hsdb (hsdb) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/idlj para 
proveer /usr/bin/idlj (idlj) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/javah para
 proveer /usr/bin/javah (javah) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/jhat para 
proveer /usr/bin/jhat (jhat) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/jsadebugd 
para proveer /usr/bin/jsadebugd (jsadebugd) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/native2asc
ii para proveer /usr/bin/native2ascii (native2ascii) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/schemagen 
para proveer /usr/bin/schemagen (schemagen) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/wsgen para
 proveer /usr/bin/wsgen (wsgen) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/wsimport p
ara proveer /usr/bin/wsimport (wsimport) en modo automático
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/xjc para p
roveer /usr/bin/xjc (xjc) en modo automático
Configurando openjdk-8-jre:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/policy
tool para proveer /usr/bin/policytool (policytool) en modo automático
Configurando openjdk-8-jdk:amd64 (8u382-ga-1~22.04.1) ...
update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/bin/appletview
er para proveer /usr/bin/appletviewer (appletviewer) en modo automático
Procesando disparadores para fontconfig (2.13.1-4.2ubuntu5) ...
Procesando disparadores para desktop-file-utils (0.26+mint3+victoria) ...
Procesando disparadores para hicolor-icon-theme (0.17-2) ...
Procesando disparadores para gnome-menus (3.36.0-1ubuntu3) ...
Procesando disparadores para libc-bin (2.35-0ubuntu3.4) ...
Procesando disparadores para mailcap (3.70+nmu1ubuntu1) ...
```
</details>

La versión que se debe de trabajar es la versión 8. Para ello verificaremos la versión de java que se esta ejecutando con la sentencia:

```code
java --version
```  
<details><summary>Salida</summary>

```code
esteban@esteban-VirtualBox:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)
```
</details>

En caso que no se ejecuta la versión 8 se debe configurar las variables de entorno.


## Configuración de las variables de entorno <a name="id3"></a>
El siguiente paso consiste en establecer las variables de entorno. Es necesario porque cuando se usa Java, Linux necesita saber dónde está ubicado el programa para ejecutarlo y qué versión de Java usar de forma predeterminada. Para modificar esto, usaremos el editor de texto nano. Primero, abra el archivo en Nano.

#### Listar la versiones de OpenJDK instaladas
Ejecuta el siguiente comando para verificar que se han descargado las diferentes versiones de OpenJDK.

```code
 ls /usr/lib/jvm
```
<details><summary>Salida</summary>

```code
esteban@esteban-VirtualBox:~$ java --version
openjdk 11.0.20.1 2023-08-24
OpenJDK Runtime Environment (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04)
OpenJDK 64-Bit Server VM (build 11.0.20.1+1-post-Ubuntu-0ubuntu122.04, mixed mode, sharing)
```
</details>

#### Actualización de las variables de entorno
Edita y modifica el fichero profile, con los comandos:

```code
sudo update-alternatives --config java
```
<details><summary>Salida</summary>

```code
esteban@esteban-VirtualBox:~$ sudo update-alternatives --config java
Existen 2 opciones para la alternativa java (que provee /usr/bin/java).

  Selección   Ruta                                            Prioridad  Estado
------------------------------------------------------------
* 0            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      modo automático
  1            /usr/lib/jvm/java-11-openjdk-amd64/bin/java      1111      modo manual
  2            /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java   1081      modo manual

Pulse <Intro> para mantener el valor por omisión [*] o pulse un número de selección:  

```
</details>

y selecciona la version 8.

<details><summary>Salida</summary>

```code
selecionamos la versión 8:

update-alternatives: utilizando /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java para proveer /usr/bin/java (java) en modo manual
```
</details>



Otra opción es : añadir el siguiente código:

```code
# Java version
JAVA_HOME=/usr/lib/jvm/(SELECCIONA UN PATH DE LA VERSION QUE DESEAS QUE SE EJECUTE)
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
```

en 

```code
/etc/profile.d/java.sh
```

Haga que el script sea ejecutable con chmod:

```code
sudo chmod +x /etc/profile.d/java.sh
```

Finalmente, cargue las variables de entorno usando el comando de source

```code
source /etc/profile.d/java.sh
```


Realizado por: Cleyber Esteban García Marval
Curso: 1º DAM
Nº lista: 8