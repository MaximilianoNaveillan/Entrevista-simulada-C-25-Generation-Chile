# Entrevista Simulada - Pablo Davila

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

¿Cuál es la diferencia entre sobrecarga (Overload) y sobrescritura (Override)?

**Respuesta del entrevistado:**

_Espacio para que el entrevistado complete su respuesta._

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Pregunta 2

**Enunciado:**

```java
@RestController
@RequestMapping("/productos")
public class ProductoController(
    private final ProductoService servicio;
    public ProductoController(ProductoService servicio){
        this.servicio = servicio
    }

    @GetMapping("/{id}")
    public ResponseEntity<Producto> obtenerProducto(@PathVariable Long id){
        Producto producto = servicio.obtenerPorId(id);
        if(producto != null){
            return ResponseEntity.ok(producto);
        } else {
            return ResponseEntity.notFound().build();
        }
    }
)
```

¿Qué hace este controlador?

¿Qué ocurre si el producto no se encuentra?

¿Cómo se maneja la inyección de dependencias aquí?

**Respuesta del entrevistado:**

_Espacio para que el entrevistado complete su respuesta._

**Observaciones del evaluador:**

- _Espacio para que el evaluador complete observaciones._

---

## Resumen Final

_Espacio para que el evaluador complete resumen final._
