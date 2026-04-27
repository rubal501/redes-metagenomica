# Análisis Comparativo de Redes Metabólicas: Sano vs. Enfermo

El código original se trabajo en [google colab](https://colab.research.google.com/drive/1iwYtVKtxozITQX-2XOf9PL0DF0oI-vnB?usp=sharing)

## Requisitos y Dependencias

Para ejecutar el notebook `analisis.ipynb`, es necesario contar con un entorno de **Python 3.x**.

### Bibliotecas de Python

Puedes instalar todas las dependencias necesarias con el siguiente comando:

```bash
pip install pandas numpy networkx matplotlib scipy statsmodels
```

### Detalle de las dependencias:
*   **Pandas**: Carga y manipulación de matrices de adyacencia (formatos CSV).
*   **NumPy**: Operaciones matriciales y manejo de datos numéricos.
*   **NetworkX**: Construcción de grafos, cálculo de métricas (grado, densidad, clustering, LCC) y análisis diferencial.
*   **Matplotlib**: Generación de visualizaciones técnicas y diagramas de red.
*   **SciPy**: Ejecución de pruebas estadísticas no paramétricas (`Kolmogorov-Smirnov`, `Mann-Whitney U`, `Wilcoxon`).
*   **Statsmodels**: Cálculo de funciones de distribución empírica (ECDF).
