# Seguros

Para este estudio se siguió la siguiente estructura:

- Leer Datos y análisis descriptivo
- Ingeniería de variables
- Machine Learning

En la Sección de Machine Learning se pusieron a competir 11 modelos:

- Random Forest
- KNN
- Logistic Regression
- XGB
- Gradient Boosting
- SVC
- Extra Trees
- AdaBoost
- GaussianNB
- Gaussian Process
- Bagging

Se inició con los modelos sin cambiar hiperparámetros ni con selección de varibles (Round 1). Luego se hizo una selección de variables que consistió en ordenar en un Dataframe lo promedios de las punticiones de las mejores variables por modelo, de ahí fueron seleccionadas 13 varibles y se ajustaron nuevamente los modelos pero ahora con la selección de variables (Round 2). Por último en el Round 3 se trabajó con los hiperparámetros de los modelos (se entrenó con la selección de variables), Luego como extra se ajustó un modelo por votaciones donde el voto lo daban los mejores modelos entre los 3 round. 

Se eligieron los dos modelos que clasificaban mejor en test los cueles corresponden a Gradient Boosting y el modelo por votaciones. Para la consideracion del ejercicio "Es 5 veces peor clasificar un cliente como bueno cuando es malo, que malo cuando es bueno". Se le dió una penalización de 5 veces más al error en los malos clasificados como buenos, por medio del costo. La idea es minimizar el costo dada la penalización y extraer el mejor punto de corte. 



