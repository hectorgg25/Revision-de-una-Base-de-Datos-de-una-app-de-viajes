# PROYECTO Sprint 6 - Héctor Gamboa
# Pruebas en Base de Datos de la App URBAN Routes 🚕 
 
# 📚Técnicas - Tecnologías utilizadas:

- SQL.

# 📃 Creación de pruebas:

🔵 Objetivo: verificar cuántos taxis hay actualmente en las calles.

Pasos:

-Conectarse a la base de datos chicago_taxi.

-Contar el número de automóviles en la tabla cabs.

* Resultado esperado: número total de taxis + consulta usada.

🟢 Objetivo: analizar cuántos taxis tiene cada compañía.

Pasos:

Contar los autos agrupados por company_name (compañia).

-Usar HAVING para filtrar compañías con menos de 100 autos.

-Ordenar en orden descendente por cantidad.

* Resultado esperado: lista de compañías con menos de 100 autos + consulta usada.

🟡 Objetivo: verificar el cálculo del coeficiente de viajes según el clima.

Pasos:

-Tomar datos de la tabla weather_records.

-Clasificar con CASE:

-Bad si la descripción contiene “rain” o “storm”.

-Good en otros casos.

-Seleccionar entre 11-05-2017 00:00 y 11-06-2017 00:00.

* Resultado esperado: tabla con columnas (ts, weather_conditions) + consulta usada.

🔴 Objetivo: comprobar número de viajes de cada compañía en fechas específicas.

Pasos:

-Conectar tablas cabs y trips.

-Agrupar por company_name.

-Contar viajes (trips_amount) en 15 y 16 de noviembre de 2017.

-Ordenar por trips_amount en orden descendente.

* Resultado esperado: tabla con compañías y número de viajes + consulta usada.

# 📝 Ejecución de pruebas:

🔴 La ejecucion de las pruebas arriba mencionadas nos ayudara a lo siguinete:

¿Tenemos suficientes taxis?

¿Cómo se distribuyen por compañía?

¿El cálculo de tarifas es correcto según el clima?

¿La cantidad de viajes coincide con lo reportado?

Esto sirve para ajustar la flota, renegociar con compañías, mejorar la lógica de tarifas y garantizar la fiabilidad de los datos.

Liga don el archivo de resultados:
https://docs.google.com/document/d/1_bnsUho_VOJYdWpZ9nTX8IBi-vBx3Naw?rtpof=true&usp=drive_fs


