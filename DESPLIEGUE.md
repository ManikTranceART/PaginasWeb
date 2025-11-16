# Instrucciones de Despliegue / Deployment Instructions

## 🌐 Cómo Crear Tu Dominio Personal / How to Create Your Personal Domain

Este hub está listo para ser desplegado en línea. Aquí están las opciones más populares:

### Opción 1: GitHub Pages (Recomendado - Gratis)

**Paso a paso:**

1. **Ir a la configuración del repositorio:**
   - Abre tu repositorio en GitHub
   - Haz clic en "Settings" (Configuración)

2. **Configurar GitHub Pages:**
   - En el menú lateral, busca "Pages"
   - En "Source", selecciona la rama `main` (o la rama que estés usando)
   - Selecciona la carpeta raíz `/` como directorio de publicación
   - Haz clic en "Save"

3. **Acceder a tu sitio:**
   - Tu sitio estará disponible en: `https://maniktranceart.github.io/PaginasWeb/`
   - GitHub te mostrará la URL exacta después de guardar

4. **Dominio personalizado (opcional):**
   - Puedes configurar un dominio personalizado (como `miportfolio.com`)
   - Necesitarás comprar un dominio y configurar los DNS
   - Instrucciones: https://docs.github.com/es/pages/configuring-a-custom-domain-for-your-github-pages-site

### Opción 2: Netlify (Gratis con más características)

**Paso a paso:**

1. **Crear cuenta:**
   - Visita https://www.netlify.com/
   - Regístrate con tu cuenta de GitHub

2. **Importar proyecto:**
   - Haz clic en "New site from Git"
   - Selecciona GitHub y autoriza el acceso
   - Elige el repositorio `PaginasWeb`

3. **Configurar despliegue:**
   - Build command: (dejar vacío)
   - Publish directory: `/` o `.`
   - Haz clic en "Deploy site"

4. **Tu dominio:**
   - Netlify te dará un dominio como `nombre-aleatorio.netlify.app`
   - Puedes cambiar el subdominio en Site settings > Domain management
   - También puedes usar tu propio dominio personalizado

### Opción 3: Vercel (Gratis para proyectos personales)

**Paso a paso:**

1. **Crear cuenta:**
   - Visita https://vercel.com/
   - Regístrate con tu cuenta de GitHub

2. **Importar proyecto:**
   - Haz clic en "New Project"
   - Selecciona el repositorio `PaginasWeb`

3. **Desplegar:**
   - Vercel detectará automáticamente la configuración
   - Haz clic en "Deploy"

4. **Tu dominio:**
   - Obtendrás un dominio como `paginasweb.vercel.app`
   - Puedes personalizar el subdominio
   - Soporte para dominios personalizados

### Opción 4: Hosting Tradicional (Requiere hosting pago)

Si tienes un hosting web tradicional:

1. **Conectar por FTP:**
   - Usa un cliente FTP como FileZilla
   - Conecta con las credenciales de tu hosting

2. **Subir archivos:**
   - Sube todos los archivos del repositorio
   - Mantén la estructura de carpetas

3. **Acceder:**
   - Tu sitio estará en `http://tudominio.com`

## 🔄 Actualizaciones Automáticas

Con GitHub Pages, Netlify y Vercel:
- Cada vez que hagas `git push` a tu repositorio
- El sitio se actualizará automáticamente
- No necesitas hacer nada más

## 📝 Dominios Gratuitos de Estudiante

Si eres estudiante, puedes obtener beneficios:

### GitHub Student Developer Pack
- Incluye: Dominio gratuito de .me por un año
- Créditos en varios servicios de hosting
- Solicítalo en: https://education.github.com/pack

### Beneficios adicionales:
- Dominio `.me` gratis con Namecheap
- Hosting en Heroku
- Créditos en DigitalOcean
- Y muchos más servicios

## 🎓 Dominios de Escuela

Si tu escuela proporciona dominios:
- Contacta al departamento de IT de tu escuela
- Pregunta por servicios de hosting para estudiantes
- Muchas escuelas ofrecen subdominios como `usuario.escuela.edu`

## ✅ Verificación

Después de desplegar, verifica:
1. ✅ La página principal carga correctamente
2. ✅ Los estilos se aplican (colores, diseño)
3. ✅ Los enlaces de navegación funcionan
4. ✅ Los proyectos se abren correctamente
5. ✅ El sitio es responsive (prueba en móvil)

## 🆘 Solución de Problemas

**Los estilos no se ven:**
- Verifica que la ruta en `index.html` sea correcta: `href="styles/main.css"`
- Asegúrate de subir la carpeta `styles/`

**Los enlaces no funcionan:**
- Usa rutas relativas, no absolutas
- Ejemplo correcto: `proyectos/proyecto1/index.html`
- Ejemplo incorrecto: `/proyectos/proyecto1/index.html`

**404 Error:**
- Verifica que `index.html` esté en la raíz del proyecto
- Asegúrate de que el nombre sea exactamente `index.html` (minúsculas)

---

¡Tu hub de desarrollo web ya está listo para el mundo! 🚀
