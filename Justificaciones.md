Justificaciones de las decisiones tomadas sobre el tablero en Dim_Clientes, Dim_Productos y Dim_Categorias 

Los registros de email y ciudad que contenían valores nulos fueron reemplazados por la leyenda "Sin dato" 
ya que esos clientes siguen existiendo dentro de la base de datos y eliminarlos implicaría perder información útil para futuros análisis. 
Esta decisión permite conservar la integridad del conjunto de datos e indicar claramente que esa información no estaba disponible.

El valor nulo de la columna categoría fue reemplazado por "Sin Categoría" para mantener el registro del producto sin eliminar información.
  
El producto con el precio nulo se mantuvo en la tabla y su valor fue reemplazado por 0, ya que ese producto está relacionado con registros de ventas. 
Eliminarlo habría generado inconsistencias en la relación entre Dim_Productos y Fact_Ventas. De esta manera se conserva la integridad referencial 
del modelo y se evita perder transacciones asociadas.
    
