
# Tarea semana 10
## 1.CREAR UNA VISTA DE FACTURAS CON EL NOMBRE DEL CLIENTE
# Sentencia:
```
CREATE VIEW invoice_view AS
SELECT i.id,1.code,i.create_at,i.total,c.full_name
FROM invoice i JOIN client c
ON c.id = i.client_id;
```
## Captura
1.png
## 2.CREAR UNA VISTA DE DETAIL
# Sentencia:
```
SELECT d.id,d.quantity,d.price,d.quantity * d.price AS total
FROM detail d JOIN product p
ON p.id = d.product_id;
```
## Captura
1.png


