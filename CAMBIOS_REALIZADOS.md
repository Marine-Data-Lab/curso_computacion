# Cambios Realizados - Preparación para Zenodo

Este documento resume todos los cambios realizados para mejorar el repositorio y prepararlo para publicación en Zenodo.

## 📋 Archivos Creados

### 1. **games-data.json** ✨
- **Propósito**: Base de datos estructurada de todos los juegos
- **Contenido**: 17 juegos con:
  - Título y descripción
  - Programa (Pesquerías / Desastres)
  - Nombre del estudiante autor (placeholders por ahora)
  - Archivo HTML asociado
  - Palabras clave
- **Uso**: JavaScript carga dinámicamente este archivo para renderizar la página

### 2. **CITATION.cff**
- **Estándar**: Citation File Format v1.2.0
- **Contenido**: Metadatos de citación del proyecto
- **Beneficio**: Permite que GitHub y otros servicios muestren cómo citar el trabajo
- **Información**:
  - Autor principal: Dr. Ricardo Cavieses Núñez
  - Licencia: CC-BY-4.0
  - Versión: 1.0.0

### 3. **.zenodo.json**
- **Formato**: JSON personalizado para Zenodo
- **Contenido**: Metadatos completos para publicación
- **Incluye**:
  - Descripción detallada
  - Palabras clave académicas
  - Información de contribuyentes
  - Licencia y relaciones
  - Esquemas de clasificación (LCSH)

### 4. **LICENSE**
- **Tipo**: Creative Commons Attribution 4.0 (CC-BY-4.0)
- **Contenido**: Texto legal completo
- **Permisos**: Uso comercial, modificación, distribución
- **Obligación**: Dar crédito al autor original

### 5. **ZENODO_GUIDE.md**
- **Propósito**: Guía paso a paso para publicar en Zenodo
- **Incluye**:
  - Instrucciones detalladas
  - Ventajas de publicar en Zenodo
  - Cómo obtener DOI
  - Formatos de citación
  - Integración con GitHub

### 6. **ESTUDIANTES_INSTRUCCIONES.md**
- **Destinatarios**: Estudiantes autores de juegos
- **Contenido**:
  - Cómo actualizar su nombre en games-data.json
  - Instrucciones paso a paso (GitHub y por correo)
  - Formatos correctos de nombres
  - Información sobre citación académica
  - FAQ

### 7. **.gitignore**
- **Propósito**: Especificar qué archivos no se deben versionar
- **Incluye**: Configuraciones comunes para IDEs, lenguajes, caché, etc.

## 📝 Archivos Modificados

### 1. **index.html**
#### Cambios de Contenido:
- ✅ Agregado "Universidad Autónoma de Baja California Sur"
- ✅ Agregado "Departamento Académico de Ingeniería en Pesquerías"
- ✅ Agregado "Dr. Ricardo Cavieses Núñez"
- ✅ Agregado párrafo descriptivo sobre sistemas de simulación

#### Cambios de Estructura:
- ✅ Convertido de contenido estático a dinámico
- ✅ Contenedor `#programs-container` reemplaza listas HTML hardcodeadas
- ✅ Script JavaScript carga datos desde `games-data.json`

#### Cambios de Estilos CSS:
- ✅ Agregadas clases `.institution-info`, `.department`, `.instructor`
- ✅ Agregada clase `.description` con fondo semi-transparente
- ✅ Mejorado `.game-item` para mostrar:
  - Descripción del juego
  - Nombre del autor
  - Mejor estructura visual
- ✅ Agregada clase `.game-meta` para información del autor
- ✅ Agregada clase `.game-description` para descripción del juego

#### Cambios JavaScript:
- ✅ Función `loadGamesData()` carga JSON de forma asincrónica
- ✅ Función `renderPrograms()` agrupa juegos por programa
- ✅ Función `createProgramSection()` genera secciones HTML dinámicas
- ✅ Renderizado automático al cargar el DOM

### 2. **README.md**
#### Mejoras:
- ✅ Información rápida en la parte superior
- ✅ Tabla de contenido mejorada con iconos y descripción
- ✅ Información de autores y cómo actualizar nombres
- ✅ Instrucciones de uso mejoradas (3 opciones)
- ✅ Tabla de tecnologías
- ✅ Tabla de información institucional
- ✅ Información sobre Zenodo
- ✅ Estadísticas del proyecto
- ✅ Enlaces útiles y repositorio

## 🎨 Mejoras Visuales y de Funcionamiento

### Página Web Dinámica
- **Antes**: 17 elementos HTML codificados manualmente
- **Después**: Generados dinámicamente desde JSON
- **Beneficio**: Cambios únicos actualizan automáticamente toda la página

### Información de Autores
- **Antes**: No había autores mostrados
- **Después**: Cada juego muestra nombre del estudiante autor
- **Estructura**: Fácil de actualizar mediante `games-data.json`

### Descripciones de Juegos
- **Antes**: Solo títulos en la página web
- **Después**: Descripción completa de cada juego
- **Mejora**: Los usuarios saben qué esperar antes de abrir un juego

### Responsive y Mejorado
- ✅ Las tarjetas de juegos ahora incluyen más información
- ✅ Mejor layout visual con descripción y autor
- ✅ Hover effects mejorados
- ✅ Información clara y estructurada

## 📊 Estructura de Datos

### games-data.json (Ejemplo)
```json
{
  "id": 1,
  "title": "Gestiona tu Empresa",
  "program": "Ingeniería en Pesquerías",
  "author": "NOMBRE DEL ESTUDIANTE",
  "description": "Simulador de gestión empresarial donde los jugadores...",
  "htmlFile": "ingeniería en pesquerías/juegos/gestiona_tu_empresa.html",
  "keywords": ["gestión", "empresa", "pesca"]
}
```

## 🔄 Flujo de Actualización

1. **Estudiante actualiza su nombre** en `games-data.json`
2. **Hace un Pull Request** o contacta al instructor
3. **Se aprueba el cambio**
4. **GitHub Pages se regenera automáticamente**
5. **Nombre aparece en la página web** dentro de minutos

## 🌐 GitHub Pages

Para habilitar GitHub Pages:
1. Ve a Settings → Pages
2. Source: Deploy from a branch
3. Branch: main
4. Folder: / (root)
5. Click Save

La página estará disponible en: `https://marine-data-lab.github.io/curso_computacion`

## 📦 Preparación para Zenodo

El repositorio ahora incluye:
- ✅ CITATION.cff para citación automática
- ✅ .zenodo.json con metadatos completos
- ✅ LICENSE con CC-BY-4.0 oficial
- ✅ README con información académica
- ✅ Estructura clara y documentada

### Siguientes Pasos (Cuando estudiantes actualicen nombres):
1. Actualizar CITATION.cff con contribuyentes
2. Hacer Release en GitHub (v1.0.0)
3. Conectar GitHub a Zenodo
4. Publicar en Zenodo con DOI

## 📈 Beneficios

| Aspecto | Beneficio |
|---------|-----------|
| **Dinámico** | Cambios centralizados en JSON |
| **Mantenible** | Fácil agregar/modificar juegos |
| **Académico** | Preparado para publicación formal |
| **Citables** | Metadatos listos para Zenodo |
| **Accesible** | Página web interactiva |
| **Documentado** | Guías claras para estudiantes |

## 🔐 Ventajas de la Nueva Estructura

1. **Separación de contenido y presentación**
   - Datos en JSON, renderizado en JavaScript
   - Cambios sin tocar HTML

2. **Escalabilidad**
   - Agregar nuevos juegos es trivial
   - Solo agregar entrada en JSON

3. **Mantenibilidad**
   - Cambios únicos para autores
   - No duplicación de información

4. **Automatización**
   - Actualizaciones automáticas al cargar
   - Consistencia garantizada

## ✅ Checklist de Completitud

- [x] Header mejorado con información institucional
- [x] Sistema dinámico de juegos desde JSON
- [x] Descripciones de todos los juegos
- [x] Información de autores (placeholders)
- [x] Archivo CITATION.cff
- [x] Metadatos Zenodo
- [x] Licencia CC-BY-4.0
- [x] Guía de Zenodo
- [x] Instrucciones para estudiantes
- [x] README mejorado
- [x] .gitignore
- [x] Página web GitHub Pages lista

## 📞 Soporte

Para preguntas o problemas:
1. Consulta ZENODO_GUIDE.md para publicación
2. Consulta ESTUDIANTES_INSTRUCCIONES.md para actualizar nombres
3. Contacta al Dr. Ricardo Cavieses Núñez

---

**Estado**: ✅ Listo para que estudiantes actualicen sus nombres
**Siguiente**: Cuando estudiantes actualicen → Publicar en Zenodo
**Fecha de cambios**: Marzo 20, 2026
