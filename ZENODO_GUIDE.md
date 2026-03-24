# Guía para Publicar en Zenodo

Este documento contiene instrucciones para compartir este repositorio en Zenodo, un repositorio de acceso abierto que proporciona DOI (Digital Object Identifier) para citar tu trabajo.

## Archivos de Configuración

El repositorio incluye los siguientes archivos preparados para Zenodo:

- **`.zenodo.json`**: Metadatos del proyecto en formato JSON para Zenodo
- **`CITATION.cff`**: Archivo de cita en formato Citation File Format (CFF)
- **`games-data.json`**: Datos estructurados de todos los juegos con información de autores

## Pasos para Publicar en Zenodo

### 1. Preparación Inicial

#### a. Actualizar información de autores

Edita el archivo **`games-data.json`** y reemplaza "NOMBRE DEL ESTUDIANTE" con los nombres reales de los estudiantes que crearon cada juego:

```json
{
  "title": "Nombre del Juego",
  "author": "Nombre del Estudiante Real"
}
```

#### b. Completar metadatos de Zenodo

Edita **`.zenodo.json`** si necesitas agregar información adicional:
- ORCID del instructor (si lo tienes)
- Información detallada de contribuyentes
- Identificadores adicionales

### 2. En GitHub

1. Asegúrate de que todo el código esté en GitHub: https://github.com/Marine-Data-Lab/curso_computacion
2. Haz un **Release** en GitHub:
   - Ve a "Releases" en el repositorio
   - Haz clic en "Create a new release"
   - Etiqueta como `v1.0.0` (o la versión que corresponda)
   - Describe brevemente el contenido

### 3. En Zenodo

1. **Crea una cuenta en Zenodo** (si no la tienes):
   - Visita https://zenodo.org
   - Haz clic en "Sign up"
   - Completa el registro

2. **Conecta tu cuenta de GitHub** (para integración automática):
   - Ve a https://zenodo.org/account/settings/github
   - Selecciona "Marine-Data-Lab/curso_computacion"
   - Activa el toggle para habilitar publicación automática

3. **Publicar manualmente** (alternativa):
   - Visita https://zenodo.org/deposit/new
   - Carga los archivos del repositorio
   - Completa los campos de metadatos:
     - **Title**: "Curso de Programación y Computación - Simuladores Educativos"
     - **Description**: Copia del campo en `.zenodo.json`
     - **License**: Selecciona "Creative Commons Attribution 4.0"
     - **Upload Type**: "Software"
     - **Keywords**: Agregar los listados en `.zenodo.json`
   - Haz clic en "Publish"

## Información Importante

### Licencia

El proyecto utiliza **Creative Commons Attribution 4.0 (CC-BY-4.0)**, que permite:
- ✅ Usar comercialmente
- ✅ Modificar
- ✅ Distribuir
- ✅ Usar privadamente

Con la condición de que den crédito al autor original.

### Citación

Una vez publicado en Zenodo, los usuarios podrán citar tu trabajo así:

```bibtex
@software{cavieses_2026,
  title = {Curso de Programación y Computación - Simuladores Educativos},
  author = {Cavieses Núñez, Ricardo},
  year = {2026},
  doi = {[DOI que genera Zenodo]},
  url = {https://zenodo.org/record/[número]}
}
```

O en formato APA:

```
Cavieses Núñez, R. (2026). Curso de Programación y Computación - Simuladores Educativos [Software]. Zenodo. https://doi.org/[DOI]
```

## Ventajas de Publicar en Zenodo

1. **DOI permanente**: Tu trabajo obtiene un identificador único y permanente
2. **Acceso abierto**: Disponible gratuitamente para cualquiera
3. **Preservación digital**: Zenodo garantiza la preservación a largo plazo
4. **Citabilidad**: Fácil de citar en artículos académicos y trabajos
5. **Visibilidad**: Indexado en motores de búsqueda académicos
6. **Estadísticas**: Puedes ver cuántas veces se ha descargado y citado

## Archivos a Incluir en Zenodo

Se recomienda incluir:

```
curso_computacion/
├── README.md
├── CITATION.cff
├── .zenodo.json
├── games-data.json
├── LICENSE
├── index.html
├── logo_uabcs.png
├── ingeniería en pesquerías/
│   └── juegos/
│       ├── *.html
│       └── [archivos asociados]
└── ingeniería en prevensión de desastres.../
    └── juegos/
        ├── *.html
        └── [archivos asociados]
```

## Contacto y Soporte

- Para más información sobre Zenodo: https://about.zenodo.org/
- Documentación de Zenodo: https://developers.zenodo.org/
- Para preguntas sobre derechos de autor: contacta con tu institución

---

**Última actualización**: Marzo 2026
