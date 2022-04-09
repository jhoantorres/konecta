# konecta
Presentación prueba

Autor: Jhoan Manuel Torres Boada
Espero les guste, pueden haber cosas por mejorar, y si me dan la oportunidad las mejorare sin duda!

Instalacion:
Primero instalaremos el proyecto JAVA
Sin correrlo aun continuaremos instalando la bd y los datos de ella

Consultas SQL

El producto mas vendido
SELECT SUM(t.cantidad_vendida) as totalvendido, t.id_producto, p.nombre_producto FROM konecta.transaccion as t INNER JOIN producto as p ON t.id_producto = p.idproducto group by t.id_producto order by 1 DESC LIMIT 1;

El producto que tiene mayor stock
SELECT stock_producto,nombre_producto FROM konecta.producto order by 1 DESC LIMIT 1;
