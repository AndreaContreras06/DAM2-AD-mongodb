# Práctica MongoDB · Gestión de una tienda online

DAM2 · Acceso a Datos · Actividad práctica

## Objetivo

Trabajar con una base de datos MongoDB de una tienda online, realizando operaciones de consulta, inserción, modificación, eliminación, agregación y administración.

Instrucciones:

- Utiliza MongoDB Compass o `mongosh`.
- Resuelve cada ejercicio utilizando la chuleta de comandos.
- Guarda las consultas realizadas en un archivo `soluciones.js`, identificadas por su número.

## Bloque 1. Exploración de la base de datos

1. Muestra todas las bases de datos disponibles.
2. Selecciona la base de datos `tienda`.
3. Lista todas sus colecciones.
4. Averigua cuántos documentos tiene cada colección.
5. Muestra todos los productos registrados.
6. Obtén un único producto.
7. Descubre qué categorías de productos existen.
8. Muestra únicamente el nombre y el precio de todos los productos, sin mostrar su `_id`.

## Bloque 2. Consultas y filtros

9. Busca todos los productos de informática.
10. Encuentra los productos cuyo precio sea superior a 100 €.
11. Busca los productos que cuestan entre 50 € y 500 €, ambos incluidos.
12. Localiza los productos que no tienen stock.
13. Encuentra los productos con stock superior a 10 unidades y precio inferior a 100 €.
14. Busca productos pertenecientes a las categorías `audio` o `movil`.
15. Encuentra los productos que no pertenecen a la categoría `informatica`.
16. Busca productos que cuesten menos de 30 € o tengan más de 50 unidades en stock.
17. Encuentra productos cuyo precio no sea superior a 100 €.
18. Localiza todos los productos cuyo nombre contenga la palabra `móvil`, sin distinguir mayúsculas de minúsculas.

## Bloque 3. Campos, tipos y ordenación

19. Encuentra los productos que tienen el campo `descuento`.
20. Busca los productos que no tienen descuento definido.
21. Comprueba qué productos tienen el precio almacenado como número.
22. Encuentra los productos cuyo precio de venta sea superior a su coste.
23. Ordena los productos del más barato al más caro.
24. Obtén los tres productos más caros.
25. Muestra los tres productos más baratos que tengan stock.
26. Implementa una paginación que muestre tres productos por página, ordenados por `_id`. Obtén las páginas 1, 2 y 3.

## Bloque 4. Inserción y actualización

Realiza estos ejercicios sobre una colección de prácticas.

27. Inserta un producto nuevo con código, nombre, categoría, precio, coste, stock y etiquetas.
28. Inserta cinco productos adicionales en una única operación.
29. Cambia el precio de uno de los productos insertados.
30. Incrementa en 20 unidades su stock.
31. Reduce el precio de todos los productos de una categoría multiplicándolo por `0.9`.
32. Añade un campo `activo` con valor `true` a todos los productos.
33. Cambia el nombre del campo `activo` por `disponible`.
34. Elimina el campo `disponible` de un producto.
35. Realiza una operación `upsert` sobre un producto con código `P999`: si existe, actualízalo; si no, insértalo.
36. Sustituye completamente uno de los documentos de prueba, conservando su `_id`.

## Bloque 5. Eliminación

37. Elimina un producto concreto utilizando su código.
38. Elimina todos los productos de prueba cuyo stock sea cero.
39. Crea una colección temporal, inserta varios documentos y vacíala sin eliminar la colección.
40. Elimina completamente la colección temporal.

## Bloque 6. Arrays y documentos anidados

41. Busca todos los productos que tengan la etiqueta `gaming`.
42. Encuentra productos que tengan simultáneamente las etiquetas `gaming` y `oficina`.
43. Busca productos que tengan exactamente dos etiquetas.
44. Añade una etiqueta `destacado` a un producto.
45. Intenta añadir de nuevo `destacado`, evitando duplicados.
46. Elimina la etiqueta `destacado`.
47. Añade varias etiquetas en una única operación.
48. Añade al producto `P001` dos valoraciones, cada una con usuario y nota.
49. Busca productos con alguna valoración de nota igual o superior a 4.
50. Busca productos que tengan una valoración realizada por `ana` con nota superior o igual a 4, asegurándote de que ambas condiciones se cumplen en la misma valoración.
51. Modifica la nota de una valoración concreta dentro del array.
52. Incrementa en una unidad las notas de todas las valoraciones de un producto de prueba, sin superar el valor máximo permitido que hayas establecido.


