# Entrevistas Simuladas - Cohorte 25 Java

Repositorio de evaluación y seguimiento para entrevistas simuladas de la cohorte 25 Java del bootcamp Generation.

Este documento funciona como índice principal, guía de formato, rúbrica de evaluación y recurso de preparación para entrevistas técnicas.

---

## Entrevistas Disponibles

| Candidato | Temas principales                    | Nivel observado | Archivo                        |
| --------- | ------------------------------------ | --------------- | ------------------------------ |
| Benjamin  | JPA, DTO, SQL                        | Inicial         | [Benjamin.md](./Benjamin.md)   |
| Engelbert | DOM, JavaScript, eventos             | Inicial         | [Engelbert.md](./Engelbert.md) |
| Gustavo   | React Router, CSS, responsive design | En desarrollo   | [Gustavo.md](./Gustavo.md)     |
| Juan      | POO, HTML, CSS                       | En desarrollo   | [Juan.md](./Juan.md)           |
| Marcos    | Spring Boot por capas, SQL           | En desarrollo   | [Marcos.md](./Marcos.md)       |

---

## Formato Estándar de Entrevista

Cada entrevista debe conservar la respuesta original del candidato y separar claramente la evaluación técnica.

```md
# Entrevista Simulada - Nombre

## Resumen de Evaluación

**Tema principal:**

Tema evaluado durante la entrevista.

**Nivel observado:**

Inicial / En desarrollo / Adecuado.

**Fortalezas:**

- Aspectos positivos detectados.

**Puntos a reforzar:**

- Conceptos o habilidades que requieren práctica.

**Recomendación de estudio:**

Recurso o enfoque sugerido para mejorar.

---

## Pregunta 1

**Enunciado:**

Pregunta realizada al candidato.

**Respuesta del candidato:**

Respuesta entregada durante la entrevista.

**Observaciones:**

- Retroalimentación técnica.

---

## Resumen Final

Síntesis del desempeño y siguiente paso sugerido.
```

---

## Criterios para Observaciones

- Indicar si la respuesta responde directamente al enunciado.
- Registrar fortalezas técnicas cuando existan.
- Mencionar conceptos que debe reforzar el candidato.
- Señalar errores relevantes de sintaxis, lógica o definición.
- Mantener intacta la respuesta original del candidato.
- Evitar convertir la observación en una corrección completa del ejercicio.
- Redactar comentarios claros, breves y accionables.

---

## Rúbrica Sugerida

| Nivel         | Descripción                                                                              |
| ------------- | ---------------------------------------------------------------------------------------- |
| Inicial       | Reconoce algunos conceptos, pero responde de forma incompleta o con errores importantes. |
| En desarrollo | Identifica la idea principal, pero necesita más precisión, ejemplos o práctica técnica.  |
| Adecuado      | Responde con claridad, usa vocabulario técnico correcto y entrega ejemplos funcionales.  |
| Sólido        | Explica con profundidad, conecta conceptos y justifica buenas prácticas.                 |

---

## Tips para Entrevistas Técnicas

### Antes de la entrevista

- Repasar Java, programación orientada a objetos, Spring Boot, JPA, SQL, HTML, CSS, JavaScript y React.
- Preparar ejemplos simples para explicar conceptos técnicos.
- Practicar respuestas en voz alta usando frases claras y directas.
- Revisar proyectos personales o del bootcamp para poder explicar decisiones técnicas.
- Aceptar que es mejor reconocer una duda y razonar que inventar una explicación incorrecta.

### Durante la entrevista

- Escuchar completa la pregunta antes de responder.
- Pedir una aclaración breve si el enunciado no queda claro.
- Responder primero la idea principal y luego agregar un ejemplo.
- Pensar en voz alta cuando se resuelva un ejercicio técnico.
- Explicar el enfoque aunque no se tenga la respuesta completa.
- Usar vocabulario técnico sin complicar innecesariamente la explicación.

### Estructura recomendada para responder

1. Definir brevemente el concepto.
2. Explicar para qué sirve o cuándo se usa.
3. Dar un ejemplo simple.
4. Mencionar una buena práctica, riesgo o comparación si aplica.

Ejemplo:

```text
Un Service en Spring Boot contiene la lógica de negocio de la aplicación.
Se usa para separar las reglas del sistema del Controller y del Repository.
Por ejemplo, antes de guardar una venta, el Service podría validar stock, calcular totales y luego llamar al Repository.
```

---

## Tips por Tema

### Java

- Reforzar encapsulación, herencia, polimorfismo y abstracción.
- Practicar diferencias entre clase, objeto, atributo, método, constructor e interfaz.
- Entender modificadores de acceso: `public`, `private`, `protected` y acceso por defecto.
- Repasar colecciones comunes: `List`, `Set`, `Map` y sus casos de uso.
- Practicar lectura de errores y excepciones comunes.

### Spring Boot

- Entender la separación por capas: Controller, Service y Repository.
- Diferenciar `@RestController`, `@Service`, `@Repository` y `@Entity`.
- Practicar endpoints básicos con `GET`, `POST`, `PUT` y `DELETE`.
- Comprender inyección de dependencias y uso de constructores.
- Explicar el flujo de una petición desde el frontend hasta la base de datos.

### JPA y Bases de Datos

- Entender que JPA es una especificación para mapear entidades Java a tablas relacionales.
- Diferenciar entidad, tabla, columna, clave primaria y relación.
- Reforzar `@OneToMany`, `@ManyToOne`, `@OneToOne` y `@ManyToMany`.
- Usar DTOs cuando no conviene exponer entidades directamente al frontend.
- Comprender riesgos como acoplamiento, fuga de datos y problemas de serialización.

### SQL

- Practicar `CREATE DATABASE`, `CREATE TABLE`, `INSERT`, `SELECT`, `UPDATE` y `DELETE`.
- Usar `WHERE` para filtrar datos.
- Usar funciones como `COUNT`, `AVG`, `SUM`, `MIN` y `MAX`.
- Evitar `SELECT *` cuando solo se necesitan algunas columnas.
- Repasar tipos de datos comunes: `INT`, `VARCHAR`, `DECIMAL`, `DATE` y `BOOLEAN`.

### HTML, CSS y JavaScript

- Dominar la estructura básica de HTML: `html`, `head`, `title` y `body`.
- Usar etiquetas semánticas cuando corresponda: `header`, `main`, `section` y `footer`.
- Reforzar CSS básico: selectores, clases, ids, colores, espaciados y bordes.
- Practicar Flexbox y Grid para layout.
- Entender el DOM como representación del HTML en forma de árbol.
- Practicar eventos con `addEventListener` y manipulación de contenido con `textContent`.

### React

- Diferenciar componente, props, estado y eventos.
- Practicar `useState` y renderizado condicional.
- Entender `useEffect` para efectos secundarios.
- Diferenciar `Link` de `useNavigate()` en React Router.
- Reforzar comunicación con APIs usando `fetch` o `axios`.

---

## Errores Comunes

- Responder solo con definiciones memorizadas sin ejemplo.
- Confundir responsabilidades entre Controller, Service y Repository.
- No cerrar correctamente etiquetas HTML.
- No explicar qué hace una media query o un selector CSS.
- Usar `SELECT *` sin justificarlo.
- No diferenciar entidad JPA de DTO.
- Quedarse en silencio cuando no se sabe una respuesta.
- No leer cuidadosamente el enunciado de ejercicios prácticos.

---

## Documentación Oficial

- Java: https://docs.oracle.com/en/java/
- Java Tutorials: https://dev.java/learn/
- Spring Boot: https://spring.io/projects/spring-boot
- Spring Guides: https://spring.io/guides
- Spring Data JPA: https://spring.io/projects/spring-data-jpa
- Hibernate ORM: https://hibernate.org/orm/documentation/
- MDN Web Docs: https://developer.mozilla.org/
- HTML en MDN: https://developer.mozilla.org/en-US/docs/Web/HTML
- CSS en MDN: https://developer.mozilla.org/en-US/docs/Web/CSS
- JavaScript en MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript
- React: https://react.dev/
- React Router: https://reactrouter.com/
- PostgreSQL: https://www.postgresql.org/docs/
- MySQL: https://dev.mysql.com/doc/

---

## Repositorios de Estudio

- Spring Guides: https://github.com/spring-guides
- Spring PetClinic: https://github.com/spring-projects/spring-petclinic
- The Algorithms Java: https://github.com/TheAlgorithms/Java
- freeCodeCamp: https://github.com/freeCodeCamp/freeCodeCamp
- Developer Roadmap: https://github.com/kamranahmedse/developer-roadmap
- Awesome Java: https://github.com/akullpp/awesome-java
- Awesome Spring Boot: https://github.com/ityouknow/awesome-spring-boot

---

## Checklist Final para Candidatos

- Puedo explicar POO con ejemplos simples.
- Puedo describir el flujo Controller, Service y Repository.
- Puedo crear una entidad JPA básica.
- Puedo explicar por qué usar DTOs.
- Puedo escribir consultas SQL simples con filtros y agregaciones.
- Puedo crear una página HTML básica con estilos.
- Puedo manipular el DOM con JavaScript.
- Puedo explicar componentes, estado y rutas en React.
- Puedo hablar de un proyecto propio y justificar decisiones técnicas.
- Puedo reconocer cuando no sé algo y explicar cómo lo investigaría.
