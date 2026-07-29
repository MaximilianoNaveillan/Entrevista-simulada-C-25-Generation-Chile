# Entrevista Simulada - Gustavo

## Resumen de Evaluación

**Tema principal:**

React Router, CSS, Flexbox, Grid y responsive design.

**Nivel observado:**

En desarrollo.

**Fortalezas:**

- Reconoce `useNavigate()` como un hook.
- Identifica parcialmente conceptos visuales relacionados con CSS.
- Tiene base para avanzar en navegación y estilos si profundiza los casos de uso.

**Puntos a reforzar:**

- Diferencia entre navegación programática y navegación declarativa en React Router.
- Explicación de Flexbox, Grid, selectores descendientes y media queries.
- Lectura precisa de código CSS y comportamiento responsive.

**Recomendación de estudio:**

Practicar una aplicación React con varias rutas usando `Link` y `useNavigate()`, junto con un layout responsive que combine Flexbox, Grid y media queries.

---

## Pregunta 1

**Enunciado:**

¿Cuándo utilizarías `useNavigate()` y cuándo un componente `Link`?

**Respuesta del candidato:**

No registrada.

**Observaciones:**

- Identifica `useNavigate()` como un hook, pero no explica con precisión su uso.
- No identifica correctamente el componente `Link` ni su propósito en navegación declarativa.
- Debe diferenciar navegación programática con `useNavigate()` frente a navegación mediante enlaces renderizados con `Link`.
- Reforzar casos de uso: redirecciones después de acciones, botones, rutas protegidas y navegación entre vistas.

---

## Pregunta 2

**Enunciado:**

Analiza cada uno de los 5 puntos marcados en el siguiente código CSS y explica, de la forma más breve posible, qué hace cada uno.

```html
<style>

    .navbar {
        display: flex;
        /* Punto 1*/
        justify-content: space-between;
        align-items: center;
        padding: 10px 20px;
        background-color: #333;
        color: #fff;
    }

    .section-grid {
        display: grid;
        /*Punto 2*/
        grid-template-columns: repeat(3, 1fr);
        /*Punto 3*/
        gap: 20px;
        padding: 20px;
    }

    /* Elementos dentro de la sección */
    .section-grid div {
        background-color: #ddd;
        padding: 20px;
        text-align: center;
        border-radius: 5px;
    }

    @media (max-width: 480px) {

        /* Punto 4*/
        .navbar {
            flex-direction: column;
            align-items: flex-start;
        }

        .section-grid {
            grid-template-columns: 1fr;
            /* Punto 5*/
        }
    }
</style>
```

**Respuesta del candidato:**

No registrada.

**Observaciones:**

- Falta profundizar el comportamiento de grilla en display grid.
- No identifica selector de descendientes.
- No identifica media query.
- No identifica formato de color hexadecimal.
- Debe reforzar conceptos de Flexbox como distribución en el eje principal y alineación en el eje cruzado.
- Debe explicar que `grid-template-columns: repeat(3, 1fr)` crea tres columnas de igual tamaño.
- Debe identificar que `gap` define separación entre elementos de la grilla.
- Debe reconocer que la media query adapta el diseño para pantallas pequeñas.

---

## Resumen Final

Gustavo muestra señales de conocimiento inicial en React Router y CSS, pero necesita explicar con mayor precisión los conceptos. El siguiente paso sugerido es practicar navegación entre vistas en React y describir línea por línea un layout responsive simple.
