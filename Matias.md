# Entrevista Simulada - Matias Alarcon

## Resumen de Evaluación

**Tema principal:**

_Espacio para que el evaluador complete._

**Nivel observado:**

_Espacio para que el evaluador complete._

**Fortalezas:**

- _Espacio para que el evaluador complete._

**Puntos a reforzar:**

- _Espacio para que el evaluador complete._

**Recomendación de estudio:**

_Espacio para que el evaluador complete._

---

## Pregunta 1

**Enunciado:**

¿Cómo protegerías una API para que solo usuarios autenticados puedan acceder a ciertos recursos?

**Respuesta del entrevistado:**

Asignar a usuarios roles los cuales manejen la autorización de recursos. Por
ejemplo, si quiero que un grupo de usuarios solo sean capaces de ver la
información de la API, pero no modificar ningún recurso, puedo asignar a este
grupo de usuarios el rol de "CLIENT".

Si en cambio quiero que otro grupo selecto de usuarios SI puedan modificar
recursos (crearlos, borrarlos, modificarlos). Entonces puedo otorgarles el rol
de "ADMIN". (y también configurar la API para que los ADMINs puedan tener los
mismos permisos que los CLIENTs, que seria ver los recursos).

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

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

**Respuesta del entrevistado:**

Primer problema seria que expone información innecesaria y a lo mejor incluso
sensible. Entonces, preguntaría por el objetivo de estas queries y a partir de
este contexto, las modificaría.

Tomemos por ejemplo la primera query:

```sql
SELECT * FROM usuarios;
```

Si se da el caso que el compañero dice: "Necesitaba una manera de ver todos los
correos electrónicos y el nombre de la persona asociada a ellos", entonces la
query puede cambiarse a:

```sql
SELECT nombre, email FROM usuarios;
```

Resultando en una query mas especifica dada la situación y el objetivo de la
misma.

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Resumen Final

_Espacio para que el evaluador complete resumen final._
