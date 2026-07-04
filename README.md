# Perfil Profesional — Edwin Andres Sanchez Orozco

Portfolio personal con tematica cyberpunk/neon. Los datos se cargan dinamicamente desde la API de GitHub.

## Estructura del proyecto

```
/
├── index.html              # Pagina principal
├── assets/
│   ├── css/
│   │   └── style.css       # Estilos (modo oscuro/claro)
│   ├── js/
│   │   └── app.js          # Logica JS (i18n, API, animaciones)
│   ├── img/
│   │   ├── logo.png        # Avatar / Favicon
│   │   └── projects/       # Capturas de proyectos
│   │       ├── vial-servi/
│   │       ├── sistema-transito/
│   │       ├── proconnect/
│   │       ├── poke-api/
│   │       ├── poliglota/
│   │       └── cubo-ps2/   # (contiene video.mp4)
│   ├── video/
│   │   └── videoplayback.webm  # Video de fondo
│   └── certificates/       # PDFs de certificados y hoja de vida
├── deploy-configs/         # Configs de deploy para sub-proyectos
├── .opencode/              # Configuracion de OpenCode AI
└── .gitignore
```

## Funcionalidades

-   Tema oscuro/claro con transiciones animadas (hyperspace jump / quantum flicker)
-   Bilingue ES/EN con traduccion completa
-   Avatar dinamico desde GitHub API
-   Terminal de perfil con efecto de tipeado al hacer scroll
-   Skills con hover terminal (codigo Hello World en cada lenguaje)
-   Galeria de proyectos con visor de imagenes y navegacion
-   Timeline de experiencia con estilo neon
-   Modal de certificados y hoja de vida
-   Navbar con ocultamiento al scrollear y resaltado de seccion activa

## Como usar

1.  Abre `index.html` en un navegador (no requiere servidor)
2.  Los datos de GitHub se cargan automaticamente desde `AndresSanchez12323`
3.  Para anadir certificados, coloca los PDFs en `assets/certificates/` y actualiza `renderCertificates()` en `assets/js/app.js`

## Personalizar

-   **Colores**: editar variables CSS en `:root` y `[data-theme="light"]` en `assets/css/style.css`
-   **Traducciones**: editar `TRANSLATIONS` en `assets/js/app.js`
-   **Skills**: editar `SKILLS` y `HELLO_WORLD` en `assets/js/app.js`
-   **Proyectos destacados**: editar `PROJECT_MEDIA` en `assets/js/app.js`
-   **Redes sociales**: editar la seccion `#contacto` en `index.html`

## Requisitos

-   Navegador moderno con soporte CSS Grid, Flexbox, y Fetch API
-   Conexion a internet para carga inicial de datos de GitHub
-   No requiere build tools ni servidor
