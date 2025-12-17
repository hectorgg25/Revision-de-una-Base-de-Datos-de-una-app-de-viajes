## Ejercicio - Pruebas en la Aplicación de Taxis 🚕 // BASE DE DATOS

### Introducción 🌟
Este proyecto se centra en evaluar y mejorar el funcionamiento de una aplicación de taxis. Abarca dos aspectos importantes: la gestión de logs (registros de actividad) y el análisis de la base de datos que contiene información sobre los taxis, los viajes y las condiciones meteorológicas.

A través de una serie de ejercicios, se identifican las solicitudes provenientes de ciertas direcciones IP, manejar errores en el sistema, y verificar la cantidad de taxis disponibles y su desempeño según diferentes condiciones climáticas. 

El objetivo final es asegurarnos de que el servicio de taxi sea eficiente, confiable y esté alineado con las expectativas de los usuarios.

---

### Servidor 🌐

#### 1: Encontrar Solicitudes de una Dirección IP
LA tarea es averiguar qué solicitudes provienen de una dirección IP que comienza con "233.201".  
**Los registros están en:** `logs/2019/12`.

**Pasos a seguir:**
- Se escribe el comando que usamos para obtener los registros. 🔍
- Incluye un ejemplo de los registros encontrados, como: `184.79.247.161 - - [30/12/2019:21:38:13 +0000] "PUT /alerts HTTP/1.1" 400 3557`.

---

#### 2: Manejo de Errores ⚠️
Hubo errores en el sistema el `12/30/2019`, específicamente errores `400` y `500`.  
**Pasos a seguir:**
- Guarda estos registros en un archivo separado. 🗂️
- Crea una carpeta llamada `bug1` y organiza los registros de manera que haya un archivo principal llamado `main.txt` y otro para cada error (400 y 500).

**Lo que necesitas enviar:**
- Los comandos para crear las carpetas `bug1` y `events`. 📁
- Los comandos para seleccionar los registros que irán en `main.txt`.
- Los comandos para mover los registros a los archivos `400.txt` y `500.txt`.

---

### Base de Datos 📊

#### Información sobre los Datos 📝
- **Tabla de Barrios:**
  - `neighborhood_id`: número del barrio.
  - `name`: nombre del barrio.

- **Tabla de Taxis:**
  - `cab_id`: número único del taxi.
  - `vehicle_id`: identificador del vehículo.
  - `company_name`: nombre de la compañía dueña del taxi.

- **Tabla de Viajes:**
  - `trip_id`: número del viaje.
  - `cab_id`: número del taxi que se usó.
  - `start_ts`: hora de inicio del viaje.
  - `end_ts`: hora de fin del viaje.
  - `duration_seconds`: cuánto duró el viaje (en segundos).
  - `distance_miles`: cuántas millas recorrió el viaje.
  - `pickup_location_id`: barrio donde comenzó el viaje.
  - `dropoff_location_id`: barrio donde terminó el viaje.

- **Tabla de Clima:**
  - `record_id`: número del registro del clima.
  - `ts`: fecha y hora de la medición.
  - `temperature`: temperatura en el momento de la medición.
  - `description`: descripción de las condiciones climáticas (por ejemplo, "lluvia ligera").

**Nota:** No hay un vínculo directo entre los viajes y el clima en la base de datos. Se pueden conectar por la hora de inicio del viaje y la hora de la observación del clima.

#### 1: Número de Taxis en Circulación 🚖
**Objetivo:** Averiguar cuántos taxis hay disponibles en las calles.  
- **Comando que necesitas incluir:**
- Cuenta cuántos automóviles hay en `cabs`.

---

#### 2: Taxis por Compañía 🏢
Cuenta cuántos taxis tiene cada compañía, ordénalos de mayor a menor, y muestra solo aquellas con menos de `100` taxis.  
**Comando que necesitas incluir:**

---

#### 3: Cálculo del Costo del Viaje 💰
**Objetivo:** Verificar si el costo del viaje se está calculando correctamente según el clima. 🌦️
- Usa un método que clasifique el clima como "bueno" o "malo".
- Haz una selección de datos entre `11-05-2017 12:00 am` y `11-06-2017 12:00 am`.

**Comando que necesitas incluir:**

---

#### 4: Número de Viajes por Compañía 📈
Obtén el número de viajes que realizó cada compañía los días `15` y `16 de noviembre de `2017`, y muestra el nombre de la compañía y la cantidad de viajes.  
**Comando que necesitas incluir:**

---

### Conclusión 🎯
Este proyecto nos ayuda a verificar cómo están funcionando los taxis, cómo manejar los errores en los registros y a revisar los datos en la base de datos para mejorar el servicio.

---

Si necesitas más ajustes o adiciones, no dudes en decírmelo.
