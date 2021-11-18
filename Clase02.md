# Informática médica- parte 2

Fecha: 18/11/2021

### Definición 

La informática médica es la disciplina que aplica las herramientas de las tecnologías de la información y la comunicación TICs al contexto de la medicina 

### Contexto historico
* *Historia clínica impresa* -> Historias clínicas electronicas. Información sensible. 

* *Laboratorio clínico*- automatización de procesos y reportes como hemogramas, medición de pH de orina u otros fluidos. 

* *Imágenes diagnósticas* -> En los procesos de imagenología paso de tener procesos de rebelación de imágenes a automatización.

* *Gestión de equipos biomédicos* -> Se legisló más o menos alrededor del 2005 en Colombia la importación, almacenamiento, distribución de equipos biomédicos sin embargo toda esta información se almacenaba de forma manual.

* *Calibración de equipos biomédicos

* *Sistema de llamado de enfermería*, ha evolucionado el tema de alarmas haciendo uso de IOT con la finalidad de mejorar la comunicación paciente-personal médico.

* *Sistemas de Home care* creció el tema de la teleasistencia cargando todo el registro a una base de datos. 

**"La informática medíca tiene como principal objetivo optimizar la *adquisición*, el *almacenamiento*, la *recuperación* y el *uso* de la información en salud."**

### Sistematización de los procesos 

Cómo adquiero los datos a traves de unos protocolos, cómo y dónde los almaceno. 

**Ventajas**
1. Agilidad de los procesos
2. Seguridad en la información
3. Disminución del error humano 
4. Facilidad en el análisis de la información
5. Disminución de costos por insumos

**Desventajas**
1. Pocas habilidades informáticas por parte de los usuarios.
2. Poca disponibilidad de programas que cubrieron las necesidades del momento 

### Diversidad en lenguajes de programación

Se manejaban muchos lenguajes de programación en las diferentes áreas de la medicina, por tanto había una desconexión entre área y área. Sin embargo se requiere una interoperabilidad.

* La informática médica apunta a estandarizar todos estos procesos. 

* Python actualmente a surgido con el tema de machine learning. 

El ambiente hospitalario esta dividido en especialidades clínicas que frecuentemente tratan a los pacientes sin considerar el manejo de otros equipos médicos. Mientras que los procesos de cobro y facturación se valen de abstracciones fragmentadas.

La IM propone mejorar la comunicación entre las diversas áreas involucradas en la atención de la salud. 

### Estándares de comunicación

Un estándar comprende un grupo de reglas y definiciones que especifican cómo llevar a cabo un proceso. 

**Ventajas**
1. Ayuda a armonizar los métodos de gestión
2. Análisis de información:
    - Empleo de un lenguaje común

El uso de un lenguaje estándar permite:
1. El intercambio de información entre sistemas de historias clínicas electrónicas (HCE)
2. Favorece la extracción eficiente de información de las bases de datos
3. Contribuye al desarrollo de sistemas de soporte diagnóstico. Predicción.
4. Habilita la minería de datos. Ya se puede extraer información.
5. Facilita la evaluación estadística.

### Necesidad de estándares en IM

Las fuentes de información son un respaldo para el ejercicio médico y esta disponible de la siguiente forma:

1. Repositorios de datos epidemiológicos y de salud públilca. 
2. Repositorios de datos bioinformáticos (datos genómicos, proteómicos, metabolómicos, etc).
3. Bases de datos de literatura cientifica
4. Sistemas de registro 

### Tipos de estándares

Toda la información en estos repositorios o bases de datos esta codificada segun unos estándares: 
1. **ICD-II: International statical classification**

**CIE-11** (Clasificación Internacional de Enfermedades): Clasificacion internacional y estadiística de enfermedades y problemas relacionados con la salud.

Son códigos que el médico le pone al paciente en la historia clínica. 

**Ejemplo:**
- **I11**: Enfermedad cardiaca hipertensiva

- **I110**: Enfermedad cardiaca hipertensiva con insuficiencia cardiaca (congestiva)

- **I119**: Enfermedad cardiaca hipertensiva sin insuficiencia cardiaca (Congestiva)

2. **CUPS** (Clasificación única de procedimientos en salud). Creo códigos CUPS, con codificación colombiana. 

**Ejemplo:**
**796970**: Lavado y desbridamiento de fractura abierta de huesos faciales. 

3. **GRD- grupos relacionados por el diagnóstico**

DRG- Diagnosis related groug. Es un algoritmo. 

4. **Health level seven (HL7)**: indican como se organia y comunica la información entre dos partes. Definen el idioma, la estructura y los tipos de datos requeridos para una integración fluida entre. 

### Importancia de la codificación

1. Ahorra tiempo en el desarrollo de sistemas.
2. Facilitaría el intercambio de información entre sistemas.
3. Contribuye a limitar el uso de palabras o terminologías distintas.

### Protocolos de comunicación de equipos biomédicos

* Serial
* Json - Protocolos etiquedos
* Xml
* DICOM - protocolos para imágenes

### Sistema de información hospitalaria (HIS)
Evolución del HIS, se agrupa toda la gestión hospitalaria, hay interoperabilidad entre las diferentes áreas. 

