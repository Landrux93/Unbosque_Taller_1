# Taller_1

-Instalación de PySpark en Linux Ubuntu 21.10
  sudo apt install openjdk-11-jdk

-Verificamos la version de java instalada
  java --versión

-Creamos la variable JAVA_HOME
  sudo vim ~/.bashrc

-Escribimos el siguiente texto en la ventana abierta ( Para editar presionamos la letra "i" y para salir del modo edicion presionamos Esc y luego escribimo ":wq" para guardar los cambios y regresar a la terminar).
-Debemos colocar la ruta donde tenemos la carpeta con la jdk.
  export JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64

-Ejecutamos el archivo bashrc.
  source ~/.bashrc

-Descargamos spark del siguiente link:
  https://spark.apache.org/downloads.html
-Para esta instalación usamos la versión 3.2.1

-Descomprimimos el archivo tgz.
-Tenemos una carpeta con el nombre spark-3.2.1-bin-hadoop3.2
-Creamos la variable SPARK_HOME y PATH
  sudo vim ~/.bashrc
  
-Escribimos las siguientes variables.
export SPARK_HOME=/"ruta de la carpeta"/spark-3.2.1-bin-hadoop3.2
export PATH=$PATH.$SPARK_HOME/bin

-Ejecutamos el archivo bashrc.
  source ~/.bashrc
  
-Ejecutamos el comando spark-shell para verificar una instalación correcta. y nos debe salir la siguiente imagen:

Spark session available as 'spark'.
Welcome to
      ____              __
     / __/__  ___ _____/ /__
    _\ \/ _ \/ _ `/ __/  '_/
   /___/ .__/\_,_/_/ /_/\_\   version 3.2.1
      /_/
         
Using Scala version 2.12.15 (OpenJDK 64-Bit Server VM, Java 11.0.14)
Type in expressions to have them evaluated.
Type :help for more information.

-Instalamos  Python-pip , Python 3 ya viene instalado en esta versión de Linux
  sudo apt update
  sudo apt install python3-pip
  
-Instalamos JupyterLAb
  sudo pip install jupyterlab

-Creamos la variable SPARK_HOME y PATH
  sudo vim ~/.bashrc
  
-Escribimos las siguientes variables.
export PYSPARK_PYTHON=/usr/bin/python3

-Ejecutamos el archivo bashrc.
  source ~/.bashrc  
-Ya tenemos instalado Spark, solo ejecutamos Jupyter lab y empezamos a programar.
