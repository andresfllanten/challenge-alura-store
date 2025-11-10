# challenge-alura-store
El proposito es ayudar al Sr. Juan a decidir qué tienda de su cadena Alura Store debe vender para iniciar un nuevo emprendimiento. Para ello, analizarás datos de ventas, rendimiento y reseñas de las 4 tiendas de Alura Store. El objetivo es identificar la tienda menos eficiente y presentar una recomendación final basada en los datos.

# 📚 Proyecto de Análisis de Datos para la Decisión de Venta de Tiendas

## 📝 Descripción del Proyecto

Este proyecto fue desarrollado para asistir a la dirección en la toma de decisiones estratégicas, específicamente, la identificación de la tienda menos viable dentro de una cadena de cuatro sucursales (Tienda 1 a Tienda 4). El análisis se centra en métricas clave de rendimiento, eficiencia y satisfacción del cliente para justificar una recomendación de venta.

El objetivo principal es determinar cuál de las tiendas (1, 2, 3 o 4) debe ser vendida, basándose en el peor desempeño consolidado entre **Ingreso Total**, **Costo de Envío Promedio** y **Calificación de Clientes**.

## 🚀 Factores Analizados

El informe final se justifica con el análisis comparativo de los siguientes factores:

1.  **Ingresos Totales (Rendimiento Financiero):** Suma total de los precios de los productos vendidos por cada tienda.
2.  **Costo de Envío Promedio (Eficiencia Operativa):** Costo logístico medio por transacción.
3.  **Calificación Promedio de Clientes (Satisfacción):** Promedio de las calificaciones recibidas (1 a 5).
4.  **Ventas por Categoría y Producto:** Análisis de los artículos más y menos vendidos en cada sucursal para identificar tendencias de mercado o problemas de stock.

## 🛠️ Requisitos y Dependencias

Este proyecto fue desarrollado en Python y requiere las siguientes librerías:

* **`pandas`**: Para la carga, limpieza y manipulación de los datos estructurados (DataFrames).
* **`matplotlib`**: Para la generación de gráficos de visualización (barras, dispersión, torta) utilizados en la justificación.
* **`numpy`**: Para cálculos numéricos avanzados (aunque no es el foco principal, es común en entornos de análisis de datos).

## 💻 Estructura del Código

El código de análisis se ejecuta en un único script (o celda de un entorno Colab) y sigue la siguiente estructura lógica:

1.  **Carga y Consolidación de Datos:** Se cargan los cuatro archivos CSV desde GitHub y se concatenan en un único DataFrame (`df_consolidado`), asignando un `ID_Tienda` único a cada fuente.
2.  **Limpieza de Datos:** Conversión de las columnas `Precio`, `Costo de envío` y `Calificación` a formato numérico y eliminación de filas con valores nulos en estas columnas críticas.
3.  **Análisis por Ítem:** Ejecución de cálculos y generación de gráficos para cada una de las 5 métricas requeridas.

## ⚙️ Uso y Ejecución

Para ejecutar el análisis:

1.  **Entorno:** Se recomienda utilizar Google Colab o un entorno Python local (Jupyter Notebooks o IDE con los paquetes instalados).
2.  **Librerías:** Asegúrese de tener instaladas las dependencias (`pip install pandas matplotlib numpy`).
3.  **Ejecución:** Ejecute el script Python. El código imprimirá los resultados tabulares en la consola y mostrará los gráficos generados para cada uno de los 5 ítems de análisis.

## 💡 Conclusión del Análisis (Resumen)

El análisis concluye que la **Tienda 3** es la más problemática y debe ser vendida, a pesar de que la Tienda 4 tiene el menor ingreso bruto. La Tienda 3 combina los siguientes factores negativos:

* **Costo de Envío Más Alto** (\$19,709.80), afectando severamente el margen de beneficio.
* **Calificación Promedio Más Baja** (2.986), indicando problemas de calidad o logística.

La venta de la Tienda 3 permite eliminar el foco de la mayor ineficiencia operativa y la mayor insatisfacción de clientes.
