# Deber semana 9
## 1.Obtener la edad promedio de los miembros:
# Sentencia:
```
SELECT AVG(age) AS promedio_edad
FROM members;
```
## Captura
 https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121131.png
## 2.Obtener la edad mínima de los miembros:
# Sentencia:
```
SELECT MIN(age) AS edad_minima
FROM members;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121231.png

## 3.Obtener el número total de registros asistidos:
# Sentencia:
```
SELECT COUNT(*) AS total_registros_asistidos
FROM attendance;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121302.png

## 4.Obtener el número total de asistentes a todas las conferencias
# Sentencia:
```
SELECT COUNT(DISTINCT member_id) AS total_asistentes_unicos
FROM attendance;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121341.png

  ## 5.Obtener el número total de eventos por cada ciudad:
# Sentencia:
```
SELECT city, COUNT(*) AS total_eventos
FROM events
GROUP BY city;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121421.png

## 6.Obtener el número de registros por cada miembro:
# Sentencia:
```
SELECT member_id, COUNT(*) AS total_registros
FROM attendance
GROUP BY member_id;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121513.png

## 7.Obtener el número de registros por cada conferencia:
# Sentencia:
```
SELECT event_id, COUNT(*) AS total_registros
FROM attendance
GROUP BY event_id;
```
## Captura
https://github.com/enriqueooo/Tareas_DB/blob/main/capturas/Captura%20de%20pantalla%202024-06-12%20121644.png

