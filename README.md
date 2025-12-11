PCA (load_wine.csv)
```markdown
# Reducción de Dimensionalidad con PCA – Dataset Wine

Autor: Diego Ivan Prieto Puga
Fecha: 11 Diciembre 2025

## Objetivo
Aplicar **Análisis de Componentes Principales (PCA)** al dataset Wine para reducir sus 13 variables químicas a 2 componentes manteniendo la máxima varianza posible y visualizar la separación de las 3 clases de vino.

## Archivos
- PCA_Wine.ipynb → Notebook completo con gráfica de varianza explicada
- load_wine.csv → Dataset original
- pca_wine_model.pkl → Objeto PCA ajustado (2 componentes)
- scaler_wine.pkl → StandardScaler usado
- requirements.txt

## Resultados
- Componentes seleccionados: 2
- Varianza explicada acumulada: XX.XX%
- Excelente separación visual de las 3 clases de vino en el espacio 2D

## Uso
```python
import joblib
pca = joblib.load('Diego_PCA_wine.pkl')
scaler = joblib.load('scaler_wine.pkl')
vino_2d = pca.transform(scaler.transform(nuevo_vino))
