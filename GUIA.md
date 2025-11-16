# Guía de Uso del Hub de Desarrollo Web

Este repositorio sirve como un hub central para organizar y mostrar todas tus aplicaciones web y proyectos de desarrollo.

## 📁 Estructura del Proyecto

```
PaginasWeb/
├── index.html          # Página principal del hub
├── styles/
│   └── main.css       # Estilos principales
├── proyectos/         # Carpeta para tus proyectos web
│   ├── proyecto1/
│   │   └── index.html
│   ├── proyecto2/
│   │   └── index.html
│   └── proyecto3/
│       └── index.html
└── GUIA.md            # Este archivo
```

## 🚀 Cómo Añadir un Nuevo Proyecto

### Opción 1: Proyecto Simple (HTML/CSS/JS)

1. Crea una nueva carpeta dentro de `proyectos/`:
   ```bash
   mkdir proyectos/mi-nuevo-proyecto
   ```

2. Añade tus archivos HTML, CSS y JavaScript:
   ```bash
   proyectos/mi-nuevo-proyecto/
   ├── index.html
   ├── styles.css
   └── script.js
   ```

3. Actualiza `index.html` principal para incluir tu proyecto:
   - Añade una nueva tarjeta de proyecto en la sección `<div class="projects-grid">`
   - Copia y modifica una tarjeta existente
   - Actualiza el título, descripción, tags y enlace

### Opción 2: Proyecto con Framework (React, Vue, Angular)

1. Desarrolla tu proyecto normalmente con tu framework preferido

2. Construye el proyecto para producción:
   ```bash
   npm run build
   # o
   yarn build
   ```

3. Copia los archivos compilados a `proyectos/nombre-proyecto/`

4. Actualiza la página principal como se describe arriba

## 🎨 Personalización

### Modificar Colores

Edita las variables CSS en `styles/main.css`:

```css
:root {
    --primary-color: #4a90e2;    /* Color principal */
    --secondary-color: #2c3e50;   /* Color secundario */
    --accent-color: #e74c3c;      /* Color de acento */
}
```

### Añadir Imágenes a los Proyectos

1. Crea una carpeta `assets/` o `images/` en la raíz:
   ```bash
   mkdir assets/images
   ```

2. Añade tus imágenes y reemplaza el `<div class="placeholder-image">` en las tarjetas:
   ```html
   <div class="project-image">
       <img src="assets/images/proyecto1.jpg" alt="Proyecto 1">
   </div>
   ```

3. Añade estilos para las imágenes en `styles/main.css`:
   ```css
   .project-image img {
       width: 100%;
       height: 100%;
       object-fit: cover;
   }
   ```

## 🌐 Despliegue

### GitHub Pages

1. Ve a la configuración de tu repositorio en GitHub
2. Navega a "Pages" en el menú lateral
3. En "Source", selecciona la rama `main` (o la que prefieras)
4. Selecciona la carpeta raíz `/` 
5. Haz clic en "Save"
6. Tu sitio estará disponible en: `https://[tu-usuario].github.io/PaginasWeb/`

### Netlify

1. Crea una cuenta en [Netlify](https://www.netlify.com/)
2. Conecta tu repositorio de GitHub
3. Configura el despliegue:
   - Build command: (deja vacío si no hay proceso de build)
   - Publish directory: `/`
4. Haz clic en "Deploy"

### Vercel

1. Crea una cuenta en [Vercel](https://vercel.com/)
2. Importa tu repositorio de GitHub
3. Vercel detectará automáticamente la configuración
4. Haz clic en "Deploy"

## 📝 Ejemplo de Tarjeta de Proyecto

```html
<div class="project-card">
    <div class="project-image">
        <div class="placeholder-image">🎮</div>
    </div>
    <div class="project-info">
        <h3>Mi Juego Web</h3>
        <p>Un juego interactivo creado con JavaScript vanilla.</p>
        <div class="project-tags">
            <span class="tag">HTML5</span>
            <span class="tag">CSS3</span>
            <span class="tag">JavaScript</span>
        </div>
        <a href="proyectos/mi-juego/index.html" class="btn btn-secondary">Ver Proyecto</a>
    </div>
</div>
```

## 🔧 Mantenimiento

- **Actualizar información personal**: Edita la sección "Sobre Mí" en `index.html`
- **Cambiar enlaces de contacto**: Modifica la sección "Contacto" en `index.html`
- **Añadir más páginas**: Crea nuevas páginas HTML y enlázalas desde el menú de navegación

## 💡 Consejos

1. **Organización**: Mantén cada proyecto en su propia carpeta con todos sus recursos
2. **Nombres descriptivos**: Usa nombres claros para las carpetas de proyectos
3. **README por proyecto**: Considera añadir un README.md en cada carpeta de proyecto
4. **Versionado**: Usa Git para mantener un historial de cambios
5. **Respaldo**: Mantén copias de seguridad de tus proyectos importantes

## 📚 Recursos Útiles

- [MDN Web Docs](https://developer.mozilla.org/) - Documentación web
- [CSS-Tricks](https://css-tricks.com/) - Trucos y guías de CSS
- [JavaScript.info](https://javascript.info/) - Tutorial moderno de JavaScript
- [GitHub Pages](https://pages.github.com/) - Hosting gratuito

## 🆘 Problemas Comunes

### Los enlaces no funcionan
- Verifica que las rutas sean correctas (relativas o absolutas)
- Asegúrate de que los archivos existen en las ubicaciones especificadas

### Los estilos no se aplican
- Verifica que el archivo CSS esté correctamente enlazado
- Revisa la consola del navegador para errores
- Asegúrate de que las rutas a los archivos CSS sean correctas

### El sitio no se ve bien en móviles
- El diseño ya es responsive, pero verifica tus proyectos individuales
- Usa `meta viewport` en todos tus archivos HTML
- Prueba en diferentes tamaños de pantalla

---

¡Disfruta construyendo tu hub de desarrollo web! 🚀
