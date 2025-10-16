# 📊 TALLER SEGUNDO CORTE: ANÁLISIS DE DATOS CON PYTHON

***

## 🏛️ Información Académica

* **Universidad:** Universidad del Pacífico.
* **Carrera o Programa:** Ingeniería en sistemas.
* **Asignatura:** Inteligencia Artificial (IA)
* **Integrantes del Grupo:**
   
    * ANDRES STEVEN RIVAS SALAS
    * KEVIN JOSEPH VALBUENA PÉREZ
    * RUBEN DARIO BARAHONA

***

## 🎯 Objetivo del Trabajo

El objetivo principal de este taller es aplicar los fundamentos de la programación en **Python** para la **manipulación y análisis de datos**, utilizando las librerías especializadas **NumPy** y **Pandas**. Específicamente, se busca:

1.  Demostrar el manejo eficiente de **arreglos numéricos** y el cálculo de medidas estadísticas fundamentales (media, moda, varianza).
2.  Realizar el **análisis exploratorio de datos** de un conjunto de estudiantes, incluyendo filtrado de información y agrupamiento.
3.  Generar **visualizaciones** (gráficos de barras, dispersión e histogramas) para interpretar la distribución y relación de las variables.

***

## 💡 Descripción del Proyecto o Taller

Este proyecto se materializa a través de un **Colab Notebook** (archivo `.ipynb`) que aborda ejercicios prácticos divididos en dos grandes bloques: la manipulación de datos con NumPy y el análisis del dataset real de estudiantes (`Dataset_Estudiantes.xlsx`) utilizando Pandas y Matplotlib.

### 🛠️ Tecnologías Utilizadas

| Librería | Versión (opcional) | Función Principal |
| :--- | :--- | :--- |
| **Python** | 3.x | Lenguaje de programación. |
| **NumPy** (`np`) | | Operaciones con vectores y matrices. |
| **Pandas** (`pd`) | | Estructuras de datos (DataFrame) y análisis. |
| **Matplotlib** (`plt`) | | Visualización de datos. |
| **SciPy** (`stats`) | | Funcionalidades científicas y estadísticas. |

***

## 💻 Desarrollo y Explicación

### 🧪 Metodología Aplicada

Se utilizó una metodología de **Análisis Exploratorio de Datos (EDA)** estructurada, que incluyó:

1.  **Preparación de Entorno:** Importación de librerías y montaje de Google Drive para la carga de datos.
2.  **Análisis Básico con NumPy:** Resolución de ejercicios matemáticos fundamentales para validar la comprensión de la librería.
3.  **Carga y Limpieza de Datos:** Lectura del archivo `.xlsx` en un DataFrame.
4.  **Estadísticas Descriptivas:** Cálculo de medidas de tendencia central y dispersión sobre las notas.
5.  **Transformación y Agrupación:** Filtrado de datos y cálculo de promedios por categorías (`Género`).
6.  **Visualización:** Creación de gráficos para una interpretación rápida y visual de los resultados.

### ✅ Pasos Realizados para Resolver el Ejercicio

#### 1. Ejercicios Fundamentales con NumPy
* Se creó un arreglo con números del 1 al 1000 y se calculó su suma total: **500500**.
* Se calcularon la **media** (6.25), **mediana** (7.0), **moda** (8) y **varianza/desviación estándar** (6.4375 / 2.5372) para un arreglo de prueba `[2, 4, 4, 6, 8, 8, 8, 10]`.

#### 2. Análisis del Dataset de Estudiantes
* **Carga de Datos:** Se cargó el archivo `Dataset_Estudiantes.xlsx` en el DataFrame `df_datasetestu`.
    ```python
    df_datasetestu = http://pd.read_excel('/content/drive/MyDrive/kaggle/Dataset_Estudiantes.xlsx')
    ```
* **Estadísticas de Notas:**
    * Media: **3.901**
    * Mínima: **2.6**
    * Máxima: **5.0**
    * Desviación Estándar: **0.7151**

* **Filtrado:** Se identificaron a los estudiantes con una nota mayor o igual a 4.0.
    ```python
    filtro = df[df['Notas'] &gt;= 4.0]
    ```
* **Análisis por Género:** Se calculó el promedio de notas por categoría:
    * Femenino: **3.978**
    * Masculino: **3.820**

#### 3. Visualizaciones
Se generaron las siguientes representaciones gráficas:
* Gráfico de Barras de `Notas`.
* Gráfico de Dispersión entre `Edad` y `Nota`.
* Histograma de la distribución de `Notas`.

### 🔎 Interpretación y Análisis de Resultados

* **Medidas de Dispersión de Notas:** Con un rango de **2.40** y una desviación estándar de **0.7115**, se observa una dispersión moderada en las notas, lo que indica que la mayoría de las calificaciones se agrupan relativamente cerca de la media (3.901).
* **Rendimiento por Género:** Las estudiantes (Femenino) obtuvieron un promedio de notas ligeramente superior (3.978) en comparación con los estudiantes (Masculino) (3.820).
* **Distribución de Notas:** El histograma permite visualizar la **frecuencia** con la que se repiten ciertos rangos de notas, mientras que el gráfico de dispersión ayuda a determinar si existe una correlación visible entre la edad del estudiante y su rendimiento académico.

***

## ✍️ Conclusión

El taller permitió aplicar de manera exitosa las herramientas de la ciencia de datos en Python, demostrando la capacidad de **NumPy** para cálculos intensivos y la robustez de **Pandas** para el análisis de datos. Los resultados obtenidos proporcionan una visión estadística clara del rendimiento académico del grupo de estudiantes, cumpliendo con el objetivo de manipulación y visualización de datos.
