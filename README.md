# proyecto_5_estadistica
Análisis estadístico del comportamiento de clientes en Megaline | Comparación de ingresos en planes de telecomunicaciones | Hipótesis de rentabilidad e impacto regional 

# ANÁLISIS DE LAS TARIFAS DE PREPAGO SURF Y ULTIMATE DE MEGALINE
## RESUMEN DEL PROYECTO
Este proyecto es un análisis preliminar para el operador de telecomunicaciones Megaline. El objetivo es determinar cuál de las dos tarifas de prepago, Surf o Ultimate, genera más ingresos para la empresa. Para ello, se analizó el comportamiento de una muestra de 500 clientes durante el año 2018, examinando la cantidad de llamadas, mensajes de texto y datos móviles utilizados. El resultado servirá para que el departamento comercial pueda ajustar el presupuesto de publicidad de manera más efectiva.

## OBJETIVO
El objetivo principal es comparar la rentabilidad de las tarifas Surf y Ultimate basándose en los patrones de uso de los clientes. El fin último es proporcionar una base sólida para que Megaline pueda tomar decisiones estratégicas sobre su modelo de negocio y sus campañas de marketing.

## METODOLOGÍA DE ANÁLISIS
### 1. DESCRIPCIÓN DE LOS DATOS
- Se utilizaron cinco conjuntos de datos proporcionados por Megaline:
  - users: Datos de los clientes.
  - calls: Información sobre las llamadas realizadas.
  - messages: Datos de los mensajes de texto enviados.
  - internet: Información sobre el consumo de datos móviles.
  - plans: Detalles de las dos tarifas de prepago.

### 2. PREPROCESAMIENTO DE DATOS
Ajuste de Tipos de Datos: Se ajustaron los tipos de datos de las columnas relevantes (por ejemplo, convertir fechas a formato datetime) para facilitar los cálculos.
Tratamiento de Errores: Se identificaron y corrigieron errores en los datos, como las llamadas con duración cero, que se asumieron como llamadas no conectadas.
Cálculo de Ingresos Mensuales: Se calcularon los ingresos mensuales por usuario, sumando la tarifa mensual fija del plan más los cargos por excedentes en minutos de llamadas, mensajes de texto y datos móviles. Se aplicaron las reglas de redondeo específicas de cada plan.

### 3. PRUEBA DE HIPÓTESIS
- Se formularon y probaron dos hipótesis estadísticas con un nivel de significancia de 0.05:
  - Hipótesis 1: El ingreso promedio mensual de los usuarios del plan Ultimate es diferente al de los usuarios del plan Surf.
    - Hipótesis nula (H 0): El ingreso promedio mensual de los usuarios de ambos planes es igual.
    - Hipótesis alternativa (H1): El ingreso promedio mensual de los usuarios de ambos planes es diferente.

  - Hipótesis 2: El ingreso promedio mensual de los usuarios en la región de Nueva York-Nueva Jersey es diferente al de los usuarios de otras regiones.
    - Hipótesis nula (H 0): El ingreso promedio mensual de los usuarios de ambas regiones es igual.
    - Hipótesis alternativa (H 1​): El ingreso promedio mensual de los usuarios de ambas regiones es diferente.

Se utilizó la prueba t de Student para muestras independientes para comparar las medias de los grupos.

### CONCLUSIONES PRINCIPALES
El plan Ultimate genera un ingreso promedio mensual significativamente mayor que el plan Surf.
Megaline depende en gran medida de los cargos por excedentes, lo que representa aproximadamente el 84% de los ingresos totales.
Esta dependencia es especialmente notable en el plan Surf.
El ingreso promedio mensual de los usuarios en Nueva York-Nueva Jersey es estadísticamente diferente al de los usuarios de otras regiones.
Se recomienda a Megaline equilibrar los ingresos por excedentes con la satisfacción del cliente. 
Se sugiere revisar los límites del plan Surf para reducir los cargos adicionales y considerar estrategias de upselling (ofrecer Ultimate a usuarios de alto consumo) y downselling (ofrecer Surf a usuarios que no aprovechan Ultimate).

### TECNOLOGÍAS UTILIZADAS
- Python
- Pandas
- NumPy
- Matplotlib y Seaborn
- SciPy
- Jupyter Notebook
- Vivual Studio Code
