# sql-select-fundamentals

¿Por qué es mala práctica usar SELECT * en producción? Mencioná al menos dos razones concretas (rendimiento, mantenibilidad, seguridad).

Es una mala practica usar select en todas las búsquedas sobre todo en producción ya que en estos ámbitos se suelen tener una gran cantidad de columnas y una enorme cantidad de datos, al pedir todos estos datos que pueden no ser necesarios en cada una de las consultas puede llevar a tomar muchísimo mas tiempo en cada una de las consultas además de recursos de nuestro computador, lo que puede llevar a que se cierre o se crashee nuestro programa y en sobrecostos para la compañía. 

¿Por qué son importantes los alias para un stakeholder no técnico? Explicá con un ejemplo concreto cómo un alias transforma total_amount en algo que cualquier persona del área de finanzas puede interpretar directamente.

Los alias son importantes en el ámbito del análisis de datos porque nos permiten expresar las columnas de datos en lenguaje que pueda ser mas claro para personas que no están detrás de todo el desarrollo de la base de datos y asi mismo poderlo llevar a modelos BI que nos permita presentar nuestros insights. Con el ejemplo de total_amount una persona que no entienda ingles o que no sepa exactamente a que se refiere esa columna podríamos ponerle un alas mas claro como valor_total_de_venta, permitiendo que sea un poco mas claro para personas que no están detrás de todo el modelado de datos. 
