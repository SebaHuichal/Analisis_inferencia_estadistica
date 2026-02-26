# 📘 Resumen del Flujo de Proyecto (Lecciones 1 a 6)

## 🎯 Visión General del Proyecto
El objetivo principal de este proyecto ha sido simular y ejecutar un **ciclo completo de investigación cuantitativa** aplicando la inferencia estadística. El flujo abarca desde el planteamiento del problema mediante el método científico hasta la validación de hipótesis para la toma de decisiones en el ámbito de la salud universitaria, pasando por el cálculo de probabilidades, modelado de distribuciones y estimación de parámetros.

---

## 🛠️ Desglose por Lección

### 1️⃣ Lección 1: Método Científico y Estadística
* **Objetivo:** Formular el problema de investigación, definir las hipótesis de trabajo y diseñar la metodología de estudio.
* **Procesos Principales:**
  * **Planteamiento del Problema:** Identificación del déficit de sueño y sedentarismo en los estudiantes.
  * **Definición de Hipótesis:** Establecer la suposición de que la carga académica impacta negativamente en el tiempo de descanso y ejercicio.
  * **Selección de Variables:** Clasificación de variables sociodemográficas (Facultad) y de salud (Horas de sueño, Minutos de ejercicio, Consumo de ultraprocesados).
  * **Diseño Muestral:** Definición de una muestra representativa de $n=385$ estudiantes.
* **Salida:** Marco metodológico y diseño de la investigación estructurado.

### 2️⃣ Lección 2: Probabilidad y Estadística
* **Objetivo:** Definir eventos aleatorios a partir de los datos y calcular probabilidades empíricas de riesgo.
* **Herramientas Clave:** Teoría de conjuntos y reglas de probabilidad en Python (`pandas`).
* **Procesos Principales:**
  * **Definición de Eventos:** Creación de eventos dicotómicos (Ej. Evento D: Duerme $\geq$ 7 horas).
  * **Cálculo de Riesgos:** Uso de operaciones de conjuntos para calcular probabilidades simples (Complemento), conjuntas (Intersección) y combinadas (Unión) para entender la proporción de estudiantes en riesgo de salud.
* **Salida:** Mapa probabilístico del estado de salud de la muestra empírica.

### 3️⃣ Lección 3: Distribución de Probabilidad
* **Objetivo:** Modelar matemáticamente el comportamiento de las variables clave utilizando distribuciones teóricas.
* **Herramientas Clave:** `scipy.stats` (norm, poisson, binom), `seaborn`, `matplotlib`.
* **Procesos Principales:**
  * **Asignación de Modelos:** Distribución Normal para variables continuas (Sueño, Ejercicio) y Poisson para variables discretas (Conteo de comidas rápidas).
  * **Cálculo de Probabilidades Teóricas:** Uso de funciones de masa (PMF) y distribución acumulada (CDF) para calcular probabilidades exactas de escenarios críticos (Ej. $P(X < 7)$ horas de sueño).
  * **Visualización:** Creación de gráficos de densidad y barras con umbrales de riesgo.
* **Salida:** Validaciones probabilísticas respaldadas por modelos teóricos y gráficos de distribución empírica vs. teórica.

### 4️⃣ Lección 4: Distribución Muestral y Teorema del Límite Central (TLC)
* **Objetivo:** Comprobar empíricamente el Teorema del Límite Central mediante técnicas de remuestreo (Bootstrapping).
* **Herramientas Clave:** `numpy` (`random.choice`), `pandas`, `matplotlib`.
* **Procesos Principales:**
  * **Simulación:** Extracción de 1000 submuestras aleatorias de distintos tamaños ($n=5, 30, 100$).
  * **Comprobación del TLC:** Demostrar que la distribución de las medias muestrales adopta una forma Normal (campana de Gauss) independientemente de la distribución de los datos originales.
  * **Análisis de Dispersión:** Visualizar cómo el aumento del tamaño muestral ($n$) reduce radicalmente el Error Estándar.
* **Salida:** Demostración matemática y visual de la fiabilidad de extraer muestras para predecir comportamientos poblacionales.

### 5️⃣ Lección 5: Inferencia e Intervalos de Confianza para la Media
* **Objetivo:** Estimar los parámetros reales de toda la población universitaria a partir de los datos de la muestra.
* **Herramientas Clave:** `scipy.stats` (t-Student).
* **Procesos Principales:**
  * **Cálculo de Intervalos:** Estimación del verdadero promedio de horas de sueño y minutos de ejercicio de la universidad al 95% de confianza.
  * **Análisis de Trade-off:** Comparación de intervalos al 90%, 95% y 99% de confianza, evaluando cómo mayor seguridad implica menor precisión.
  * **Impacto de la Muestra:** Visualización de cómo el tamaño total de la encuesta ($n=385$) garantiza intervalos estrechos y de alta utilidad analítica frente a muestras pequeñas.
* **Salida:** Rangos poblacionales estimados (Intervalos de Confianza) listos para interpretación de negocio y salud pública.

### 6️⃣ Lección 6: Test de Significancia (Pruebas de Hipótesis)
* **Objetivo:** Validar afirmaciones sobre la población y descartar el azar mediante rigor estadístico para guiar la toma de decisiones institucionales.
* **Herramientas Clave:** `scipy.stats` (`ttest_1samp`, `ttest_ind`).
* **Procesos Principales:**
  * **Prueba Poblacional (1 Muestra):** Confirmación estadística de que el déficit de sueño es un problema real a nivel general ($p-value < \alpha$).
  * **Prueba Comparativa (2 Muestras):** Comparación entre facultades (Ingeniería vs. Salud) para determinar si la fatiga es transversal o aislada a ciertas carreras.
  * **Gestión de Riesgos:** Identificación y mitigación de Falsos Positivos (Error Tipo I) y Falsos Negativos (Error Tipo II) respaldados por el alto poder estadístico de la muestra.
* **Salida (Entregable Final):** Conclusiones definitivas y recomendaciones basadas en evidencia matemática irrefutable.



---

## 🏁 Conclusión
El flujo de trabajo ha transformado un problema de salud cualitativo y empírico en un **diagnóstico cuantitativo robusto**. Se ha transitado metodológicamente desde la estadística descriptiva inicial hacia la inferencia avanzada, entregando a las autoridades universitarias evidencia matemática rigurosa y libre de sesgos para la formulación e implementación de nuevas políticas de bienestar estudiantil.
