# TelecomX_Challenge
Challenge TelecomX Data Science.

Análisis de Cancelación de Clientes (Churn) en Telecomunicaciones
Descripción del Proyecto
Este proyecto tiene como objetivo principal realizar un análisis exploratorio y predictivo sobre la cancelación de clientes (churn) en una empresa de telecomunicaciones. A través de un proceso de Extracción, Transformación y Carga (ETL), se limpian, preparan y analizan los datos para identificar los factores que influyen en la decisión de un cliente de cancelar su servicio. El análisis busca proporcionar información valiosa para comprender el comportamiento de los clientes y desarrollar estrategias efectivas de retención.

Datos
El análisis se basa en el conjunto de datos TelecomX_Data.json, que contiene información sobre clientes de una empresa de telecomunicaciones, incluyendo datos demográficos, servicios contratados, información de facturación y estado de cancelación (Churn).

Análisis Realizado
El cuaderno realiza los siguientes pasos clave:

Extracción de Datos: Carga de los datos desde un archivo JSON.
Transformación de Datos:
Normalización de columnas anidadas.
Limpieza y conversión de tipos de datos (ej. Charges.Total).
Manejo de valores nulos.
Creación de variables dummy para características categóricas.
Creación de nuevas características (ej. Cuentas_Diarias).
Traducción y reorganización de columnas para facilitar la interpretación.
Análisis y Visualización:
Análisis de la distribución de la cancelación.
Comparativa de estadísticas (media, mediana, desviación estándar) entre clientes que cancelan y los que no, en relación con el tiempo de contrato y gastos.
Análisis de la proporción de servicios (teléfono, internet DSL/Fibra) según el estado de cancelación.
Análisis de la proporción de servicios adicionales (seguridad, backup, soporte, streaming) según el estado de cancelación.
Análisis de la proporción de métodos de pago según el estado de cancelación.
Análisis de la proporción de tipos de contrato según el estado de cancelación.
Análisis de la relación de cancelación con características demográficas (género, jubilado, dependientes).
Visualización de la relación entre cancelación, gasto total y tiempo de contrato.
Cálculo y visualización de la matriz de correlación entre variables clave y la cancelación.

Hallazgos Clave
Los principales insights obtenidos del análisis incluyen:

Los clientes con contratos mensuales, servicio de Internet de Fibra Óptica y que utilizan el pago con cheque electrónico muestran una mayor propensión a cancelar.
Una menor antigüedad (pocos Meses_Contrato) y un menor Cuentas_Totales acumulado están asociados con una mayor probabilidad de cancelación.
Los servicios adicionales de seguridad y soporte técnico parecen estar asociados con una menor tasa de cancelación.
Los contratos a largo plazo (1 y 2 años) están fuertemente correlacionados con una menor cancelación.
Los pagos automáticos (transferencia bancaria y tarjeta de crédito) están asociados con una menor tasa de cancelación en comparación con los cheques.

Recomendaciones
Basado en el análisis, se sugieren las siguientes recomendaciones:

Fomentar la adopción de contratos a largo plazo y métodos de pago automáticos.
Investigar las razones detrás de la alta tasa de cancelación entre usuarios de Fibra Óptica y pagos con cheque electrónico.
Promocionar los servicios de seguridad y soporte técnico como herramientas de retención.
Identificar y dirigir estrategias de retención específicas a clientes con alto riesgo de cancelación (ej. contratos mensuales, baja antigüedad, alto coste diario).

Cómo Ejecutar el Cuaderno

Asegúrate de tener Google Colab o un entorno Python con las bibliotecas pandas, numpy, matplotlib y seaborn instaladas.
Sube el archivo TelecomX_Data.json a tu entorno (por ejemplo, a Google Drive si usas Colab, en una carpeta llamada Colab Notebooks).
Ejecuta las celdas del cuaderno secuencialmente. Asegúrate de montar Google Drive si el archivo está almacenado allí.
