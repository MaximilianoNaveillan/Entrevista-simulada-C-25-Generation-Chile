# Entrevista Simulada - Marcos

## Resumen de Evaluación

**Tema principal:**

Arquitectura por capas en Spring Boot y optimización básica de consultas SQL.

**Nivel observado:**

En desarrollo.

**Fortalezas:**

- Reconoce que una aplicación Spring Boot se organiza en capas.
- Asocia correctamente el Repository con el acceso a base de datos.
- Muestra una base inicial para diferenciar responsabilidades técnicas, aunque todavía requiere precisión.

**Puntos a reforzar:**

- Explicar con claridad qué hace cada capa: Controller, Service y Repository.
- Diferenciar entrada/salida HTTP, lógica de negocio y persistencia de datos.
- Completar respuestas con ejemplos concretos de flujo en una API REST.
- Identificar riesgos de usar `SELECT *` cuando solo se necesitan algunas columnas.
- Proponer mejoras como selección explícita de columnas, DTOs, proyecciones y paginación.

**Diagnóstico:**

Marcos se encuentra en una etapa en desarrollo. Tiene nociones generales de arquitectura por capas y logra proponer una mejora básica frente al uso de `SELECT *`, pero todavía necesita explicar con mayor profundidad las razones técnicas detrás de sus respuestas.

**Recomendación de estudio:**

Repasar el flujo completo de una petición en Spring Boot y practicar consultas SQL enfocadas en seleccionar solo los datos necesarios.

**Plan de desarrollo sugerido:**

| Objetivo | Práctica recomendada | Resultado esperado |
| --- | --- | --- |
| Entender capas en Spring Boot | Crear un endpoint simple con Controller, Service y Repository | Puede explicar qué responsabilidad tiene cada archivo |
| Reforzar lógica de negocio | Agregar una validación en el Service antes de guardar datos | Diferencia lógica de negocio de acceso a datos |
| Mejorar SQL | Comparar `SELECT *` con consultas de columnas específicas | Identifica impacto en rendimiento y seguridad |
| Aplicar buenas prácticas | Crear un DTO para devolver solo datos necesarios | Comprende por qué no siempre se expone el modelo completo |

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
- Sería recomendable incluir un ejemplo breve usando Spring Boot, por ejemplo: un Controller recibe una solicitud para crear un usuario, el Service valida los datos y el Repository guarda la información.

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

```sql
SELECT nombre, email FROM usuarios;
```

Así las consultas son más eficientes y fáciles de mantener

**Observaciones:**

- Propone seleccionar columnas específicas, lo cual responde correctamente a una parte del problema.
- La respuesta identifica una mejora de eficiencia y mantenimiento, pero queda breve.
- Faltó mencionar riesgos como tráfico innecesario, mayor consumo de memoria y posible exposición de datos sensibles al usar `SELECT *`.
- También se esperaba mencionar DTOs, proyecciones o paginación cuando el volumen de datos lo requiera.

---

## Resumen Final

Marcos muestra una base en desarrollo: reconoce la separación por capas y propone una mejora válida para evitar `SELECT *`. Su siguiente avance debería enfocarse en explicar no solo qué haría, sino por qué esa decisión mejora rendimiento, seguridad y mantenibilidad.

**Siguiente paso sugerido:**

Construir un ejemplo pequeño de API con una entidad, un DTO, un Controller, un Service y un Repository. Luego explicar oralmente qué ocurre desde que llega una petición HTTP hasta que se consulta o guarda información en la base de datos.
