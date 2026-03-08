# Test A/B y Validación Estadística
-------------------------------------
## 📝 Descripción del Proyecto
- Este proyecto consiste en un análisis estadístico avanzado para evaluar la efectividad de un cambio implementado en la plataforma (Versión B) frente a la versión actual (Versión A). El objetivo es determinar si las diferencias observadas en los ingresos de los usuarios son estadísticamente significativas o producto del azar, permitiendo tomar decisiones basadas en datos sobre la implementación final del cambio.

## 🎯 Objetivos
- Análisis Descriptivo: Caracterizar el comportamiento de los ingresos en ambos grupos mediante métricas de tendencia central y dispersión.
- Verificación de Supuestos: Evaluar la normalidad y la homocedasticidad de las muestras para seleccionar el test estadístico adecuado.
- Prueba de Hipótesis: Ejecutar un test de significancia para validar si el incremento de ingresos en el Grupo B es representativo.

## 🛠️ Tecnologías y Librerías
- Python (versión 3.x)
- Librerías principales: * pandas y numpy para la manipulación y estructuración de datos.
- matplotlib y seaborn para la visualización de distribuciones y comparativas.
- scipy.stats para la ejecución de pruebas de Shapiro-Wilk, Levene y Mann-Whitney U.

## 📈 Hallazgos Principales
- Comportamiento de la Distribución: Ambas muestras presentan un sesgo positivo pronunciado, lo que indica que la mayoría de los usuarios generan ingresos bajos, con unos pocos usuarios de alto valor desplazando la media.
- Incremento en Métricas: El Grupo B mostró una media de ingresos de 121.82, superando la media del Grupo A de 99.17.
- Validación de Datos: Se confirmó que los datos no siguen una distribución normal (p-valor < 0.05 en Shapiro-Wilk), lo que invalidó el uso de pruebas paramétricas como el T-Test.
- Diferencia Significativa: El test de Mann-Whitney U arrojó un p-valor de 0.0000, confirmando que la diferencia a favor del Grupo B es estadísticamente sólida.

## ✅ Resultados y Conclusiones
- Recomendación de Inversión: Se aconseja proceder con el despliegue total de la versión probada en el Grupo B, ya que garantiza un retorno de ingresos superior de manera consistente.
- Análisis de Riesgo: Aunque el Grupo B tiene un mejor desempeño, presenta una mayor desviación estándar (79.28). Se recomienda monitorear la volatilidad de los ingresos en este segmento.
- Optimización Estratégica: Dada la naturaleza no normal de los ingresos, las futuras estrategias de marketing deben enfocarse en los segmentos de "usuarios premium" que se encuentran en la cola larga de la distribución, ya que son los que más impactan en la rentabilidad total.
