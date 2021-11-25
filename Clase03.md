# Protocolos de codificación en informática médica 

Fecha: 23/11/2021

Protocolos de información: HIS, LIS, RIS.

### CIE

**Clasificacion internacional y estadística de enfermedades y problemas relacionados con la salud- International statical classification of discases and related health problems**
Sigla CIE- Clasifiación internacional de enfermedades

Se utiliza a nivel internacional para fines estadísticos relacionados con:
1. Morbilidad
2. Mortalidad
3. Los sistemas de reíntegro
4. Soportes de decisión automática en medicina 

Este sistema esta diseñado para promover la comparación internacional de:
1. La recolección
2. Procesamiento
3. Clasificación
4. Presentación de estas estadísticas

Existen algunos paisen que han hecho adaptaciones de esta codificación internacional con los códigos y epidemiologías locales.

Por ejemplo:
* Australia 1era edición, la CIE-10-AM en 1998 
* Alemania: la CIE-10-GM
* Canadá publicó su versión en el 2000, la CIE-10-CA
* Colombia: CUPS- resolución 365 de 1999

### ¿Qué codifica la CIE?

Cada afección puede ser asignada a una categoría y recibir un código de hasta seis caracteres de longitud. 


### CIE-10-ES
Estas agrupados por códigos 
Ejemplo:

![picture 1](images/47bd63b60eac7559e4c3a7f862202246fe8aa4dc6ba884f93ad1b29420a91b89.png)  

![picture 2](images/f8c88ea5a494d2e8973e2f2a8877d48296dcab71ec7f9ca0e3637be30fa460e3.png)  

cómo codifica los diagnosticos la CIE
1. Primer codigo hace referencia al capitulo
![picture 3](images/b246406bd535748e8d64cabc6cd35edc0ef30582d470c5f7f09418a180eb3772.png)  

![picture 4](images/5a0bdefa65f1a523cc7b183703e183c28659b08d96b25232bb548a5b7b2ed966.png)  

### CUPS- Clasificación única de procedimientos en salud

Adopta procedimientos que relaciona la CIE10 

Es una lista tabular que consta de dos secciones:
* **Seccion 00**: procedimientos quirúrgicos 
![picture 5](images/8bd4bfc07d0d437a776e0b5b27ef6888661ef29a8b0ab259ba811dcbf03ad804.png)  

* **Seccion 01**: procedimientos no quirúrgicos 

![picture 6](images/f7fcaf9ff733290785795c9667e87c01fc6ae16eb7b0f03ba7ae81ae601b8063.png)  

Estas dos secciones contemplan los relacionado con el individuo. Cada secciín esta integrada por capítulos descritos por dos dígitos.

### Definición y uso de los GRD (grupos relacionados por el diagnostico) 

Sistemas de clasificación de pacientes que proveen medios para relacionar el tipo de pacientes que un hospital trata(es decur casuística), son los costos en que ese hosputal incurre

1. Monitoreo epidemiológico
2. La gestión clínica- Indicadores de mortalidad, promedio días de estancia y estimación de costos.
3. La comparación estandarizada de la actividad del hospital con otros hospitales
4. El presupuesto y planeación hospitalaria
5. El desarrollo e implementación de sistemas de pago prospectivo. 

Nace aproximadamente desde los 60's . En latinoamerica a finales de 2010 empezó.

Los Grupos Relacionados por el Diagnóstico (GRD) son algoritmos de agrupación de pacientes que ayudan a la gestión clínica y a la gestión financiera de hospitales y centros de atención sanitaria, cuya validez ha sido reconocida a nivel internacional. En los últimos años, estos algoritmos han adquirido gran relevancia en distintos países de América Latina. En el caso de Colombia, son muchas las IPS y EPS que están consiguiendo importantes avances en gestión clínica y gestión financiera gracias a su utilización.

![picture 7](images/e5b7676b68f187f63485e9d430d19777ab92e1358ee509a1c8867b88148f4c97.png)  


Información requerida para la clasificación en GRD

1. Datos de indentificación del paciente
    
    1.1 Identificación del paciente
    
    1.2 Fecha de nacimiento
    
    1.3 Sexo
    
    1.4 Municipio
    
    1.5 CIAS_PRO
2. Datos de identificación del episodio 
    2.1 Financiador

    2.2 Fecha de ingreso
    
    2.3 Tipo de ingreso
    
    2.4 Servicio responsable del alta 
    
    2.6 Área clínica
    
    2.7 Fecha de alta
    
    2.8 Médico
    
    2.9 Tipo de alta 
    
    2.10 Fecha de la intervención
3. Variable clínicas
    
    3.1 Diagnostico principal
    
    3.2 Diagnostico secundarios
    
    3.3 Procedimientos diagnósticos y terapéuticos
    
    3.4 Morgología de las neoplasías

Tener en cuenta que esta información solo se obtiene cuando el paciente se ha desplazado. 

**Ejemplo de clasificación**
![picture 8](images/af07e77da94950a9aab958c87436d67ccc576bdb98e01e50038ca8078b8cad6e.png)  

![picture 9](images/aa1b4358c11f67c7b1df78d6aecbcbc1772a680bf31d0184c183cddc84d62516.png)  

### Problemáticas actuales de estas codificaciones

1. Los códigos CIE y CUPS (para el caso de Colombia) se deben ingresar manualmente
2. En muchas ocasiones, el médico no es suficientemente específico en el código y hace que la codificación quede mal.
3. En ocasiones, no se actualizan los diagnósticos cuando estos cambian
4. Para el caso de los GRD, portan a la gestión en forma retrospectiva.
5. Si hay problemas de gestión con un paciente, no se puede hacer nada en el instante porque no hay evidencia. 

### Soluciones desde la IM

1. Utilizar procesamiento del lenguaje natural para **sugerir** códigos de diagnósticos y/o procedimientos a los médicos, con base en lo que este escriba en la HCE
2. Utilizar algoritmos de ML para clasificación, que prediga el GRD del paciente durante la estancia hospitalaria. 


