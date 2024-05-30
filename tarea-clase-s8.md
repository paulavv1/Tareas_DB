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





