

​
# <h1 align="center">**`Proyecto Individual 2`**


​
¡Bienvenidos a mi segundo proyecto! Durante este proyecto estaré poniendo a prueba mis habilidades en el campo de la predicción de la mano de Machine Learning. 

<p align="center">
<img src="https://revistabyte.es/wp-content/uploads/2020/01/el-machine-learning-como-metodo-para-predecir-el-impago.jpg"   
>
</p>

​
## **Información relevante**
​
La hospitalización, o estancia hospitalaria, cuando es prolongada constituye una preocupación a nivel mundial debido a sus efectos negativos en el sistema de salud, aumentando los costos, generando deficiencia en la accesibilidad de prestación de servicios de salud, saturación de unidades de hospitalización y urgencias, por consiguiente, mayores efectos adversos como lo son las enfermedades intrahospitalarias.

El estudio de los procesos de atención en salud, así como el conocimiento de las características y perfiles de los usuarios con el objetivo de predecir la ocupación hospitalaria, es uno de los aspectos al que las autoridades de salud han prestado gran interés, pues permite no sólo garantizar los recursos necesarios para la atención del paciente, sino realizar ajustes respecto a la oferta y demanda de los servicios de salud y los implementos asociados.
​
<p align="center">
<img src="https://thumbs.dreamstime.com/b/edificio-del-hospital-59693686.jpg"   
>
</p>


## **Descripción del problema**

Un importante Centro de Salud me ha contratado con el fin de poder predecir si un paciente tendrá una estancia hospitalaria prolongada o no, utilizando la información contenida en el dataset asociado, la cual recaba una muestra histórica de sus pacientes, para poder administrar la demanda de camas en el hospital según la condición de los pacientes recientemente ingresados. 

Para esto, se define que un paciente posee estancia hospitalaria prolongada si ha estado hospitalizado más de 8 días. Por lo que deberé generar dicha variable categórica y luego categorizar los pacientes según las variables que considere necesarias. 
​
<p align="center">
<img src="https://blogs.iadb.org/salud/wp-content/uploads/sites/15/2021/06/infraestructura-en-salud.jpg"   
>
</p>

## **Métrica a utilizar**
​
Como método de evaluación del desempeño del modelo, se utilizará la métrica de Exhaustividad (Recall) para las estadías hospitalarias largas, a partir de la matriz de confusión (Confusion Matrix). 


$$ Recall=\frac{TP}{TP+FN}$$


Donde $TP$ son los verdaderos positivos y $FN$ los falsos negativos.

Como métrica adicional para verificar el desempeño del modelo, también se utilizará la métrica de precisión (Accuracy) para las estadías hospitalarias largas.

$$ Accuracy=\frac{TP+TN}{P+N}$$

siendo $TP$ los verdaderos positivos, $TN$ verdaderos negativos y $P+N$ población total.


<p align="center">
<img src="https://miro.medium.com/max/1400/1*c_fiB-YgbnMl6nntYGBMHQ.jpeg"   
>
</p>

## **Pasos a realizar**
- En primera instancia se realiza un EDA para entende que tipos de datos tenemos y como estan distribuidos.
- Luego se procede a hacer los cambios pertinentes para cada conjunto de datos.
- Evaluamos la correlacion de los mismos.
- Establecemos cual va a se el conjunto de datos a utilizar desechando aquello que no guarde correlacion.
- Instanciamos un modelo de predicción, se entrena y se testea.
- Procedemos a generar la prediciones correspondientes y necesarias.
- Guardamos nuestra predicción para el conjunto de datos que se desea hacer la predicción.  



## **Archivos disponibles**
​
Se trabaja con los siguientes archivos para realizar el proyecto:
 - 'hospitalizaciones_train.csv': Contiene 410000 registros y 15 dimensiones, el cual incluye la información numérica de la cantidad de días de estancia hospitalaria.
 - 'hospitalizaciones_test.csv': Contiene 90000 registros y 14 dimensiones, el cual no incluye la información de la cantidad de días de estancia hospitalaria.
​
## **Descripción de las dimensiones**
- Available Extra Rooms in Hospital: Habitaciones adicionales disponibles en el hospital. Una habitación no es igual a un paciente, pueden ser individuales o compartidas.
- Department: Área de atención a la que ingresa el paciente. 
- Ward_Facility_Code: Código de la habitación del paciente.
- doctor_name: Nombre de el/la doctor/a a cargo del paciente.
- staff_available: Cantidad de personal disponible al momento del ingreso del paciente.
- patientid: Identificador del paciente.
- Age: Edad del paciente.
- gender: Género del paciente.
- Type of Admission: Tipo de ingreso registrado según la situación de ingreso del paciente.
- Severity of Illness: Gravedad de la enfermedad/condición/estado del paciente al momento del ingreso.
- health_conditions: Condiciones de salud del paciente. 
- Visitors with Patient: Cantidad de visitantes registrados para el paciente.
- Insurance: Indica si la persona posee o no seguro de salud. 
- Admission_Deposit: Pago realizado a nombre del paciente, con el fin de cubrir los costos iniciales de internación. 
- Stay (in days): Días registrados de estancia hospitalaria. 
​
## **Palabras finales**

Despues de revisar un par de modelos me decidí por uno, en este caso particular **Arbol de Decicion**. Aún asi, podrán ver el desarrollo de otro modelo (k-vecinos) y la evualuacion de modelos con pipeline, pero los resultados de los mismos no terminó de dar los valores esperados. 
Dejo ambos modelos y la evaluacion de modelos  para su consideracion.


P/D: Tengan en cuanta la correcta refrigeracion de su equipo de trabajo, esto demanda tiempo y capacidad de procesamiento, aumentando considerablemente la temperatura del mismo. 

Saludos.



<p align="center">
<img src="https://media.tenor.com/hEwfEcj2R60AAAAM/laptop-smoking.gif"   
>
</p>