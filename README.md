# Análisis Comparativo de Redes Metabólicas: Sano vs. Enfermo

Este repositorio contiene un análisis computacional de las propiedades
topológicas de redes de rutas metabólicas reconstruidas a partir de datos
metagenómicos. El estudio compara la estructura de estas redes en individuos
sanos frente a individuos enfermos, utilizando herramientas de teoría de grafos
y estadística.

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
