# 📊 Análisis de la Producción de Energía Renovable en América Latina (2015-2022)

Este repositorio contiene un proyecto de **Análisis Exploratorio de Datos (EDA)** y modelado estadístico descriptivo desarrollado para evaluar la evolución, correlación y capacidad per cápita de la transición energética en Sudamérica (Argentina, Brasil, Chile y Colombia). 

El proyecto fue desarrollado bajo la metodología de Ciencia de Datos en el programa **Talento Tech (Nivel Explorador)** del Ministerio de las TIC de Colombia.

---

## 📝 Introducción y Justificación
Ante los desafíos globales del cambio climático y la necesidad de transición energética, América Latina se posiciona como una región estratégica debido a su vasta disponibilidad de recursos hídricos, solares y eólicos. 

El objetivo principal de este análisis es evaluar los registros históricos de generación eléctrica en Gigavatios-hora (GWh) para identificar los liderazgos regionales, la velocidad de adopción de tecnologías limpias (solar y eólica) y el impacto demográfico en la demanda energética mediante coeficientes de correlación estadística.

---

## 📑 Diccionario de Datos (Metadata)
Los datos combinan métricas de generación mensuales de fuentes energéticas de la base de datos de producción con variables macroeconómicas de población del **Banco Mundial**:

* **PAÍS:** Nación sudamericana evaluada (Argentina, Brasil, Chile, Colombia).
* **AÑO / MES:** Variables temporales del periodo 2015-2022.
* **PRODUCTO:** Tipo de tecnología de generación (`Hydro`, `Wind`, `Solar`, `Geothermal`).
* **VALOR:** Electricidad neta generada medida en Gigavatios-hora (GWh).
* **Población:** Cantidad total de habitantes por país y año (fuente: Banco Mundial) para el cálculo de métricas *per cápita*.

---

## 🎯 Hallazgos y Respuestas a Preguntas de Negocio

### 1. Evolución Temporal y Predominancia de Fuentes
La **energía hidroeléctrica (*Hydro*)** continúa siendo el pilar fundamental y la fuente con mayor volumen de generación en toda la región. 

### 2. Principales Productores de la Región
* **Brasil:** Líder absoluto en volumen total, registrando un acumulado histórico de **3,502,996 GWh** en el periodo evaluado.
* **Colombia:** Ocupa el segundo lugar regional con **486,461 GWh**, impulsado fuertemente por su matriz hidroeléctrica.
* **Chile:** Tercer lugar con **374,869 GWh**.
* **Argentina:** Cuarto lugar con **275,107 GWh**.

### 3. Dinámica Demográfica vs. Producción (Correlación)
El análisis estadístico de correlación demostró que el crecimiento de la infraestructura limpia no siempre va ligado de manera uniforme al aumento de habitantes:
* **Brasil:** Correlación fuerte y positiva (**0.82**). A mayor población, mayor generación de infraestructura.
* **Colombia:** Correlación moderada (**0.35**).
* **Argentina:** Correlación débil (**0.19**).
* **Chile:** Registra una correlación fuertemente negativa (**-0.83**), demostrando que la velocidad de su transición e inversión energética superó e independizó su ritmo de crecimiento demográfico.

### 4. Capacidad Per Cápita e Innovación Tecnológica
* **Energía Eólica:** Brasil domina en volumen vertical, mostrando una curva de crecimiento exponencial en el periodo.
* **Energía Solar:** **Chile** destaca como el referente de mayor crecimiento constante y eficiencia por habitante, apalancado por las condiciones geográficas de zonas como el Desierto de Atacama y políticas públicas de incentivo.

---

## 🛠️ Tecnologías y Herramientas Utilizadas
* **Lenguaje:** Python 3 (Google Colab Environment).
* **Librerías de Datos:** `pandas` para limpieza, filtrado y uniones de datasets; `numpy` para soporte matemático.
* **Librerías de Visualización:** `matplotlib.pyplot` y `seaborn` para la creación de gráficos de líneas, barras apiladas y matrices de correlación.
* **Documentación:** Formato académico bajo normas técnicas para reportes de analítica.

