# Landing Page - IngeniaSoft

Una landing page moderna y profesional para empresas de tecnología, construida con HTML, CSS y JavaScript vanilla.

## 🚀 Características

- **Diseño Responsivo**: Se adapta perfectamente a todos los dispositivos
- **Navegación Suave**: Scroll suave entre secciones
- **Animaciones Modernas**: Efectos visuales atractivos y profesionales
- **Formulario de Contacto**: Con validación en tiempo real
- **Optimización SEO**: Meta tags y estructura semántica
- **Navegación Móvil**: Menú hamburguesa para dispositivos móviles
- **Efectos Interactivos**: Hover effects y animaciones de entrada

## 📁 Estructura del Proyecto

```
anding page ingeniasoft/
├── index.html          # Página principal
├── styles.css          # Estilos CSS
├── script.js           # Funcionalidades JavaScript
└── README.md           # Este archivo
```

## 🎨 Secciones Incluidas

1. **Header/Navegación**: Logo y menú de navegación
2. **Hero Section**: Título principal con llamadas a la acción
3. **Servicios**: 6 servicios principales con iconos
4. **Nosotros**: Información de la empresa con estadísticas
5. **Proyectos**: Portfolio de trabajos destacados
6. **Contacto**: Formulario de contacto e información de contacto
7. **Footer**: Enlaces adicionales y redes sociales

## 🛠️ Personalización

### Cambiar Colores

Los colores principales están definidos en `styles.css`:

```css
/* Colores principales */
--primary-color: #2563eb;      /* Azul principal */
--secondary-color: #fbbf24;    /* Amarillo/dorado */
--gradient-primary: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
--text-dark: #1f2937;
--text-light: #6b7280;
```

### Modificar Contenido

1. **Información de la Empresa**: Edita el contenido en `index.html`
2. **Servicios**: Modifica las tarjetas de servicios en la sección correspondiente
3. **Proyectos**: Actualiza los proyectos destacados
4. **Contacto**: Cambia la información de contacto y redes sociales

### Agregar Imágenes

Para agregar imágenes reales:

1. Crea una carpeta `images/` en el proyecto
2. Reemplaza los iconos FontAwesome con imágenes:
   ```html
   <!-- En lugar de: -->
   <i class="fas fa-code"></i>
   
   <!-- Usa: -->
   <img src="images/your-image.jpg" alt="Descripción">
   ```

### Modificar Animaciones

Las animaciones están en `styles.css` y `script.js`:

- **CSS**: Busca las secciones `@keyframes` y `.animation`
- **JavaScript**: Modifica las funciones de animación en `script.js`

## 📱 Responsive Design

La landing page incluye breakpoints para:

- **Desktop**: > 768px
- **Tablet**: 768px - 480px
- **Mobile**: < 480px

## 🔧 Funcionalidades JavaScript

### Navegación
- Menú hamburguesa para móviles
- Scroll suave entre secciones
- Header con efecto de transparencia

### Animaciones
- Contadores animados en la sección "Nosotros"
- Efectos de entrada para tarjetas
- Animación de escritura en el título principal
- Efecto parallax suave

### Formulario
- Validación en tiempo real
- Notificaciones de éxito/error
- Validación de email

## 🚀 Despliegue

### Opción 1: Servidor Local
```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx serve .

# Usando PHP
php -S localhost:8000
```

### Opción 2: Hosting Estático
- **Netlify**: Arrastra la carpeta del proyecto
- **Vercel**: Conecta tu repositorio Git
- **GitHub Pages**: Sube a un repositorio público

### Opción 3: Servidor Web
Sube los archivos a tu servidor web (Apache, Nginx, etc.)

## 📧 Integración del Formulario

El formulario actualmente simula el envío. Para integrarlo con un backend:

1. **Modifica la función de envío en `script.js`**:
```javascript
// Reemplaza la simulación con una llamada real
fetch('/api/contact', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(data)
})
.then(response => response.json())
.then(data => {
    showNotification('Mensaje enviado correctamente', 'success');
})
.catch(error => {
    showNotification('Error al enviar el mensaje', 'error');
});
```

2. **O usa servicios como**:
   - Formspree
   - Netlify Forms
   - EmailJS

## 🎯 SEO y Optimización

### Meta Tags Incluidos
- Título optimizado
- Descripción meta
- Viewport para responsive
- Charset UTF-8

### Mejoras Sugeridas
1. Agregar Open Graph tags para redes sociales
2. Incluir schema markup
3. Optimizar imágenes con WebP
4. Agregar sitemap.xml
5. Configurar robots.txt

## 🔍 Próximas Mejoras

- [ ] Modo oscuro
- [ ] Más animaciones
- [ ] Galería de imágenes
- [ ] Blog integrado
- [ ] Chat en vivo
- [ ] Testimonios de clientes
- [ ] Integración con CRM

## 📞 Soporte

Para personalizaciones adicionales o soporte técnico, contacta a tu equipo de desarrollo.

## 📄 Licencia

Este proyecto está disponible para uso comercial y personal.

---

**IngeniaSoft** - Transformando ideas en soluciones digitales innovadoras. 