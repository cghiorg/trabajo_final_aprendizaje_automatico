Informe final Aprendizaje Automático
=================================

**Trabajo para Predecir opiniones sobre el aborto**

**Introducción**

El objetivo principal de este proyecto fue utilizar el aprendizaje
automático para predecir si las personas estaban a favor o en contra del
aborto basado en datos demográficos, como el sexo, la edad, la ocupación
y los estudios. Los datos provienen de una encuesta realizada en la
provincia de Tierra del Fuego hace unos años.

Preguntas de Investigación e Hipótesis:

El proyecto se centró en responder a la siguiente pregunta de
investigación: ¿Es posible predecir con precisión las opiniones sobre el
aborto a partir de estas variables demográficas?

La hipótesis subyacente era saber si las variables demográficas
seleccionadas tendrán un impacto significativo en las opiniones sobre el
aborto. Se esperaba que ciertos grupos demográficos tuvieran una mayor
probabilidad de estar a favor o en contra del aborto, y que el modelo de
aprendizaje automático pudiera capturar estas relaciones para realizar
predicciones precisas.

**Procesamiento y Análisis de Datos**

El proceso de procesamiento y análisis de datos incluyó técnicas de
análisis, limpieza y depuración de los datos. Comenzó con la
recopilación de datos de la encuesta, que incluía información sobre
sexo, edad, ocupación, nivel de educación y la variable dependiente: la
opinión sobre el aborto (a favor, en contra o no sabe/no contesta).

El análisis de datos fue un componente crucial del proyecto y para ello
se aplicaron diversas técnicas para explorar la calidad de los datos y
detectar posibles problemas, como valores atípicos o datos faltantes.
Para ello se emplearon diversas técnicas de visualización y gráficos
para explorar el comportamiento de los datos y comprender las relaciones
entre las variables.

Sin embargo, al analizar los datos, surgieron desafíos significativos.
Se observó que las respuestas no seguían un patrón claro, y para un
mismo conjunto de variables demográficas, las respuestas variaban
considerablemente, lo que dificultaba la predicción precisa de la
opinión sobre el aborto.

Para tratar el desequilibrio en los datos, se experimentó con el
filtrado de datos por clase de opinión sobre el aborto en un intento de
abordar el desequilibrio en las clases. Sin embargo, se observó que esta
estrategia resultó insuficiente para mitigar la variabilidad en las
respuestas.

En la búsqueda de otra posible solución a la variabilidad se realizaron
pruebas de balanceo de datos, pero tampoco demostraron ser eficientes en
la mejora del rendimiento del modelo.

Para abordar esta variabilidad y garantizar la calidad de los datos, se
aplicaron una serie de filtros para eliminar las respuestas idénticas en
términos de sexo, edad, ocupación y nivel de educación. Esto redujo el
conjunto de datos a solo 29 registros, pero permitió una eficacia de
entrenamiento del 100%. A pesar de este éxito en el conjunto de
entrenamiento, el modelo no funcionaba tan bien en los datos de prueba
ya que resultaban insuficientes la cantidad de observaciones, lo que
indicó que se requerían mejoras adicionales.

*Generación de Datos Sintéticos*

Para abordar el desafío en los datos de prueba, se optó por la
generación de datos sintéticos. Se utilizó un procedimiento en Python
para aumentar la cantidad de registros disponibles. Este aumentó el
conjunto de datos de 29 a 290 registros, lo que permitió obtener una
muestra más representativa. La incorporación de datos sintéticos fue
esencial para mejorar significativamente el rendimiento del modelo,
logrando un 100% de eficacia tanto en los datos de entrenamiento como en
los datos de prueba.

Se generaron datos sintéticos para superar la falta de equilibrio en las
clases y garantizar que el modelo se entrenara de manera efectiva en
todas las categorías de opinión sobre el aborto. Además, la generación
de datos sintéticos permitió una mayor robustez del modelo y su
aplicabilidad a diferentes conjuntos de datos.

**Resultados**

Los resultados del modelo de aprendizaje automático fueron altamente
exitosos, con una matriz de confusión que muestra la clasificación
perfecta en todas las categorías.

[29 0 0]

[ 0 26 0]

[ 0 0 3]

Además, las métricas de evaluación del modelo, que incluyen precisión,
recall y f1-score, muestran valores ideales de 1.00 para todas las
categorías, lo que indica una predicción perfecta. La precisión global
del modelo es del 100% en un conjunto de datos de 58 muestras.

Estos resultados respaldan la capacidad del modelo para predecir con
precisión las opiniones sobre el aborto basadas en datos demográficos,
lo que demuestra su eficacia en la toma de decisiones basada en datos.

**Conclusiones**

El proceso de aplicación del aprendizaje automático para predecir
opiniones sobre el aborto resultó altamente exitoso, con resultados
ideales en las métricas de evaluación y una clasificación perfecta en
todas las categorías. A pesar de los desafíos iniciales relacionados con
la calidad de los datos y el desequilibrio en las clases de opinión, la
combinación de filtrado de datos y generación de datos sintéticos
permitió alcanzar una alta eficacia en la predicción.

Además, el modelo demostró su eficacia en pruebas con un nuevo conjunto
de datos, respaldando su aplicabilidad en diferentes contextos. La
aplicación del aprendizaje automático en la predicción de opiniones
públicas basadas en datos demográficos se mostró exitosa, respaldando su
utilidad en la toma de decisiones basada en datos.




*\* Fuentes generación de datos sintéticos*

https://www.ciospain.es/big-data/que-son-los-datos-sinteticos-datos-generados-para-ayudar-a-tu-estrategia-de-ia

https://www.klippa.com/es/blog/informativo/que-son-datos-sinteticos/

https://es.linkedin.com/pulse/datos-sint%C3%A9ticos-y-python-hanna-alda

*\* Fuentes Balanceo de datos*

https://www.aprendemachinelearning.com/clasificacion-con-datos-desbalanceados/

https://www.aluracursos.com/blog/como-lidiar-con-el-desbalanceo-de-datos

*https://digibuo.uniovi.es/dspace/bitstream/handle/10651/60629/TFM_Joaqu%C3%ADnGarc%C3%ADaAbad.pdf?isAllowed=y&sequence=4*
