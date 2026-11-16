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

## Bloque 7. Agregaciones

53. Calcula el precio medio de los productos de cada categoría.
54. Obtén el número de productos por categoría.
55. Calcula el stock total disponible por categoría.
56. Obtén el producto más caro y el más barato de cada categoría.
57. Calcula el margen de beneficio de cada producto (`precio - coste`).
58. Calcula el valor total del inventario de cada categoría (`precio × stock`).
59. Ordena las categorías según su precio medio, de mayor a menor.
60. Obtén una lista de los nombres de productos agrupados por categoría.
61. Descubre qué etiquetas son las más utilizadas.
62. Agrupa los productos en intervalos de precios: 0–50 €, 50–200 € y más de 200 €.
63. Genera un informe que muestre, en una misma operación, el total de productos y las estadísticas por categoría.

## Bloque 8. Relaciones entre colecciones

64. Muestra cada pedido junto con los datos del cliente que lo realizó.
65. Obtén todos los pedidos de Ana.
66. Muestra cada línea de pedido junto con el nombre y precio del producto correspondiente.
67. Calcula el importe total de cada pedido utilizando las cantidades y los precios de los productos.
68. Calcula cuánto ha gastado cada cliente.
69. Obtén el producto del que se han vendido más unidades.

## Bloque 9. Índices y rendimiento

70. Consulta los índices existentes en la colección `productos`.
71. Ejecuta una búsqueda por categoría y examina su plan de ejecución.
72. Crea un índice sobre el campo `categoria`.
73. Repite la consulta anterior y compara los resultados de `explain()`.
74. Crea un índice compuesto sobre `categoria` y `precio`.
75. Crea un índice único sobre `codigo` e intenta insertar un producto con un código duplicado. Explica el resultado.
76. Elimina uno de los índices creados.

## Bloque 10. Validación de documentos

77. Crea una colección `usuarios` donde `nombre` y `email` sean obligatorios.
78. Establece que `edad` sea un número entre 0 y 120.
79. Limita el campo `rol` a los valores `alumno` o `profesor`.
80. Intenta insertar un usuario sin email y comprueba qué ocurre.
81. Inserta un usuario válido.
82. Modifica la validación para incorporar un nuevo campo obligatorio y comprueba su funcionamiento.

## Entrega

Cada alumno debe entregar un archivo `soluciones.js` con las consultas numeradas y los resultados solicitados en los ejercicios de análisis.

## Distribución de la actividad

| Bloque                       | Ejercicios | Prioridad   |
| ---------------------------- | ---------- | ----------- |
| Exploración                  | 1–8        | Obligatorio |
| Consultas y filtros          | 9–18       | Obligatorio |
| Campos y ordenación          | 19–26      | Obligatorio |
| Inserción y actualización    | 27–36      | Obligatorio |
| Eliminación                  | 37–40      | Obligatorio |
| Arrays y documentos anidados | 41–52      | Obligatorio |
| Agregaciones                 | 53–63      | Obligatorio |
| Relaciones                   | 64–69      | Obligatorio |
| Índices y rendimiento        | 70–76      | Ampliación  |
| Validación                   | 77–82      | Ampliación  |
