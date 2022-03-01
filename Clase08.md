# Hadoop

* Framework de código abierto
* Desarrollado para trabajar con grande volúmenes de datos , distribuidos en nodos diferentes, suele ser muy rápido, ya que utiliza núcleo muy grande. 
* Posee almacenamiento distribuido 
* Procesamiento en paralelo 
* La licencia es tipo apache

## ¿Cómo funciona Hadoop?
* HDFS:
    - Sistema de archivos distribuidos de hadoop
    - Mestro-esclavo

* NameNode (Demonios)
    - Daemons que se ejecuta en la máquina maestra o    principal
    - Pieza central de un sistema de archivos HDFS 
    - Conexión de ssh, máquina virtual 

* Datanode
    - Daemons que se ejecuta en los nodos esclavos
    - Almacena datos en HDFS
    - Sistema de archivos funcional
    - Los datos se replican en diferentes DataNodes. 

Esta inspirando en el `algoritmo de MapReduce de google`, su objetivo es respaldar el motor de búsqueda Nuth (Motor de google). Versión vigente 2017. 


## Ventajas hadoop
* Acepta diferentes tipos de datos (txt,img,etc). Es muy útil para el estudio de imágenes, en donde se tengan grandes flujo de trabajo. 
* Rentable a nivel de hardware
* Alto desempeño
* Tolerancia a fallos. Cuando falla un nodo, se genera una réplica. 
* Alta disponibilidad
* Tráfico de red bajo
* Alta rendimiento. Capacidad de acelerar el proceso
* Código abierto
* Escalable horizontal
* Facilidad de uso
* Compatibilidad con otras plataforma como pyspark, apache, flink. 
* Multi-idiomas (Java, python, C, C++)


## Desventajas hadoop 
* Trabajar cocn archivos pequeños, puede ocasionar problemas.
* Vulnerable por su naturaleza java. Las interfaces suelen tener muchas vulnerabilidades. 
* Operaciones de escritura costosa. 
* Procesamiento por lotes.
* No permite procesamiento iterativo como ML 

## Componentes principales para instalación de proceso
* Hadoop
* HDFS
* Hadoop YARN
* Hadoop MapReduce


## Instalaciones 
* Modo autónomo
* Modo completamente distribuido
* Modo pseudo-distribuido
* Ecosistema de Hadoop (Herramientas como SQL e intérpretes  para otros lenguajes)
* El framework esta escrito en java
    - Java Runtine environment- JRE
    - Java Development Kit- JDK
* La versión compatible es Java 8 (opernjdk-8-jdk)
    - `supo apt install opernjdk-8-jdk-y`
* 

Base de datos médico: mimie 
