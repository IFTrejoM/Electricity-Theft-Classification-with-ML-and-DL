El presente proyecto busca clasificar, de forma efectiva, hogares que defraudan a la compañía
eléctrica de los que no, evaluando el desempeño algoritmos de aprendizaje supervisado.

Para efecto, contamos con un conjunto de datos cuyas variables características son el consumo
diario de energía eléctrica de 9957 hogares. La variable objetivo es de carácter binario, e indica
cuáles hogares se detectaron como defraudadores (1) y cuáles no (0).

La selección de las métricas a utilizar dependerá de los objetivos específicos del proyecto y del
equilibrio que se desee encontrar entre Precisión y Recall. Por ejemplo, si el costo de identificar
un hogar que no defrauda a la compañía eléctrica como un hogar que sí defrauda es muy alto,
entonces se debe priorizar Recall sobre Precision. Por otro lado, si el costo de identificar un hogar
que defrauda a la compañía eléctrica como un hogar que no defrauda es muy alto, entonces se debe
priorizar Precision sobre Recall.

A la par, para evaluar la capacidad de generalización de los modelos, revisaremos los valores de
Error Cuadrado Medio (MSE) de cada uno. Calcularemos el MSE de validación cruzada así como
el obtenido en los conjuntos de entrenamiento train_mse y evaluación test_mse. Cosideraremos
los modelos con menor valor de train_mse - test_mse como aquellos con menor sobreajuste, es
decir, mejor capacidad de generalización.
