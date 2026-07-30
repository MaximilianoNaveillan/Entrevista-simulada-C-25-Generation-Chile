# Entrevista Simulada - Elvis Bracho

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

¿Cuál es la diferencia entre Props y State?

**Respuesta del entrevistado:**

la diferencia entre props y state:
props: son los datos que un componente padre le pasa a un componente hijo para decirle cómo debe configurarse o renderizarse.

state:es la memoria interna de un componente. Sirve para guardar datos que cambian con el tiempo a causa de la interacción del usuario, peticiones a un servidor o temporizadores.

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Pregunta 2

**Enunciado:**

```java
/* ¿Qué hace este código? */
public static boolean Ejercicio(String texto){
    // Normalizar el texto: eliminar espacios y convertir minusculas
    texto = texto.replaceAll("\\s+", "").toLowerCase();
    int izquierda = 0;
    int derecha = texto.length() -1;
    while(izquierda < derecha){
        if(texto.charAt(izquierda) != texto.charAt(derecha)){
            return false;
        }
        izquierda++;
        derecha--;
    }
    return true
}
```

**Respuesta del entrevistado:**

lo que hace el codigo es un transformador de palabras en paliodromos por ejemplo cambia una palabra y la coloca al reves ej: palabra arbalap
y tambien elimina los espacios del texto y los convierte en minusculas

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Resumen Final

_Espacio para que el evaluador complete resumen final._
