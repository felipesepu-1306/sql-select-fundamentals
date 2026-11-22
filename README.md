# sql-select-fundamentals

A. ¿Por qué es mala práctica usar SELECT * en producción? Mencioná al menos dos razones concretas (rendimiento, mantenibilidad, seguridad).

1. La primera razon es por el tiempo que puede tomar cada consulta, ya que si consultamos todas las columnas en vez de la informacion especifica que necesitamos va a traer un monton de datos a nuestra query, que no son necesarios y al hacer esto el tiempo se va a incrementar bastante.

2. La segunda razon son los costos que conlleva traer toda esa informacion desde un repositorio o base de datos en linea, ya que puede llevar mucho tiempo la consulta y esto elevaria los costos del proceso.

3. Otra razon que me gustaria agregar es por temas de mantenibilidad a largo plazo, ya que si se modifica una columna o se modifica la estructura al traer todo la tabla nos puede llegar a generar errores. 

B. ¿Por qué son importantes los alias para un stakeholder no técnico? Explicá con un ejemplo concreto cómo un alias transforma total_amount en algo que cualquier persona del área de finanzas puede interpretar directamente.

Los alias son importantes en el ámbito del análisis de datos porque nos permiten expresar las columnas de datos en lenguaje que pueda ser mas claro para personas que no están detrás de todo el desarrollo de la base de datos y asi mismo poderlo llevar a modelos BI que nos permita presentar nuestros insights. Con el ejemplo de total_amount una persona que no entienda ingles o que no sepa exactamente a que se refiere esa columna podríamos ponerle un alas mas claro como valor_total_de_venta, permitiendo que sea un poco mas claro para personas que no están detrás de todo el modelado de datos. 

SELECT total_amount AS monto_total
FROM sales;
