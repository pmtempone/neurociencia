# 24/07 -  clase 01

## Demostrar que es consciente:

+ Hablar y conversar
+ Sin hablar
+ Sin usar músculos del cuello para abajo
+ Sin usar ningún músculo del cuerpo **problema**

Detectar consciencia, bypass.

## Neurona:

+ celula muy grande
+ comunica información en el sistema nervioso
+ Se propaga algo electrico
+ comunicacion entre neuronas es quimica

## Potencial de accion

+ Se pueden diferenciar las capas por iones (positivos o negativos)
+ interior de la celula tiene mas carga negativa que el exterior

EPSP: neurotransmisor excitatorio

IPSP: Neurotransmitor inhibitorio

Medición de los pulsos:

+ Spikes (series de tiempo) - señales binarias

Hans Berger: Frecuencias continuas, electroencefalografia (fourier)

### Dificil inferir interraccion entre areas del cerebro

Ver donde se consume energia, por ahi hubo actividad electrica.

## Suministro de energía

+ energia más alta cuando están unidas las moleculas de atp
+ diferencia entre hemoglobina oxigenada o no


## Hipotesis: flujo sanguineo mido actividad cerebral

## Pesar pensamiento: actividad congnitiva cambia el flujo sanguineo (resonador nuclear en la actualidad):

+ protones son pequeños imanes que se alimentan de campo magnetico.
+ Frecuencia de presion

## Introducir un gradiente:

Ahora la frecuencia de resonancia depende de la coordenada z y es posible excitar solo los protones que estén en la rebanada.


**Se miden correlaciones entre serie temporal del cerebro**

Preprocesado:

+ correccion de movimiento: Rigid body/ Alfine transformations / non - linear transformations
+ filtrado temporal: Filtrado temporal (baja frecuencias/altas frecuencias por el aliasing y frecuencias lentas)
+ segmentacion
+ suavizado espacial
+ normalizacion: se distorsionan distintos cerebros para que ocupen el mismo espacio en la representacion

# 25/07 -  clase 02: conectividad funcional

## Correlacion entre zonas del cerebro:

Se correlaciona con la correlacion entre dos señales Rx,y = (x-media_x)*(y-media_y)/(ssd(x)*sd(y))

Se busca correlacion entre voxel semilla y otro voxel.

Hay redes anticorrelacionadas como resultado de una regresión global del estado de todo el cerebro.

## Baja frecuencia respiratoria

Se analiza la señal IMRI para ver las bajas frecuencias.

## Conectividad estructural del cerebro

Correlacion entre funciones y estructuras (scatter plot r2 0.61)

+ Surgen "redes de estado de reproso"

+ branching ratio < 1 inactivo
+ branching ratio > 1 activo

# 26/07 -  clase 03

## Problema a resolver: 

+ Detección de estados de sueño
+ Elige los puntos de corte en base a simetria entre las tasas de error.

# 27/07 - clase 04

## Selección de features

+ muchos mas sujetos que features

+ agregar features adicionales a los sujetos (pero agregar puede que empeore)

+ Correlacion entre los features

+ PCA

+ Selección recursiva (foward): Evaluar con AUC cada feature a ver cual mejora. ej: [(1,0,0)(0,1,0)(0,0,1)] y [(1,1,0)(0,1,1)]

+ Bacward: al revés.

+ Filtro univariado: t-student para diferencia para cada variable respecto a su clase. X% que tiene el nro más grande.


## Relevancia de features

+ importancia de cada feature

+ Interrelaciones

## Normalización

+ SVM se escalan para que los ejes sean parecidos

+ cross validation muchas veces para validar auc bajos.

## Clasificadores multiclase

+ 4 fases del sueño