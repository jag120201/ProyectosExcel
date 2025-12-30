Análisis de ventas conforme al tiempo
🔍 Validación de Calidad de Datos
Durante el proceso de análisis se realizó una revisión exhaustiva de la calidad de los datos mediante el uso de funciones de Excel para la detección de errores y celdas vacías.
•	Se comprobó que no existen errores de cálculo o de tipo de dato en las columnas analizadas, lo que garantiza la fiabilidad del dataset para la creación de KPIs.
•	Las celdas vacías identificadas no representan incoherencias ni errores de registro, sino que responden a la naturaleza del propio dato.
•	Por ejemplo, el campo STATE solo aplica a países como Estados Unidos, mientras que en otros países (como España) este campo no es obligatorio ni relevante, por lo que su ausencia es correcta.
•	De igual forma, campos como direcciones secundarias pueden aparecer en blanco sin afectar a la integridad de la información principal.
Gracias a esta validación, se concluye que el dataset es consistente, coherente y apto para el análisis, sin necesidad de correcciones forzadas.
🔧 Cambios Realizados
Durante el proceso de preparación y análisis de los datos, se realizaron los siguientes cambios y mejoras:
•	Recalcular SALES ya que estaba mal calculado.
•	Creación de la columna NET_SALES para calcular correctamente las ventas reales, excluyendo pedidos no completados. En el que clasificamos:
o	Pedidos completados (Shipped, Resolved)
o	Pedidos pendientes (In Process, On Hold, Disputed)
o	Pedidos cancelados (Cancelled)
•	Uso de tablas dinámicas para la creación de todos los KPIs, permitiendo un análisis dinámico y escalable.
•	Análisis temporal a partir del campo ORDERDATE, permitiendo estudiar tendencias mensuales y anuales.
•	Creación de un campo Nombre Completo del Contacto, combinando nombre y apellido para una mejor presentación.
•	Estandarización de todos los KPIs utilizando Net Sales, evitando resultados inflados por pedidos cancelados o pendientes.
________________________________________
📈 KPIs Desarrollados
El dashboard incluye los siguientes indicadores clave de rendimiento:
•	Ventas Totales
•	Ventas Netas
•	Ventas Canceladas
•	Ventas Pendientes
•	Ventas Promedio
•	Ventas por línea de productos
•	Ventas en el tiempo
•	Top 10 Clientes
•	Ventas totales por país.
________________________________________
🧠 Resumen del Proyecto
Este proyecto se centra en el análisis de datos de ventas con el objetivo de comprender el rendimiento del negocio a lo largo del tiempo, por productos, clientes y regiones. Mediante la limpieza de los datos y la diferenciación entre ventas brutas y ventas reales (netas), el análisis ofrece una visión mucho más precisa de los ingresos reales de la empresa.
________________________________________
📊 Conclusiones y Principales Insights
•	Hay tendencias de ventas por países.
•	Existen claras tendencias temporales en las ventas: hay meses con mayores niveles de ventas que otros, lo que indica la presencia de estacionalidad en la demanda.
•	No todas las ventas registradas representan ingresos reales: es fundamental filtrar por estado del pedido para evitar sobreestimar el rendimiento del negocio.
•	Un número reducido de clientes concentra una parte significativa de las ventas totales, destacando la importancia de los clientes clave.
•	Algunas líneas de producto superan claramente a otras en volumen de ventas, lo que abre oportunidades para optimizar estrategias comerciales y de inventario.
En conjunto, el proyecto demuestra cómo una correcta limpieza de datos, una definición clara de KPIs y un análisis temporal estructurado permiten obtener conclusiones fiables y accionables para el negocio.
