# 📱 ConnectaTel: Análisis de Patrones de Uso y Segmentación de Clientes

## 📌 Descripción del proyecto

Este proyecto tiene como objetivo analizar el comportamiento de uso de los clientes de ConnectaTel, una empresa de telecomunicaciones. A partir de información demográfica y registros de uso, se identificaron patrones de consumo, segmentos de clientes y oportunidades de mejora para la oferta comercial de la compañía.

---

## 🎯 Objetivos del análisis

- Identificar problemas de calidad en los datos y aplicar procesos de limpieza.
- Detectar valores faltantes, sentinels y fechas fuera de rango.
- Analizar patrones de uso de llamadas y mensajes.
- Identificar valores atípicos relevantes para el negocio.
- Segmentar a los clientes según su nivel de uso y grupo de edad.
- Explorar la relación entre edad y comportamiento de consumo.
- Generar insights accionables para apoyar la toma de decisiones comerciales.

---

## 📂 Datasets utilizados

### `users_latam.csv`
Información demográfica y contractual de los clientes.

Variables relevantes:
- `user_id`
- `age`
- `city`
- `reg_date`
- `plan`
- `churn_date`

### `usage.csv`
Detalle del uso realizado por los clientes.

Variables relevantes:
- `user_id`
- `type`
- `duration`
- `length`
- `date`

### `plans.csv`
Información de los planes disponibles.

Variables relevantes:
- nombre del plan
- beneficios incluidos
- costos asociados

---

## 🔎 Etapas del análisis

### 1. Exploración inicial
- Revisión de estructura y tipos de datos.
- Identificación de valores faltantes.
- Identificación de sentinels y valores inválidos.

### 2. Limpieza de datos
- Reemplazo del sentinel `-999` en edad.
- Conversión de fechas al formato adecuado.
- Corrección de fechas fuera del rango esperado.
- Conservación de nulos con significado de negocio.
- Verificación del patrón de faltantes estructurales.

### 3. Análisis exploratorio (EDA)
- Estadísticas descriptivas.
- Distribución de variables numéricas.
- Distribución de variables categóricas.
- Comparación por tipo de plan.
- Identificación y evaluación de outliers.

### 4. Ingeniería de variables
- Segmentación por nivel de uso:
  - Bajo uso
  - Uso medio
  - Alto uso

- Segmentación por edad:
  - Joven
  - Adulto
  - Adulto Mayor

### 5. Insights de negocio
- Identificación de patrones de consumo.
- Evaluación del comportamiento según edad y plan.
- Detección de oportunidades de segmentación.
- Elaboración de recomendaciones para ConnectaTel.


---

## 🛠️ Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## ▶️ Cómo ejecutar el proyecto

### Opción 1: Jupyter Notebook

1. Clona este repositorio:

```bash
git clone https://github.com/camilalealed/connectatel-customer-usage-analysis.git
```

2. Abre el archivo `.ipynb` en Jupyter Notebook o VS Code.

3. Ejecuta las celdas en orden.

---

## 📁 Estructura del repositorio

```
.
├── README.md
├── ConnectaTel_Analysis.ipynb
└── datasets/
    ├── users_latam.csv
    ├── usage.csv
    └── plans.csv
```

