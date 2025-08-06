# Mi Página Personal - Jekyll

Una página web personal moderna construida con Jekyll y GitHub Pages para mostrar proyectos, blog y información personal.

## 🚀 Características

- **Diseño Moderno**: Interfaz limpia y responsive con animaciones suaves
- **Blog Personal**: Sistema de blog integrado con categorías y etiquetas
- **Portafolio de Proyectos**: Muestra tus proyectos con filtros por categoría
- **Página Sobre Mí**: Información personal, experiencia y habilidades
- **SEO Optimizado**: Meta tags, sitemap y estructura semántica
- **Navegación Intuitiva**: Menú responsive y navegación fluida
- **Animaciones**: Efectos visuales y transiciones suaves
- **Lightbox**: Visualización de imágenes en pantalla completa

## 📋 Requisitos Previos

- Ruby 2.7 o superior
- RubyGems
- Git

## 🛠️ Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/tu-repositorio.git
cd tu-repositorio
```

### 2. Instalar dependencias

```bash
bundle install
```

### 3. Configurar el sitio

Edita el archivo `_config.yml` con tu información personal:

```yaml
# Información personal
title: "Tu Nombre"
description: "Tu descripción personal"
author: "Tu Nombre"
email: "tu.email@ejemplo.com"
url: "https://tu-usuario.github.io"

# Redes sociales
social:
  github: tu-usuario
  linkedin: tu-usuario-linkedin
  twitter: tu-usuario-twitter
  email: tu.email@ejemplo.com
```

### 4. Ejecutar localmente

```bash
bundle exec jekyll serve
```

El sitio estará disponible en `http://localhost:4000`

## 📁 Estructura del Proyecto

```
├── _config.yml              # Configuración principal
├── _layouts/                # Layouts de Jekyll
│   ├── default.html         # Layout base
│   ├── home.html           # Layout para página de inicio
│   ├── post.html           # Layout para posts del blog
│   ├── project.html        # Layout para proyectos
│   └── page.html           # Layout para páginas simples
├── _posts/                  # Posts del blog
├── _projects/               # Proyectos (colección personalizada)
├── assets/                  # Archivos estáticos
│   ├── css/
│   ├── js/
│   └── images/
├── index.html              # Página de inicio
├── sobre-mi.html           # Página "Sobre Mí"
├── proyectos.html          # Listado de proyectos
├── blog.html               # Listado del blog
└── README.md
```

## ✍️ Crear Contenido

### Nuevo Post del Blog

Crea un archivo en `_posts/` con el formato `YYYY-MM-DD-titulo.md`:

```markdown
---
layout: post
title: "Título del Post"
date: 2024-01-15
categories: [desarrollo]
tags: [javascript, react, tutorial]
description: "Descripción del post"
image: /assets/images/blog/imagen.jpg
author: Tu Nombre
---

Contenido del post en Markdown...
```

### Nuevo Proyecto

Crea un archivo en `_projects/` con el formato `nombre-proyecto.md`:

```markdown
---
layout: project
title: "Nombre del Proyecto"
date: 2024-01-10
description: "Descripción del proyecto"
image: /assets/images/projects/imagen.jpg
category: web
status: Completado
featured: true
technologies: [React, Node.js, MongoDB]
tags: [web, react, fullstack]
github: "https://github.com/tu-usuario/proyecto"
demo: "https://proyecto.vercel.app"
---

Contenido detallado del proyecto...
```

## 🎨 Personalización

### Colores

Edita las variables CSS en `assets/css/main.css`:

```css
:root {
    --primary-color: #3b82f6;
    --primary-dark: #2563eb;
    --secondary-color: #64748b;
    /* ... más variables */
}
```

### Imágenes

- **Foto de perfil**: Coloca tu imagen en `assets/images/profile.jpg`
- **Imágenes de proyectos**: `assets/images/projects/`
- **Imágenes del blog**: `assets/images/blog/`

### Navegación

Modifica la navegación en `_config.yml`:

```yaml
navigation:
  - title: Inicio
    url: /
  - title: Proyectos
    url: /proyectos/
  - title: Blog
    url: /blog/
  - title: Sobre Mí
    url: /sobre-mi/
```

## 🚀 Despliegue en GitHub Pages

### 1. Crear repositorio

Crea un nuevo repositorio en GitHub con el nombre `tu-usuario.github.io`

### 2. Subir código

```bash
git add .
git commit -m "Initial commit"
git push origin main
```

### 3. Configurar GitHub Pages

1. Ve a Settings > Pages
2. En Source, selecciona "Deploy from a branch"
3. Selecciona la rama `main` y la carpeta `/ (root)`
4. Haz clic en Save

### 4. Configurar Jekyll

GitHub Pages detectará automáticamente que es un sitio Jekyll y lo construirá.

## 🔧 Configuración Avanzada

### Plugins

El sitio incluye estos plugins de Jekyll:

- `jekyll-feed`: Genera feed RSS
- `jekyll-seo-tag`: Optimización SEO
- `jekyll-sitemap`: Genera sitemap

### Variables de Entorno

Para desarrollo local, puedes crear un archivo `.env`:

```bash
JEKYLL_ENV=development
```

### Optimización

- **Imágenes**: Usa formatos WebP y optimiza el tamaño
- **CSS/JS**: Los archivos ya están minificados
- **Lazy Loading**: Implementado para imágenes

## 📱 Responsive Design

El sitio está optimizado para:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (320px - 767px)

## 🔍 SEO

El sitio incluye:
- Meta tags optimizados
- Open Graph para redes sociales
- Sitemap automático
- Estructura semántica HTML5
- URLs amigables

## 🐛 Solución de Problemas

### Error de dependencias

```bash
bundle update
```

### Error de permisos

```bash
sudo gem install bundler
```

### Puerto ocupado

```bash
bundle exec jekyll serve --port 4001
```

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature
3. Commit tus cambios
4. Push a la rama
5. Abre un Pull Request

## 📞 Contacto

- **Email**: tu.email@ejemplo.com
- **GitHub**: [@tu-usuario](https://github.com/tu-usuario)
- **LinkedIn**: [Tu Nombre](https://linkedin.com/in/tu-usuario)

---

¡Espero que este template te ayude a crear una página personal increíble! 🚀 