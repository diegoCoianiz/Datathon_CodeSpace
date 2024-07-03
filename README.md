# Sistema de predicción de ventas para empresa gastronómica

![alt text](image.png)

# Introducción

Este estudio, diseñado en parte en Google Colab y en parte en un entorno CONDA, corresponde al módulo final del bootcamp de Ciencia de Datos & IA de la academia española [CodeSpace](https://codespaceacademy.com/), y tiene como finalidad el desarrollo de un modelo predictivo de regresión temporal para determinar, en un lapso de tiempo X (de 1 mes, para la presentación de este proyecto), las venta futuras de cada uno de los productos que esta compañia, dividida en 3 emprendimientos, tiene.

# Acerca del conjunto de datos

El dataset es un conjunto de datos de 10322 × 8 fechas de venta para 15 **articulos** denominados numéricamente y pertenecientes, cada uno, a uno de 3 emprendimientos (denominados **familias**), en un lapso de tiempo que va desde: 2021-05-18 a 2023-04-20. Los datos para este set están desvalaceados y se encuentran articulos como el N° 3960 con un total de 730 fechas de venta, y en el extremo opuesto el N° 6549 con 426 fechas.

# Descripción del proyecto
El proyecto consta de 2 notebooks:

 * Proyecto_final_Datathon : En el se realizan los esstudios e inspecciones correspondientes. A partir de la fase 3 se comienza a proyectar diferentes modelos y, sobre todo, estrategias de partición del set para alcanzar la mayor performance predictiva. Tras una serie de estudios, ya en la fase 4, se concluye cual es la estrategia optima para particionar y determinar el mejor (los mejores, hablando propiamente) modelo predictivo y se crea un dataframe **best_config** con la info sobre la estrategia de división

 * mlfow_predictions : Este notebook trabaja sobre un entorno de desarrollo CONDA, para ser ejecutado con algun editor de codigo, en mi caso Visual Studio Code. Se habilita un puerto 5000 para generar un laboratorio de operaciones con MLFlow y, utilizando la info en el dataSet **best_config** , se opera con la estrategia final sobre cada uno de los items y se almacenan los resultados en **predicciones_totales**, un csv con información sobre las ultimas predicciones a comparar respecto del dataFrame original, en otras palabras predicciones que van desde enero de 2023 hasta mediados de abril del mismo año (momento en que finaliza el set original) y contunian un mes mas, hasta el 2023-05-28 aprox, con datos totalmente predichos para cada item.

# Contribuye!
¡Las contribuciones son bienvenidas! Si desea contribuir al proyecto, no dude en ponerse en contacto y pullerar sus actualizaciones!

# Licencia
Este proyecto está bajo la licencia MIT . Siéntase libre de usarlo, modificarlo y distribuirlo de acuerdo con los términos de la licencia.