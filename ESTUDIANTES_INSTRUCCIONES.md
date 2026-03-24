# Instrucciones para Estudiantes: Actualizar tu Crédito

¡Hola! Tu juego ha sido seleccionado para formar parte del repositorio oficial del Curso de Programación y Computación de UABCS. Esta guía te ayudará a actualizar tu nombre en la galería de proyectos.

## 📝 ¿Por qué actualizar tu nombre?

El archivo `games-data.json` mantiene un registro oficial de todos los autores de los simuladores. Tu actualización:
- ✅ Te da crédito público por tu trabajo
- ✅ Facilita la citación académica
- ✅ Aparecerá en la página web oficial
- ✅ Se incluirá en futuras publicaciones (Zenodo, etc.)

## 🔍 Ubicar tu Juego

1. Abre el archivo `games-data.json` en la raíz del repositorio
2. Busca el título de tu juego
3. Busca la línea que dice `"author": "NOMBRE DEL ESTUDIANTE"`

**Ejemplo:**
```json
{
  "id": 5,
  "title": "Pesquería UABCS",
  "program": "Ingeniería en Pesquerías",
  "author": "NOMBRE DEL ESTUDIANTE",  ← ¡AQUÍ!
  ...
}
```

## ✏️ Cómo Actualizar

### Opción 1: Directamente en GitHub (Recomendado)

1. Ve a: https://github.com/Marine-Data-Lab/curso_computacion
2. Abre el archivo `games-data.json`
3. Haz clic en el lápiz (✏️) para editar
4. Encuentra tu juego y reemplaza:
   - `"NOMBRE DEL ESTUDIANTE"` → `"Tu Nombre Completo"`
5. Desplázate hasta abajo y:
   - Selecciona "Create a new branch for this commit"
   - Haz clic en "Propose changes"
6. Haz clic en "Create pull request"
7. Agrega una descripción simple: "Actualizar crédito: [Tu Nombre]"
8. Haz clic en "Create pull request"

### Opción 2: Por Correo

1. Envía un correo al Dr. Ricardo Cavieses Núñez con:
   - **Asunto**: "Actualizar crédito - [Tu Nombre]"
   - **Contenido**:
     ```
     Solicito actualizar mi nombre en el juego: [Título del Juego]

     Nombre completo: [Tu Nombre]
     Grupo: [Tu Grupo/Sección]
     ```

## 📌 Formato Correcto

Por favor, usa:
- Tu nombre completo y real
- Mayúsculas normales (no TODO EN MAYÚSCULAS)
- Tu nombre como prefieres ser acreditado

**Ejemplos correctos:**
- `"Juan García López"`
- `"María de la Cruz"`
- `"Pedro J. Martínez Ruiz"`

**Ejemplos incorrectos:**
- `"JUAN GARCIA LOPEZ"` (todo mayúsculas)
- `"JGL"` (abreviado)
- `"estudiante"` (genérico)

## ✅ Validación

Después de actualizar, tu nombre:
1. Aparecerá en `games-data.json`
2. Se mostrará en la página web: https://marine-data-lab.github.io/curso_computacion
3. Se incluirá en futuras publicaciones de Zenodo

## 🎖️ Citación

Una vez actualizado tu nombre, tu trabajo podrá ser citado así:

**Formato BibTeX:**
```bibtex
@software{lastname_2026,
  title = {[Título de tu Juego]},
  author = {Tu Nombre Completo},
  year = {2026},
  url = {https://github.com/Marine-Data-Lab/curso_computacion}
}
```

**Formato APA:**
```
Tu Nombre Completo. (2026). [Título de tu Juego]. En Curso de Programación y Computación - UABCS. https://github.com/Marine-Data-Lab/curso_computacion
```

## ❓ Preguntas Frecuentes

### ¿Es obligatorio actualizar mi nombre?
No es obligatorio, pero se recomienda. Es tu crédito académico.

### ¿Puedo cambiar el título del juego?
El título del juego **no** debe cambiar. Si necesitas cambiar algo en tu proyecto, contacta al instructor.

### ¿Qué pasa después?
Tu trabajo forma parte de un proyecto educativo que será:
- Usado por otros estudiantes para aprender
- Potencialmente publicado en Zenodo (repositorio académico)
- Citado en trabajos futuros

### ¿Hay algún costo?
No. Todo es completamente gratuito. El repositorio usa Licencia Creative Commons.

### ¿Puedo ver mi actualización inmediatamente?
- En GitHub: sí, inmediatamente después del merge
- En la página web: en la próxima actualización (dentro de minutos)

## 📞 Contacto

Si tienes problemas:
1. Revisa esta guía de nuevo
2. Pregunta a un compañero
3. Contacta al Dr. Ricardo Cavieses Núñez

---

**¡Gracias por tu contribución al curso!** 🎉

Tu simulador ayudará a futuros estudiantes a aprender programación de una manera práctica y divertida.
