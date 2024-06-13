# Tarea en clase de la semana 8
## 1.Escribir una sentencia que muestre los productos que no registren su pais de origen 
# Sentencia:
```
SELECT COUNT(*) - COUNT(country_of_origin) AS product_without_country
FROM product;
```
## Captura
![image](https://github.com/enriqueooo/Tareas_DB/assets/148830588/a8cd942e-1666-49e8-be23-4884268513ef)

## 2.Numero de clientes por ciudad
# Sentencia:
```
SELECT DISTINCT city, COUNT(city)
FROM client
GROUP BY (city)
```
## Captura
![image](https://github.com/enriqueooo/Tareas_DB/assets/148830588/be05f65f-b353-447b-b9d0-6321b6c0fce2)

# Tarea en clase de la semana 8
## 3.Contar el número de productos cuyo precio está dentro de un rango específico 
# Sentencia:
```
SELECT COUNT (*) AS products_price_range_from_90_to_500 
FROM product 
WHERE price > 90 AND price < 500;
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20193544.png

## 4.Seleccionar clientes que viven en una ciudad específica y tienen un tipo de cliente específico
# Sentencia:
```
SELECT * 
FROM client 
WHERE city = 'Philadelphia' AND type_of_client = 'Retai';
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20193836.png

# Tarea en clase de la semana 8
## 5.Seleccionar productos que pertenecen a una categoría específica y cuyo precio está por encima de un valor específico
# Sentencia:
```
SELECT * 
FROM product 
WHERE category = 'Electronics' AND price >= 90;
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20194109.png

## 6.Seleccionar productos que fueron producidos en un año específico y en un país de origen específico
# Sentencia:
```
SELECT * 
FROM product 
WHERE year_of_production = '2023' AND country_of_origin = 'USA';
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20194340.png

# Tarea en clase de la semana 8
## 7.Seleccionar clientes cuyo nombre completo comience con 'J'.
# Sentencia:
```
SELECT * 
FROM client 
WHERE full_name LIKE 'J%';
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20194609.png

## 8. Seleccionar clientes cuya ciudad contenga la letra 'a'
# Sentencia:
```
SELECT * 
FROM client 
WHERE city LIKE '%A%';
```
## Captura
https://github.com/jcalle7/TRABAJOS_BASE_DATOS/raw/main/Capturas/Captura%20de%20pantalla%202024-06-12%20194800.png



















