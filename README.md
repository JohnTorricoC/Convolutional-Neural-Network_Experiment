# Convolutional-Neural-Network_Experiment

![Accuracy_Stadistics](https://user-images.githubusercontent.com/34653032/120119089-c969a880-c163-11eb-8899-d107196c4235.png)


# Descripcion de los experimentos

- Exp1 - Este experimento se logro estableciendo un epoch de 1 y se logro una precision de 90.75%
- Exp2 - Este experimento se logro estableciendo un epoch de 3 y se logro una precision de 96.13%
- Exp3 - Este experimento se logro estableciendo un epoch de 5 y se logro una precision de 97.26%

Se pudo ver que a mayor numero de epoch se logra una mejor precision esto es debido a que a mayor cantidad de epoch hay una mayor cantidad de ajustes de los pesos y biases

- Exp4 - Este experimento se logro estableciendo 2 capas convuncionales y estableciendo un epoch de 1, el cual los resultados lanzaron una precision de 92.01%
- Exp5 - Este experimento se logro estableciendo 2 capas convuncionales y estableciendo un epoch de 3, el cual los resultados lanzaron una precision de 98.31%
- Exp6 - Este experimento se logro estableciendo 2 capas convuncionales y estableciendo un epoch de 5, el cual los resultados lanzaron una precision de 98.12%

Se pudo ver que a mayor cantidad de capas que se le agrega a nuestra red convulcional esta tiene mayor precision, esto es debido a que a mayor numero de capas existen una mayor cantidad de filtros los cuales extraen mejor las caracteristicas del set de datos.

- Exp7 - Este experimento se logro estableciendo un dropout de 0.1 y tambien estableciendo un epoch de 3, el cual los resultados fueron de 91.92%
- Exp8 - Este experimento se logro estableciendo un dropout de 0.5 y tambien estableciendo un epoch de 3, el cual los resultados fueron de 90.86%
- Exp9 - Este experimento se logro estableciendo un dropout de 0.99 y tambien estableciendo un epoch de 3, el cual los resultados fueron de 60.88%

Se pudo ver que cuando el parametro dropout sea mas grande la precision baja, primaremente decir que el parametro dropout nos ayuda a evitar el overfitting, pero a su vez este hace que el modelo sea menos preciso una hipotesis es que el dropout incrementa el margen de error que pueda tener una red neuronal provocando un menor rendimiento en el accuracy

- Exp10 - Este experimento se logro estableciendo una capa fully connected entre el output layer y el convuntional layer, el cual tuvo una precision de 98.06%
- Exp11 - Este experimento se logro estableciendo un max pool size de 2x2 y un stride de 2 el cual lanzo una precision de 95.75%
- Exp12 - Este experimento se logro estableciendo un max pool size de 3x3 y un stride de 3 el cual lanzo una precision de 82.43%
- Exp13 - Este experimento se logro estableciendo un average pool size de 2x2 y un stride de 3 el cual lanzo una precision 94.07%
- Exp14 - Este experimento se logro estableciendo un average pool size de 3x3 y un stride de 3 el cual lanzo una precision 74.10%

Se pudo ver que cuando el pool size es mas pequeño se obtiene reducir la imagen convulcionada a una con mejor resolucion, en cambio cuando el pool size es mas grande la imagen convulcionada pierde resolucion lo cual tiene un impacto negativo en la precision, aparte de este experimento se vio que el max pool layer tuvo una mayor precision que el average pool layer, desafortunadamente no se pudo realizar una hipotesis de porque en este set de experimentos el max pool layer tuvo un mejor rendimiento que el average pool layer, la unica sospecha que se puede dar es que los filtros de sobel que se aplican a los datos de pruebas son resaltados de mejor manera en el max pool layer a diferencia del  average pool layer, pero me gustaria recalcar que es una sospecha la cual no la podemos respaldar
