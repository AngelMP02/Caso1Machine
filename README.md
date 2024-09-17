# Caso1Machine
https://github.com/AngelMP02/Caso1Machine

-Limpieza de Datos: Identificacion y tratamiento de valores
faltantes, outliers y datos inconsistentes.

-Codificación de Variables Categóricas: Transformacion de datos categoricos en un formato adecuado para el modelo.
Supongamos que tienes una columna de combustible como esta:

Combustible
Gasolina
Diesel
Gasolina
Eléctrico

LabelEncoder asigna un número único a cada categoría:

Combustible	Codificado
Gasolina	0
Diesel	1
Eléctrico	2

De esta manera, cada categoría ahora está representada por un valor numérico, permitiendo que el modelo trabaje con estas características categóricas.

-Normalización y Escalado: Ajuste de los valores numericos para facilitar la convergencia del modelo.

Supongamos que tienes una columna con valores de edad del cliente:

Edad Cliente
18
53
21
48
Primero calculamos la media y la desviación estándar de esta columna. Luego, transformamos cada valor usando la fórmula:
valor escalado = (valor original - media) / desviación estándar  

Resultado del Escalado:
Al escalar las variables, los valores numéricos quedan transformados de manera que su media es 0 y su desviación estándar es 1, como se muestra en las primeras filas del dataset escalado:

EDAD_COCHE	COSTE_VENTA	km_anno	Edad Cliente	Tiempo
-1.07	0.40	-1.21	-2.59	-0.58
-0.94	-0.73	-0.44	0.50	-0.58
-0.92	-0.73	-1.21	-2.33	0.43

Este proceso asegura que las variables están en la misma escala y que el modelo no favorecerá a ninguna variable solo por su magnitud.
