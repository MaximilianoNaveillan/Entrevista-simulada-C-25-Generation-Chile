# Guía para Candidatos

Esta guía explica cómo completar tus respuestas, guardar los cambios y subirlos a la rama `main`.

---

## 1. Actualizar el repositorio

Antes de modificar tu archivo, asegúrate de tener la última versión del repositorio:

```bash
git pull origin main
```

---

## 2. Abrir tu archivo

Busca el archivo Markdown con tu nombre.

Ejemplos:

- `Luis.md`
- `Catalina.md`
- `Christian.md`
- `Pablo.md`
- `Maria.md`
- `Elvis.md`
- `Matias.md`
- `Claudio.md`

---

## 3. Completar tus respuestas

Dentro de tu archivo encontrarás secciones como esta:

````md
**Respuesta del entrevistado:**

_Espacio para que el entrevistado complete su respuesta._
````

Reemplaza `_Espacio para que el entrevistado complete su respuesta._` por tu respuesta.

Ejemplo:

````md
**Respuesta del entrevistado:**

La autenticación verifica quién es el usuario. La autorización define qué permisos tiene ese usuario dentro del sistema.
````

No borres el enunciado de la pregunta ni las secciones del documento.

---

## 4. Guardar el archivo

Después de completar tus respuestas, guarda el archivo.

---

## 5. Revisar los cambios

Ejecuta:

```bash
git status
```

Deberías ver tu archivo como modificado.

También puedes revisar qué cambiaste con:

```bash
git diff
```

---

## 6. Agregar tu archivo al commit

Agrega solo tu archivo.

```bash
git add NombreDelArchivo.md
```

Ejemplo:

```bash
git add Luis.md
```

---

## 7. Crear el commit

Crea un commit con un mensaje claro.

```bash
git commit -m "Agrega respuestas de Luis"
```

Cambia el nombre según corresponda.

Ejemplos:

```bash
git commit -m "Agrega respuestas de Catalina"
git commit -m "Agrega respuestas de Pablo"
```

---

## 8. Subir los cambios a main

Sube tus cambios a la rama `main`.

```bash
git push origin main
```

---

## 9. Verificar el resultado

Después del push, revisa el repositorio remoto y confirma que tu archivo quedó actualizado con tus respuestas.

---

## Recomendaciones

- Modifica solo el archivo que corresponde a tu nombre.
- Responde debajo de cada sección `Respuesta del entrevistado`.
- No borres los enunciados de las preguntas.
- No modifiques respuestas de otros candidatos.
- Escribe respuestas claras y completas.
- Si `git push origin main` falla, ejecuta `git pull origin main`, resuelve cualquier conflicto si aparece y vuelve a intentar el push.
- Si tienes dudas con Git, pide ayuda antes de subir cambios.
