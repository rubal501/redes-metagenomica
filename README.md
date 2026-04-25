# Análisis Comparativo de Redes Metabólicas: Sano vs. Enfermo

Este repositorio contiene un análisis computacional de las propiedades topológicas de redes de rutas metabólicas reconstruidas a partir de datos metagenómicos. El estudio compara la estructura de estas rutas en individuos sanos frente a individuos enfermos, utilizando herramientas de teoría de grafos y estadística.

El análisis se centra en un conjunto compartido de **619 nodos** (rutas metabólicas), evaluando cómo la conectividad y la organización global cambian entre las dos condiciones.

## Estructura del Proyecto

*   `analisis.ipynb`: Notebook de Jupyter con el flujo completo de análisis (procesamiento, métricas, estadística y visualización).
*   `H_adjcent_path_completeNET.csv`: Matriz de adyacencia de la red de individuos sanos.
*   `DD_adjcent_path_completeNET.csv`: Matriz de adyacencia de la red de individuos enfermos.
*   `network_topology_summary.csv`: Resumen de las métricas topológicas globales calculadas.
*   `reporte-latex/`: Directorio con el manuscrito académico y las figuras.
    *   `main.tex`: Archivo principal del reporte en LaTeX.
    *   `figures/`: Gráficos generados (distribución de grados, prueba de permutación, etc.).
*   `nmeth.4468.pdf`: Documento de referencia sobre la metodología empleada.

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

## Metodología y Resultados

1.  **Construcción de Grafos**: Binarización de matrices y alineación de 619 nodos.
2.  **Métricas Globales**: Cálculo de densidad, grado promedio y coeficiente de agrupamiento. Se observó una mayor densidad en la red enferma (1,215 aristas vs 876).
3.  **Análisis Diferencial**: Clasificación de aristas en ganadas, perdidas y conservadas.
4.  **Validación Estadística**: 
    *   Pruebas de hipótesis clásicas para comparar distribuciones de grado.
    *   **Prueba de Permutación**: Realización de 10,000 iteraciones para evaluar la significancia de la diferencia en el grado promedio ($p = 0.0067$).
5.  **Reporte**: El archivo `reporte-latex/main.tex` documenta detalladamente los hallazgos, incluyendo la interpretación biológica de la reorganización topológica observada.
