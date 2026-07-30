# Entrevista Simulada - Christian Lorca

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

¿Qué es el DOM y cómo JavaScript interactua con él?

**Respuesta del entrevistado:**

_Espacio para que el entrevistado complete su respuesta._

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Pregunta 2

**Enunciado:**

Diseña un formulario sencillo con los siguientes campos:

- Nombre, input de texto.
- Correo electrónico, input de email.
- Mensaje, textarea.
- Botón de enviar.

Requisitos:

- HTML: estructura semántica con etiquetas adecuadas.
- CSS: estilos básicos.
- JavaScript: mostrar un `alert("¡Enviado con éxito!")` al presionar el botón.

**Respuesta del entrevistado:**

```html
<head>
    <style>

        body {
        display: flex;
        }

        .formulario {
            max-width: 400px;
        }
    </style>
</head>
<body>
<form id="contactoForm" class="formulario">
    <div class="campo">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required>
    </div>

        <div class="campo">
        <label for="correo">Correo:</label>
        <input type="email" id="correo" name="correo" required>
    </div>

        <div class="campo">
        <label for="mensaje">Mensaje:</label>
        <textarea id="mensaje" name="mensaje" required></textarea>
    </div>

    <button type="submit">Enviar
    </button>

</form>

<script>
    const formulario = document.getElementById('contactoForm');

    formulario.addEventListener('submit', function(evento) {
        evento.preventDefault();
        alert("¡Enviado con éxito!");
    })
</script>

</body>

```


**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Resumen Final

_Espacio para que el evaluador complete resumen final._
