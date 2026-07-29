# Entrevista Simulada - Benjamin

## Resumen de Evaluación

**Tema principal:**

JPA, DTOs y SQL básico.

**Nivel observado:**

Inicial.

**Fortalezas:**

- Reconoce parcialmente la relación entre objetos y base de datos.
- Identifica la idea de traer solo la información necesaria hacia el frontend.
- Logra iniciar la creación de una base de datos en SQL.

**Puntos a reforzar:**

- Definición precisa de JPA, ORM, entidad y persistencia.
- Uso de DTOs para evitar exponer entidades directamente.
- Sintaxis SQL para creación de tablas, inserción de datos y consultas.

**Recomendación de estudio:**

Repasar JPA con entidades simples, practicar DTOs en Spring Boot y resolver ejercicios SQL de creación, inserción y consulta de datos.

---

## Pregunta 1

**Enunciado:**

¿Qué es JPA?

**Respuesta del candidato:**

JPA Es una herrmienta que permite transformar la Base de datos En objeto.

**Observaciones:**

- Reconoce parcialmente la relación entre JPA, objetos y base de datos.
- La explicación es imprecisa: JPA no transforma directamente la base de datos en objetos, sino que define una especificación para mapear entidades Java a tablas relacionales.
- Debe reforzar conceptos como entidad, ORM, persistencia y repositorios.
- Sería recomendable mencionar Hibernate como implementación común de JPA.

---

## Pregunta 2

**Enunciado:**

¿Por qué no conviene devolver una entidad JPA al frontend?

**Respuesta del candidato:**

Porque es mas rápido traer solo la información que se requiere.

**Observaciones:**

- La respuesta identifica la idea de devolver solo la información necesaria, lo cual es positivo.
- Falta profundizar en riesgos de exponer entidades directamente, como fuga de datos sensibles, acoplamiento con el modelo interno y problemas de serialización.
- Se esperaba mencionar el uso de DTOs para controlar qué datos se envían al frontend.

---

## Pregunta 3

**Enunciado:**

Crear una base de datos llamada `empresa`.

**Respuesta del candidato:**

```sql
CREATE DATABASE empresa;
CREATE TABLE empleados(
   id PRIMARY KEY,
   nombre VARCHAR(50),
   area VARCHAR(50),
   salario DECIMAL(10,2)
)
```

**Observaciones:**

- Crea la base de datos solicitada correctamente.
- La respuesta incluye también parte de la creación de tabla, aunque esta corresponde a la siguiente pregunta.
- Nota: no continúa por tiempo.

---

## Pregunta 4

**Enunciado:**

Crear una tabla llamada `empleados` con estas columnas:

- `id` número, identificador único.
- `nombre` texto.
- `área` texto, como "Ventas" o "IT".
- `salario` número.

**Respuesta del candidato:**

Ver respuesta registrada en la Pregunta 3.

**Observaciones:**

- Intenta crear la tabla `empleados`, pero la definición está incompleta.
- Falta definir el tipo de dato para `id`, por ejemplo `INT`, antes de declarar `PRIMARY KEY`.
- Falta cerrar la sentencia con punto y coma.
- Nota: no continúa por tiempo.

---

## Pregunta 5

**Enunciado:**

Insertar 5 empleados de ejemplo, por ejemplo: "Juan, Ventas, 3000".

**Respuesta del candidato:**

No registrada.

**Observaciones:**

- No se registra respuesta para la inserción de empleados.
- Se esperaba el uso de sentencias `INSERT INTO empleados (...) VALUES (...)` con cinco registros.
- Nota: no continúa por tiempo.

---

## Pregunta 6

**Enunciado:**

Hacer estas consultas:

- Mostrar todos los empleados de un área específica, por ejemplo "IT".
- Mostrar empleados con salario mayor a X, por ejemplo "> 2000".
- Calcular el salario promedio de todos los empleados.

**Respuesta del candidato:**

No registrada.

**Observaciones:**

- No se registran las consultas solicitadas.
- Se esperaba uso de `SELECT`, filtros con `WHERE` y función de agregación `AVG` para el promedio de salarios.
- Nota: no continúa por tiempo.

---

## Resumen Final

Benjamin muestra una comprensión inicial de algunos conceptos, pero necesita reforzar definiciones técnicas y práctica SQL. El siguiente paso sugerido es construir un CRUD simple con Spring Boot, DTOs y una tabla relacional, explicando cada capa del flujo.
