# Entrevista Simulada - Marcos

## Resumen de Evaluación

**Tema principal:**

Arquitectura por capas en Spring Boot y buenas prácticas SQL.

**Nivel observado:**

Inicial.

**Fortalezas:**

- Reconoce de forma general las capas Controller, Service y Repository.
- Identifica que Repository está relacionado con el acceso a base de datos.

**Puntos a reforzar:**

- Responsabilidades específicas de cada capa en Spring Boot.
- Diferencia entre lógica de negocio, controladores y persistencia.
- Riesgos de usar `SELECT *` cuando solo se necesitan algunas columnas.
- Uso de DTOs, proyecciones y paginación cuando corresponde.

**Recomendación de estudio:**

Repasar el flujo de una petición en Spring Boot y practicar consultas SQL enfocadas en seleccionar solo los datos necesarios.

---

## Pregunta 1

**Enunciado:**

¿Cuál es la responsabilidad de un Controller, Service y Repository?

**Respuesta del candidato:**

Controller: Recibe las solicitudes .

Service: Contiene la lógica de .

Repository: Accede a la base de datos y realizando consultas .

**Observaciones:**

- Reconoce de forma general la separación por capas, pero la explicación queda incompleta.
- Debe reforzar que el Controller recibe peticiones HTTP y coordina la entrada/salida.
- Debe precisar que el Service contiene la lógica de negocio y que el Repository encapsula el acceso a datos.
- Sería recomendable incluir un ejemplo breve usando Spring Boot.

---

## Pregunta 2

**Enunciado:**

Estás trabajando en un proyecto grande y notas que un compañero crea varias consultas a la base de datos así:

```sql
SELECT * FROM usuarios;
SELECT * FROM productos;
SELECT * FROM ventas;
```

Lo hace incluso cuando solo necesita un par de columnas para mostrar datos en pantalla.

¿Qué problemas podría generar esta práctica y qué le sugerirías para mejorarla?

**Respuesta del candidato:**

No registrada.

**Observaciones:**

- No se registra respuesta del candidato.
- La respuesta esperada debía identificar problemas de rendimiento, tráfico innecesario y posible exposición de datos sensibles al usar `SELECT *`.
- Se esperaba sugerir seleccionar solo las columnas necesarias, usar DTOs o proyecciones y revisar paginación cuando aplique.

---

## Resumen Final

Marcos tiene una base inicial sobre separación por capas, pero necesita completar las definiciones y asociarlas a ejemplos reales. El siguiente paso sugerido es explicar un endpoint completo desde Controller hasta Repository y comparar consultas con `SELECT *` frente a consultas con columnas específicas.
