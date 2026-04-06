# Template LaTeX - Tesis de Grado Ingeniería de Sonido (UNTREF)

Este repositorio contiene una plantilla en formato LaTeX con la estructura y formato esperados para la Tesis de Grado de la carrera de Ingeniería de Sonido en la UNTREF. 

La idea principal es que este sea un repositorio grupal y colaborativo. El objetivo es que entre todos vayamos actualizando el *template* a medida que surjan nuevos requerimientos o cambios formales por parte de la materia.

## 🚀 Uso

Podés compilar este documento usando distintas herramientas según tu entorno de preferencia, como TeXstudio, VS Code o Overleaf. 

> **Aviso sobre Overleaf:** Por el tamaño y la longitud final que suele tener el documento de la tesis, es muy probable que requieras una versión paga de Overleaf para evitar que la compilación se corte por "timeout".

A continuación vas a encontrar las instrucciones para ejecutar este proyecto de forma local usando VS Code (se aceptan contribuciones con instrucciones de uso en otros editores).

### Uso en VS Code

Para trabajar de forma local, yo utilizo VS Code con la extensión **[LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)**.

**Pasos:**
1. Instalar una distribución de LaTeX de forma local en tu sistema (por ejemplo, TeX Live en Linux/Windows o MacTeX en macOS). Para Windows recomiendo [TeX Live](https://www.tug.org/texlive/).
2. Instalar la extensión LaTeX Workshop en VS Code.
3. Abrir la carpeta raíz de este repositorio en VS Code.
4. Usar la UI de la extensión para generar el PDF.

**Citas:**
Para que se vean las citas usando el formato, se tienen que agregar las referencias en el archivo `reference.bib`. 

Si la extensión no resuelve las citas automáticamente, vas a necesitar compilar la bibliografía. El flujo de trabajo manual para que el documento integre bien todas las referencias requiere ejecutar los siguientes comandos en la terminal integrada de VS Code:

```bash
biber main
```

💡 **Automatización:** Para no tener que ejecutar `biber` manualmente cada vez que agregás una cita, podés configurar la extensión para que lo haga por vos. Te recomiendo leer la [documentación oficial de LaTeX Workshop sobre "Recipes" y "Tools"](https://github.com/James-Yu/LaTeX-Workshop/wiki/Compile), donde explican cómo agregar `biber` a tu cadena de compilación (`settings.json`).

## 📝 Changelog / Versiones

* **v1.0.0**: El documento actual y su estructura están validados por la cátedra de *Taller de Tesis* durante el segundo cuatrimestre de 2025. 

## 🤝 Contribuciones

¡Todas las contribuciones son bienvenidas! Si encontrás algún error, querés sumar un paquete útil, o adaptar el formato a un nuevo requerimiento de la cátedra:

1. Creá una nueva rama desde `main` (ej: `git checkout -b mejora-formato-bibliografia`).
2. Hacé tus cambios y commitealos.
3. Subí la rama y mandá un **Pull Request (PR)** para que lo revisemos y lo sumemos al proyecto.

El pasaje del documento original en Word a Latex fue un esfuerzo conjunto de muchos compañeros de la carrera.