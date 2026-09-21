
# Tarea 1: Construcción de Interfaces Web Adaptables con HTML y CSS

## Identificación
* **Nombre del estudiante:** Andrés Meléndez Carvajal
* **Curso:** Programación Web Avanzada (SOFT-12)
* **Sección:** SCV2
* **Periodo:** III Cuatrimestre 2026
* **Docente facilitador:** Álvaro Cordero Peña
* **Fecha de entrega:** 20 de setiembre de 2026

---

## Descripción de los Casos
* **Caso 1 - Centro de control de una expedición científica:** Diseñado para coordinadores de una expedición en Costa Rica. Funciona como un panel visual interactivo con CSS Grid en escritorio para visualizar simultáneamente indicadores KPI, misiones activas, alertas clasificadas por severidad, estado de equipos y agenda.
* **Caso 2 - Panel público de información de un festival:** Enfocado en asistentes que consultan eventos desde dispositivos móviles durante un festival cultural. Priorizando la sección «En este momento», avisos de última hora y servicios, reorganizándose en escritorio para comparar escenarios simultáneamente.

---

## Estructura del Repositorio
```text
Tarea1/
├── README.md
├── caso1/
│   ├── index.html
│   ├── css/
│   │   └── estilos.css
│   └── img/
└── caso2/
    ├── index.html
    ├── css/
    │   └── estilos.css
    └── img/
```

## Instrucciones para abrir cada caso

Este repositorio contiene dos proyectos independientes de maquetación web responsiva. Para visualizar y probar cada caso en tu navegador, sigue los pasos a continuación:

## Opciones de visualización

#### Opción 1: Abrir directamente desde el explorador de archivos
1. Descarga o clona este repositorio en tu equipo.
2. Navega hasta la carpeta del caso que deseas revisar:
   - Para el Caso 1 (Dashboard): abre la carpeta `caso1/`.
   - Para el Caso 2 (Festival Cultural): abre la carpeta `caso2/`.
3. Haz doble clic sobre el archivo `index.html` del caso correspondiente para abrirlo en tu navegador predeterminado (Chrome, Firefox, Edge, Safari, etc.).

#### Opción 2: Uso de la extensión Live Server (Visual Studio Code)
1. Abre la carpeta raíz del proyecto en Visual Studio Code.
2. Si aún no la tienes, instala la extensión **Live Server** desde el mercado de extensiones (`Ctrl + Shift + X`).
3. Abre el archivo `index.html` correspondiente al caso que deseas ejecutar:
   - `caso1/index.html`
   - `caso2/index.html`
4. Haz clic derecho sobre el editor y selecciona **"Open with Live Server"** (o presiona `Alt + L, Alt + O`).

---

### Prueba de Responsividad

Para verificar la adaptación responsiva en distintos dispositivos:
1. Con la página abierta en tu navegador, presiona la tecla `F12` (o clic derecho -> **Inspeccionar**) para abrir las Herramientas de Desarrollador (*DevTools*).
2. Haz clic en el icono de alternar la barra de dispositivos (`Ctrl + Shift + M` o `Cmd + Shift + M`).
3. Prueba las siguientes resoluciones principales:
   - **Móvil:** 320px – 600px.
   - **Tableta:** 601px – 1023px.
   - **Escritorio:** 1024px o superior.

## Decisiones de Diseño

El proyecto se desarrolló bajo el enfoque **Mobile-First**, diseñando primero para pantallas móviles (320px+) con una estructura lineal y limpia, y expandiendo el layout mediante *Media Queries* a partir de los 1024px. Para el posicionamiento de elementos clave se utilizó `position: relative` en el contenedor de las tarjetas junto con `position: absolute` en las etiquetas de estado ("EN VIVO"), lo que permite fijar la insignia con precisión en la esquina superior derecha sin romper el flujo del texto ni desordenar la información interna.

En cuanto a los estilos, se configuró un tema claro utilizando **variables CSS (`:root`) exclusivamente para la paleta de colores** (fondos, superficies, bordes y tonos semánticos para categorías). De esta manera se garantiza un alto contraste y una gestión de color centralizada y fácil de mantener, mientras que los valores de espaciados, bordes y tipografías se manejaron con unidades fijas (`rem` y `px`) para mantener un código directo, limpio y eficiente.

## Tabla Resumen de comits
| 2026-09-20 | 886c753 | Estilos completos para el html del caso 2, añadido |
| 2026-09-20 | 1284cdc | Estructura completa del html del caso 2 añadida |
| 2026-09-20 | 68818c7 | Estilos del caso 1 añadidos |
| 2026-09-20 | f2c9d81 | Estructura del html del caso 1 añadida |
| 2026-09-20 | 95f31d9 | Creación de estructura inicial de carpetas y archivos base HTML y CSS |