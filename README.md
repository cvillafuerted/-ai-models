# Artículo Técnico: Usabilidad en el Desarrollo de Software

Este proyecto contiene un artículo técnico sobre usabilidad en el desarrollo de software, desarrollado con Quarto en una estructura modular.

## Estructura del Proyecto

```
Usabilidad_Informe/
├── index.qmd              # Archivo principal con frontmatter e inclusiones
├── 00-portada.qmd        # Portada del documento
├── 01-objectivos.qmd     # Objetivos del trabajo
├── 02-estado-arte.qmd    # Estado del arte en usabilidad
├── 03-analisis.qmd       # Análisis y reflexión
├── 04-conclusiones.qmd   # Conclusiones y recomendaciones
├── 05-bibliografia.qmd   # Referencias bibliográficas
├── _quarto.yml          # Configuración de Quarto
├── references.bib       # Bibliografía en formato BibTeX
├── styles.css          # Estilos CSS personalizados
├── header.tex         # Configuraciones LaTeX adicionales
├── apa.csl           # Estilo de citación APA
├── img/             # Directorio de imágenes
│   └── image.png    # Logo y otras imágenes
└── README.md        # Este archivo
```

## Contenido del Artículo

El artículo está estructurado en módulos separados:

1. **`00-portada.qmd`** - Portada con información del título, autores y universidad
2. **`01-objectivos.qmd`** - Objetivos del trabajo
3. **`02-estado-arte.qmd`** - Definiciones, principios y estándares de usabilidad
4. **`03-analisis.qmd`** - Importancia y evaluación de la usabilidad
5. **`04-conclusiones.qmd`** - Resumen y recomendaciones
6. **`05-bibliografia.qmd`** - Referencias en formato APA

## Ventajas de la Estructura Modular

- ✅ **Mantenimiento más fácil** - Cada sección en su propio archivo
- ✅ **Colaboración mejorada** - Múltiples personas pueden trabajar en diferentes secciones
- ✅ **Reutilización** - Los módulos pueden reutilizarse en otros proyectos
- ✅ **Organización clara** - Estructura lógica y fácil de navegar
- ✅ **Control de versiones** - Cambios más granulares y fáciles de rastrear

## Requisitos

Para trabajar con este proyecto necesitas:

- [Quarto](https://quarto.org/) instalado en tu sistema
- Un editor de texto (VS Code, RStudio, etc.)
- Conocimientos básicos de Markdown

## Instalación y Uso

### 1. Instalar Quarto

Visita [quarto.org](https://quarto.org/docs/get-started/) y sigue las instrucciones de instalación para tu sistema operativo.

### 2. Verificar la instalación

```bash
quarto --version
```

### 3. Renderizar el documento

Desde la terminal, en el directorio del proyecto:

```bash
# Renderizar a HTML
quarto render index.qmd --to html

# Renderizar a PDF
quarto render index.qmd --to pdf

# Renderizar a Word
quarto render index.qmd --to docx
```

### 4. Vista previa en tiempo real

```bash
quarto preview
```

## Trabajando con Módulos

### Editar una sección específica

Para editar una sección específica, simplemente abre el archivo correspondiente:

- `01-portada.qmd` - Para modificar la portada y objetivos
- `02-estado-arte.qmd` - Para el estado del arte
- `03-analisis.qmd` - Para el análisis y reflexión
- `04-conclusiones.qmd` - Para las conclusiones
- `05-bibliografia.qmd` - Para la bibliografía

### Agregar nuevas secciones

Para agregar una nueva sección:

1. Crea un nuevo archivo `.qmd` (ej: `06-nueva-seccion.qmd`)
2. Agrega el contenido de la sección
3. Incluye el archivo en `index.qmd` usando `{=include} 06-nueva-seccion.qmd`
4. Actualiza `_quarto.yml` si es necesario

### Reorganizar secciones

Para cambiar el orden de las secciones:

1. Modifica el orden de las inclusiones en `index.qmd`
2. Actualiza la numeración de los archivos si es necesario

## Personalización

### Modificar el contenido

Edita los archivos `.qmd` individuales para modificar el contenido de cada sección. Cada archivo es independiente y puede ser editado por separado.

### Agregar referencias

Edita el archivo `references.bib` para agregar nuevas referencias bibliográficas. Usa el formato BibTeX estándar.

### Personalizar estilos

Modifica el archivo `styles.css` para cambiar la apariencia del documento HTML.

### Configuración de Quarto

Ajusta la configuración en `_quarto.yml` según tus preferencias.

## Formato de Referencias

El proyecto está configurado para usar el formato APA. Las referencias se citan en el texto usando `[@clave]` y se generan automáticamente al final del documento.

## Estructura de Secciones

Cada sección del artículo tiene un identificador único:

- `#objetivos` - Sección de objetivos
- `#estado-arte` - Estado del arte
- `#analisis` - Análisis y reflexión
- `#conclusiones` - Conclusiones
- `#bibliografia` - Bibliografía

## Consejos para el Desarrollo

1. **Mantén la estructura modular**: Respeta la organización en archivos separados
2. **Usa nombres descriptivos**: Los nombres de archivo deben reflejar su contenido
3. **Cita apropiadamente**: Usa las referencias del archivo `references.bib`
4. **Revisa la ortografía**: Usa un corrector ortográfico
5. **Prueba la renderización**: Verifica que el documento se renderice correctamente
6. **Mantén versiones**: Usa control de versiones (Git) para seguir los cambios

## Solución de Problemas

### Error de renderización

Si encuentras errores al renderizar:

1. Verifica que Quarto esté instalado correctamente
2. Asegúrate de que todos los archivos estén en el directorio correcto
3. Revisa la sintaxis de Markdown en los archivos `.qmd`
4. Verifica el formato de las referencias en `references.bib`
5. Comprueba que las inclusiones en `index.qmd` sean correctas

### Problemas con las referencias

Si las referencias no se generan correctamente:

1. Verifica que el archivo `references.bib` esté en formato correcto
2. Asegúrate de que las citas en el texto usen la sintaxis `[@clave]`
3. Verifica que el archivo `apa.csl` esté disponible (se descarga automáticamente)

### Problemas con módulos

Si algún módulo no se incluye correctamente:

1. Verifica que el archivo existe y tiene la extensión `.qmd`
2. Comprueba que la sintaxis de inclusión sea correcta: `{=include} archivo.qmd`
3. Asegúrate de que el archivo esté en el mismo directorio que `index.qmd`

## Recursos Adicionales

- [Documentación de Quarto](https://quarto.org/docs/)
- [Guía de Markdown](https://quarto.org/docs/authoring/markdown-basics.html)
- [Gestión de referencias en Quarto](https://quarto.org/docs/authoring/footnotes-and-citations.html)
- [Personalización de estilos](https://quarto.org/docs/output-formats/html-themes.html)
- [Inclusiones en Quarto](https://quarto.org/docs/authoring/include-code.html)

## Licencia

Este proyecto es para uso educativo. Puedes modificar y distribuir libremente para fines académicos.
