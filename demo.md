

    ---
    Titulo: demo
    Autor: Mariángeles Alomar
    Fecha: 15/10/2025
    Fromato: gfm
    Editor: visual
    ---

## 

# Exploración inicial del dataset

El dataset mtcars incluye información sobre distintos modelos de
automóviles: rendimiento (millas por galón), potencia, peso, número de
cilindros, etc.

A continuación mostramos su estructura y las primeras filas:

## 

``` r
# Ver estructura del dataset
str(mtcars)
```

    'data.frame':   32 obs. of  11 variables:
     $ mpg : num  21 21 22.8 21.4 18.7 18.1 14.3 24.4 22.8 19.2 ...
     $ cyl : num  6 6 4 6 8 6 8 4 4 6 ...
     $ disp: num  160 160 108 258 360 ...
     $ hp  : num  110 110 93 110 175 105 245 62 95 123 ...
     $ drat: num  3.9 3.9 3.85 3.08 3.15 2.76 3.21 3.69 3.92 3.92 ...
     $ wt  : num  2.62 2.88 2.32 3.21 3.44 ...
     $ qsec: num  16.5 17 18.6 19.4 17 ...
     $ vs  : num  0 0 1 1 0 1 0 1 1 1 ...
     $ am  : num  1 1 1 0 0 0 0 0 0 0 ...
     $ gear: num  4 4 4 3 3 3 3 4 4 4 ...
     $ carb: num  4 4 1 1 2 1 4 2 2 4 ...

``` r
# Mostrar las primeras filas
head(mtcars)
```

                       mpg cyl disp  hp drat    wt  qsec vs am gear carb
    Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
    Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
    Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
    Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
    Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2
    Valiant           18.1   6  225 105 2.76 3.460 20.22  1  0    3    1

# Figura creada por R

![](demo_files/figure-commonmark/unnamed-chunk-3-1.png)

Como se ve, los autos con mas potencia tienden a tener menor rendimiento
en el consumo

# Figura importada desde URL

![Auto eléctrico representando eficiencia
energética](https://www.motorterra.com/wp-content/uploads/2022/07/2024-Chevrolet-Equinox-EV-004-1-820x394.jpg)

# Tablas de resumen

En esta sección se muestran dos ejemplos de tablas: una escrita
manualmente con sintaxis Markdown y otra generada automáticamente con
código de R.

## 1) Tabla escrita con Markdown

| Variable | Descripción                            | Ejemplo de valor |
|----------|----------------------------------------|------------------|
| mpg      | Millas por galón (rendimiento)         | 21.0             |
| hp       | Caballos de fuerza del motor           | 110              |
| wt       | Peso del vehículo (en miles de libras) | 2.62             |
| cyl      | Número de cilindros                    | 6                |

Esta tabla se escribió directamente usando sintaxis Markdown.

------------------------------------------------------------------------

## 2) Tabla generada con código de R

El siguiente bloque de código muestra las primeras filas del dataset
`mtcars`.  

``` r
# Mostrar las primeras 5 filas del dataset 
head(mtcars, 5)
```

                       mpg cyl disp  hp drat    wt  qsec vs am gear carb
    Mazda RX4         21.0   6  160 110 3.90 2.620 16.46  0  1    4    4
    Mazda RX4 Wag     21.0   6  160 110 3.90 2.875 17.02  0  1    4    4
    Datsun 710        22.8   4  108  93 3.85 2.320 18.61  1  1    4    1
    Hornet 4 Drive    21.4   6  258 110 3.08 3.215 19.44  1  0    3    1
    Hornet Sportabout 18.7   8  360 175 3.15 3.440 17.02  0  0    3    2

# Exploración descriptiva con texto Markdown

En esta sección se muestran ejemplos de *texto con formato*,
**negritas**, *cursivas*, y una lista simple.

El conjunto de datos `mtcars` contiene información sobre distintos
**modelos de automóviles** y variables que describen su rendimiento.  
Podemos destacar algunas variables importantes:

- **mpg** (*miles per gallon*): mide el rendimiento del vehículo.  
- **hp** (*horsepower*): indica la potencia del motor.  
- **wt** (*weight*): representa el peso del automóvil (en miles de
  libras).  
- **cyl** (*cylinders*): número de cilindros del motor.

A continuación, se resumen algunos pasos del análisis que realizamos:

1.  Cargar el dataset `mtcars` en R.  
2.  Explorar su estructura con `str(mtcars)`.  
3.  Visualizar relaciones entre variables con gráficos.  
4.  Documentar los resultados en este informe reproducible con
    **Quarto** y **Markdown**.

------------------------------------------------------------------------

## Ejemplo de escritura matemática

Una relación simple entre potencia (`hp`) y rendimiento (`mpg`) puede
expresarse como:

$$
\text{Eficiencia} = \frac{\text{mpg}}{\text{hp}}
$$

donde una mayor potencia generalmente implica una menor eficiencia.  
  
