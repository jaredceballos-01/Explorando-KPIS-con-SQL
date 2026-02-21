# Explorando-KPIS-con-SQL

1. Integración de Datos (ETL SQL)
El código consolida información dispersa en diferentes tablas (ventas_2017, productos, productos_categorias y territorios) utilizando Joins para construir una base de datos maestra que permite ver el detalle de cada pedido junto con su categoría y ubicación geográfica.
2. Cálculo de Métricas de Negocio
Calcula automáticamente los valores financieros que no vienen por defecto en la base de datos:
Ingreso Total: (Precio × Cantidad).
Costo Total: (Costo del Producto × Cantidad).
Beneficio Bruto: La ganancia neta tras descontar los costos.
Margen %: El porcentaje de utilidad sobre las ventas.
3. Análisis de Eficiencia de Marketing (ROI)
Cruza los datos de ventas con la tabla de campanas para determinar el Retorno de Inversión (ROI) por territorio. Esto permite identificar qué países están generando ganancias reales frente a lo que se gasta en publicidad.
4. Control de Calidad de Datos (Data Quality)
Incluye una sección de auditoría para detectar errores comunes que podrían sesgar los reportes:
Búsqueda de valores nulos en llaves primarias (ID de pedido, producto o territorio).
Identificación de registros inválidos (cantidades o precios menores o iguales a cero).
