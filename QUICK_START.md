# 🚀 Inicio Rápido

## Lo que se ha hecho ✅

### Estructura
```
Curso_Computacion/
├── 📄 index.html .......................... Página web dinámica (ACTUALIZADA)
├── 📊 games-data.json .................... Base de datos de juegos (NUEVO)
├── 📖 README.md .......................... Documentación (MEJORADO)
├── 🔖 CITATION.cff ....................... Citación académica (NUEVO)
├── 🌐 .zenodo.json ....................... Metadatos Zenodo (NUEVO)
├── 📜 LICENSE ............................ CC-BY-4.0 (NUEVO)
├── 📚 ZENODO_GUIDE.md .................... Guía Zenodo (NUEVO)
├── 📝 ESTUDIANTES_INSTRUCCIONES.md ....... Guía estudiantes (NUEVO)
├── 🔧 CAMBIOS_REALIZADOS.md ............. Documentación técnica (NUEVO)
└── 🎯 QUICK_START.md .................... Este archivo (NUEVO)
```

## Próximos Pasos

### 1️⃣ Comunicar a Estudiantes
Comparte el archivo **`ESTUDIANTES_INSTRUCCIONES.md`** con ellos.
- Explica que deben actualizar su nombre en `games-data.json`
- Muéstrales donde aparecerá su crédito
- Proporciona dos opciones: GitHub o por correo

### 2️⃣ Recopilar Actualizaciones
Los estudiantes actualizan sus nombres:
```json
{
  "title": "Su Juego",
  "author": "Nombre Completo del Estudiante"  ← Cambiar aquí
}
```

### 3️⃣ Verificar en GitHub
1. Ve a: https://github.com/Marine-Data-Lab/curso_computacion
2. Abre `games-data.json`
3. Verifica que todos los nombres estén actualizados

### 4️⃣ Crear Release en GitHub
```bash
git tag -a v1.0.0 -m "Version 1.0.0 - Simuladores Educativos Completos"
git push origin v1.0.0
```

O vía GitHub Web:
1. Ve a "Releases" en tu repositorio
2. Click "Create a new release"
3. Tag: `v1.0.0`
4. Describe el lanzamiento
5. Click "Publish release"

### 5️⃣ Publicar en Zenodo
Sigue **`ZENODO_GUIDE.md`** para obtener DOI permanente

## Verificación Rápida ✓

- [x] Header mejorado con información institucional
- [x] Sistema dinámico de juegos desde JSON
- [x] Descripciones para todos los juegos
- [x] Campos de autor (esperando actualizaciones)
- [x] Página web GitHub Pages configurada
- [x] Archivos Zenodo listos
- [x] Licencia CC-BY-4.0
- [x] Documentación completa

## Archivos por Audiencia

### 👨‍🎓 Para Estudiantes
- `ESTUDIANTES_INSTRUCCIONES.md` - Cómo agregar tu nombre
- `README.md` - Información del proyecto

### 📚 Para Zenodo
- `ZENODO_GUIDE.md` - Paso a paso
- `CITATION.cff` - Archivo de cita
- `.zenodo.json` - Metadatos
- `LICENSE` - Licencia CC-BY-4.0

### 🔧 Para Técnico/Mantenedor
- `CAMBIOS_REALIZADOS.md` - Documentación detallada
- `games-data.json` - Base de datos
- `index.html` - Código fuente

## URLs Importantes

| Recurso | URL |
|---------|-----|
| Repositorio GitHub | https://github.com/Marine-Data-Lab/curso_computacion |
| Página Web | https://marine-data-lab.github.io/curso_computacion |
| Zenodo | https://zenodo.org |
| CITATION.cff | https://citation-file-format.github.io |

## Plantilla para Email a Estudiantes

```
Asunto: Actualizar tu Crédito en el Proyecto del Curso

Hola [Nombre],

Tu simulador ha sido seleccionado para el repositorio oficial del curso.
Para que tu nombre aparezca en la galería de proyectos, necesito que actualices
tu información en el archivo games-data.json.

Archivo: games-data.json
Línea a buscar: "author": "NOMBRE DEL ESTUDIANTE"
Cambiar por: "author": "[Tu Nombre Completo]"

Opciones para actualizar:
1. Vía GitHub (Recomendado): Ver ESTUDIANTES_INSTRUCCIONES.md
2. Por Correo: Responde este email con tu nombre

Tu crédito aparecerá automáticamente en:
- Página web: https://marine-data-lab.github.io/curso_computacion
- Zenodo (después de publicación)

Preguntas: Consulta ESTUDIANTES_INSTRUCCIONES.md

¡Tu trabajo merece crédito! 🎉
```

## Timeline Sugerido

```
Día 1-2:   Enviar instrucciones a estudiantes
Día 3-5:   Estudiantes actualizan nombres
Día 6:     Revisar y consolidar cambios
Día 7:     Crear Release v1.0.0 en GitHub
Día 8-10:  Publicar en Zenodo
Día 11:    Compartir DOI con estudiantes
```

## Soporte Rápido

### "¿Mi cambio no aparece en la web?"
- Espera 5 minutos para que GitHub Pages se regenere
- Limpia caché del navegador (Ctrl+F5)
- Verifica que el JSON esté válido

### "¿Cómo cito el trabajo ahora?"
Usa el formato en `CITATION.cff` o espera a DOI de Zenodo

### "¿Se puede agregar un nuevo juego?"
Sí, solo agrega una entrada en `games-data.json`:
```json
{
  "id": 18,
  "title": "Nuevo Juego",
  "program": "...",
  "author": "...",
  "description": "...",
  "htmlFile": "...",
  "keywords": [...]
}
```

---

**¡Listo! El proyecto está completamente preparado. Espera a que los estudiantes actualicen sus nombres y luego publica en Zenodo.** 🚀
