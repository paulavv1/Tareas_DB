
# Tarea semana 10
## 1.CREAR UNA VISTA DE FACTURAS CON EL NO,BRE DEL CLIENTE
# Sentencia:
```
CREATE VIEW invoice_view AS
SELECT i.id,1.code,i.create_at,i.total,c.full_name
FROM invoice i JOIN client c
ON c.id = i.client_id;
```
## Captura
1.png

