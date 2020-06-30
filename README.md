_Este repositorio corresponde al programa de mentorías de la Diplomatura en Ciencias de Datos, FaMAF, UNC._

# Introducción 

## Título de la mentoría: 
Predicción de ausentismo de pacientes en una institución de salud

## Mentor: 
Nahuel Almeira

## Grupo: 
1
 
### Integrantes:

+ Gianuzzi Emmanuel

+ Lascano Lucas

+ Salgado Cristian

## Página de la diplomatura:
[http://diplodatos.famaf.unc.edu.ar/](http://diplodatos.famaf.unc.edu.ar/)

## Problemática asociada a la mentoría:

En esta mentoría trabajaremos con datos de una institución de salud de la Ciudad de Córdoba y la problemática que abordaremos será el ausentismo de los pacientes. 
El ausentismo de los pacientes genera pérdidas económicas en la institución, ya que los turnos asignados que no se efectivizan suponen una distribución ineficiente de recursos. La relevancia económica es tal, que la problemática es ampliamente estudiada en todo el mundo.

El sistema de salud de Argentina presenta características que lo diferencian del resto de los países, particularmente de los sistemas europeos y norteamericanos, donde se realiza la mayor cantidad de investigación. Por eso, es importante estudiar datos de instituciones locales. En ese sentido, utilizaremos como referencia una tesis realizada con datos similares, correspondientes a una institución de la provincia de Buenos Aires.

Buscaremos identificar las variables que conllevan al ausentismo, y construir modelos que permitan predecir la probabilidad de que los turnos no sean atendidos. Evaluaremos la relevancia de cada conjunto de variables (administrativas, de pacientes, meteorológicas). 
Con esta información, la institución podría implementar medidas específicas para intentar reducir la tasa de ausentismo, como por ejemplo, enviar recordatorios a los pacientes, redistribuir los horarios según los servicios, etc. 

## Referencias:

D. H. Giunta, Ausentismo de pacientes a consultas programadas en un sistema de salud: estimación de tasas, identificación de factores asociados, causas y predicción. [Tesis de Doctorado en Ciencias de la Salud (2019)](http://trovare.hospitalitaliano.org.ar/greenstone/collect/tesisytr/index/assoc/D942.dir/tesis-giunta-diego.pdf), Instituto Universitario y Hospital Italiano de Buenos Aires.

# Datos:

Todos los datos aquí disponibles fueron obtenidos con los correspondientes permisos de las autoridades de la institucinó de salud, cuyo nombre no mencionaremos. La información correspondiente a personas se encuentra debidamente anonimizada y toda información potencialmente sensible ha sido removida.

Contaremos con un canal de comunicación de la institución, por el cual podremos solicitar información que consideremos relevante, y que no se encuentre en los datasets inicialmente provistos.

## Descripción del dataset de turnos:

**Archivo**: _dataset_turnos_2018-2019.zip_

El dataset forma parte de las bases de datos de la institución médica. Contiene información referida a los turnos correspondientes a consultas y prácticas médicas que se realizan en cada uno de los centros de atención.

### Campos:

* **Centro de atención:** Cada uno de los cuatro centros de atención con que cuenta la institución

* **Servicio:** Servicio utilizado en el turno

* **Recurso:** Profesional o instrumento específico correspondiente al turno

* **Prestación asignada:** Prestación asignada en en el turno

* **Estado del turno:** Estado (presente o pasado) correspondiente al turno. Indica si el turno fue atendido, se encuentra libre, si el paciente se ausentó, si fue cancelado o reprogramado, etc.

* **Nombre del Canal:** Canal de comunicación por donde se realizó la reserva del turno

* **Fecha del turno:** Día correspondiente al turno

* **Hora del turno:** Horario del turno

* **Es sobre turno:** Indica si se trata de un turno regular o de un sobre turno

* **Tipo de turno asignado:** Indica si el turno corresponde a una primera consulta, a la realización de una práctica, a un control, etc.

* **Edad:** Edad del paciente

* **Género:** Género del paciente

* **Cobertura:** Obra social o prepaga, en caso de que la tenga


## Descripción del dataset de condiciones meteorológicas:

Los dataset *dataset_clima_2018.csv* y *dataset_clima_2019.csv* contienen información meteorológica por día para el período correspondiente al análisis, de los años 2018 y 2019 respectivamente. Fueron obtenidos a partir de datos abiertos disponibles en [https://www.ogimet.com/](https://www.ogimet.com/). 

# Librerías necesarias:

* ``pandas`` (>= 1.0.5)
* ``numpy`` (>= 1.19.0)
* ``matplotlib`` (>= 3.2.2)
* ``seaborn`` (>= 0.10.1)
* ``scipy`` (>= 1.4.1)
* [``sidetable``](https://github.com/chris1610/sidetable) (>= 0.5.0)

# Tiempo de ejecución aproximado:
_10 min_

# Notas

En el futuro se incluirá una versión de ejecución online (Colab)
