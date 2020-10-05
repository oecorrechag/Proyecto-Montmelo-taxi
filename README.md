# Proyecto Montmelo

# <center> Distribución de las ganancias
Actividad Clase Estadistica Bayesiana
  
**Universidad Nacional de Colombia**

**Diseño de experimento:**

# Objetivo

# Resultados y conclusiones

En la siguiente figura se evidencia la elicitación realizada (panel de expertos).

Figura 1: Grafico ganancias taxistas.

![alt text](https://github.com/oecorrechag/Proyecto-taxi/blob/main/Grafico_1.png)

En la siguiente figura se evidencia la media de la elicitación realizada (panel de expertos).

Figura 2: Grafico ganancias medias.

![alt text](https://github.com/oecorrechag/Proyecto-taxi/blob/main/Grafico_2.png)

Funcion: *fitdistr*
Libreria: *MASS*
Lenguaje: R
Con ayuda de la funcion *fitdistr* se calculan los valores optimos de la Alpha y Beta.

| Muestra | Alfa |  Beta |
| :---: | :----: | :---: |
|   1   | 113.59 | 4.343 |
|   2   | 635.45 | 16.26 |
|   3   | 130.91 | 5.523 |
|   4   | 75.40  | 4.150 |
|   5   | 299.24 | 11.82 |
|   6   | 352.62 | 11.38 |

Asumiendo que los grupos son similares la distribuci?n aprirori se calcula por medio de:

$$  \xi (\theta) = \frac{1}{6} \sum_{i=1}^{6} \frac{\beta_{i} ^ {\alpha_{i}} } {\Gamma (\alpha_{i})} \theta ^ {\alpha_{i} - 1}  exp (-\beta_{i} \theta) $$

Si utilizamos la distribución calculada a partir de la media geometrica de las apriori se obtiene:

$$ \xi(\theta) \alpha \theta ^ {\sum_{i=1}^{6} \frac{\alpha_{i}}{6-1}} exp (-\theta \sum_{i=1}^{6} \frac{\beta_{i}}{6} )$$

Calculando:

$$ \xi(\theta) \alpha \theta ^ {194.3575} exp (- 6.203293\theta)$$

De esta forma se obtienen las distribuciones apriori de los datos obtenidos de los taxistas.

Figura 3: Grafico distribución ganancias taxistas.

![alt text](https://github.com/oecorrechag/Proyecto-taxi/blob/main/Grafico_3.png)

### Bibliografia

1. Correa, J., (2014). *Introducción a la Estadística Bayesiana: Notas de Clase.* Medellín. Colombia.
