# *Hierarchical Risk Parity* Topológico: Eliminando el Ruido con Árboles de Expansión Mínima
**Maestría en Finanzas Cuantitativas | Universidad del Rosario (2026-II)**

### Abstract
La optimización media-varianza suele fallar en las pruebas fuera de la muestra de entrenamiento debido a la poca estabilidad de la matriz de covarianzas histórica y la amplifiación de los errores de estimación en el tiempo. Los acercamientos modernos que utilizan organización jerarquica, como *Hierarchical Risk Parity* (HRP), atacan este problema utilizando teoría de grafos y agrupamiento (*clustering*) con técnicas de aprendizaje de maquinas para distribuir el riesgo sin la necesidad de invertir matrices. Sin embargo, en momentos de crisis sistémica, las matrices de correlación se vuelven altamente colineales, lo cual introduce ruido al proceso de agrupamiento.

El presente projecto introduce un **Filtro Topológico utilizando Árboles de Expansión Minima (MST)** antes de realizar la distribución jerárquica. Al reducir conexiones redundantes entre activos en nuestro grafo inicial, mantenemos únicamente las conexiones más relevantes para determinar una medida de distancia con mucho menos ruido. El proyecto compara tres estrategias de distribución fuera de la muestra de entrenamiento:

1. Pesos Iguales ($1/N$)
2. Hierarchical Risk Parity Estándar (HRP)
3. MST-Filtered HRP (Nuestra contribución topológica)
