# Segmentación de Clientes para Estrategias de Marketing Personalizadas

Este proyecto aplica técnicas de Ciencia de Datos para segmentar clientes de una empresa ficticia de retail, con el objetivo de identificar patrones de comportamiento que permitan diseñar estrategias de marketing más efectivas y personalizadas.

---

## Objetivo

Utilizar **clustering con K-Means** para agrupar clientes con características similares, basándonos en:
- Ingreso mensual (`Income`)
- Gasto total (`MntTotal`)
- Recencia de compra (`Recency`)
- Frecuencia y canal de compra (`NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases`)

---

## Dataset

- **Nombre:** `ifood_df.csv`
- **Fuente:** Kaggle - Marketing Analytics Dataset
- **Variables clave:** ingresos, gasto, frecuencia de compra y canales utilizados.

---

## Metodología

1. **Revisión inicial del dataset**
   - No se encontraron valores nulos.
   - Se seleccionaron 6 variables numéricas relevantes.

2. **Preprocesamiento**
   - Escalado estandarizado con `StandardScaler`.

3. **Modelo de Clustering**
   - Algoritmo utilizado: `K-Means`
   - Número de clústers: 4 (selección empírica)
   - Visualización de resultados con boxplots, heatmaps y reducción de dimensiones (`PCA`).

4. **Asignación de etiquetas**
   - Se asignaron descripciones interpretables a cada clúster para facilitar su análisis y uso en estrategias de marketing.

---

## Principales Hallazgos

| Cluster | Descripción                            | Características Destacadas                             |
|--------|-----------------------------------------|--------------------------------------------------------|
| 0      | Alto ingreso, alto gasto                | Clientes rentables, frecuentes y con alto poder adquisitivo |
| 1      | Bajo ingreso, bajo gasto                | Segmento de bajo valor, ideal para campañas de retención |
| 2      | Ingreso medio, gasto medio              | Clientes estables, potencial para fidelización         |
| 3      | Clientes recientes, bajo gasto          | Compradores nuevos con posibilidad de crecer su ticket promedio |

- El **Cluster 0** es el más rentable y debe ser enfocado con beneficios premium.
- El **Cluster 3** agrupa a clientes recientes y podría activarse con campañas de bienvenida o upselling.
- El análisis visual con PCA y heatmaps confirmó la separación de los segmentos.

---

## Conclusiones

- La segmentación permite adaptar mensajes y promociones a cada tipo de cliente.
- Usar clustering como parte de una estrategia de marketing basada en datos ayuda a tomar decisiones más inteligentes.
- Este enfoque puede escalarse e integrarse a sistemas CRM y automatización de campañas.

---

## Herramientas y Librerías

- Python (Google Colab)
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`: StandardScaler, KMeans, PCA

---

## 📁 Archivos del proyecto

- `Segmentacion_Clientes_Marketing.ipynb`: Notebook con el código completo
- `ifood_df.csv`: Dataset utilizado
- `README.md`: Este archivo

---

## 📬 Contacto

Proyecto desarrollado por José Alberto Hurtado Echeverría  
[LinkedIn](https://www.linkedin.com/in/jos%C3%A9-alberto-hurtado-echeverr%C3%ADa-77910a319/)  
[GitHub](https://github.com/jose-alberto-hurtado)

---
▶️ [Abrir notebook en Google Colab](https://colab.research.google.com/github/jose-alberto-hurtado/segmentacion-clientes-marketing/blob/main/Segmentacion_Clientes_Marketing.ipynb)

