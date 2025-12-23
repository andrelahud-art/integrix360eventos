# Integrix360 Eventos - Landing Page Profesional

Landing page moderna y orientada a conversión para negocio de renta de inflables en León, Guanajuato.

## 🎯 Características

- ✅ **Diseño profesional y moderno** - Colores sobrios con acentos llamativos
- ✅ **100% Responsive** - Optimizado para móviles, tablets y desktop (Mobile-first)
- ✅ **Orientado a conversión** - CTAs estratégicos de WhatsApp en toda la página
- ✅ **SEO optimizado** - Meta tags, Schema.org y contenido para búsqueda local
- ✅ **Rendimiento optimizado** - CSS moderno, carga rápida
- ✅ **Accesible** - Cumple estándares de accesibilidad web
- ✅ **Fácil de personalizar** - Variables CSS para cambios rápidos

## 📁 Estructura del Proyecto

```
integrix360eventos/
├── index.html          # Página principal
├── css/
│   └── styles.css      # Estilos principales
└── README.md           # Este archivo
```

## 🚀 Cómo Usar

### 1. Personalizar Número de WhatsApp

**IMPORTANTE:** Debes cambiar el número de WhatsApp en TODAS las instancias.

Busca y reemplaza en `index.html`:

```
5214771234567
```

Por tu número de WhatsApp en formato internacional (sin espacios ni guiones):

```
52477XXXXXXXX
```

**Ubicaciones a cambiar:**
- Header (botón superior)
- Hero section (botón principal)
- Cada tarjeta de producto (4 botones)
- Sección de proceso
- CTA final
- Botón flotante de WhatsApp

### 2. Actualizar Información de Contacto

En el footer de `index.html`, actualiza:

```html
<li><i class="fas fa-phone"></i> 477-XXX-XXXX</li>
<li><i class="fab fa-whatsapp"></i> WhatsApp: 477-XXX-XXXX</li>
<li><i class="fas fa-envelope"></i> contacto@integrix360eventos.com</li>
```

### 3. Agregar Imágenes Reales de los Inflables

Actualmente la página usa placeholders con iconos. Para agregar imágenes reales:

1. Crea una carpeta `images/`:
```bash
mkdir images
```

2. Agrega tus imágenes (recomendado: formato WebP o JPG optimizado, 800x600px):
```
images/
├── castillo.jpg
├── unicornio.jpg
├── mario-bros.jpg
└── resbaladilla.jpg
```

3. En `index.html`, reemplaza los placeholders. Ejemplo para el Castillo:

**Antes:**
```html
<div class="product-card__image">
    <div class="product-card__placeholder">
        <i class="fas fa-fort-awesome"></i>
    </div>
    <span class="product-card__badge">Más Popular</span>
</div>
```

**Después:**
```html
<div class="product-card__image">
    <img src="images/castillo.jpg" alt="Inflable Castillo para fiestas infantiles">
    <span class="product-card__badge">Más Popular</span>
</div>
```

Repite para los 4 inflables.

### 4. Personalizar Colores de Marca (Opcional)

Si quieres cambiar los colores, edita las variables CSS en `css/styles.css`:

```css
:root {
    --color-primary: #25D366;        /* Verde WhatsApp - cámbialo por tu color principal */
    --color-secondary: #FF6B35;      /* Naranja acento */
    --color-accent: #FFD23F;         /* Amarillo acento */
}
```

### 5. Configurar Redes Sociales

En el footer, actualiza los enlaces de redes sociales:

```html
<a href="https://facebook.com/TU_PAGINA" target="_blank">
<a href="https://instagram.com/TU_CUENTA" target="_blank">
```

## 📱 Implementación de Analytics (Opcional pero Recomendado)

### Google Analytics 4

Agrega antes del `</head>` en `index.html`:

```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Facebook Pixel (Para anuncios en Facebook/Instagram)

Agrega después del `<body>` en `index.html`:

```html
<!-- Facebook Pixel Code -->
<script>
!function(f,b,e,v,n,t,s)
{if(f.fbq)return;n=f.fbq=function(){n.callMethod?
n.callMethod.apply(n,arguments):n.queue.push(arguments)};
if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
n.queue=[];t=b.createElement(e);t.async=!0;
t.src=v;s=b.getElementsByTagName(e)[0];
s.parentNode.insertBefore(t,s)}(window, document,'script',
'https://connect.facebook.net/en_US/fbevents.js');
fbq('init', 'TU_PIXEL_ID');
fbq('track', 'PageView');
</script>
<noscript><img height="1" width="1" style="display:none"
src="https://www.facebook.com/tr?id=TU_PIXEL_ID&ev=PageView&noscript=1"
/></noscript>
```

## 🌐 Publicar la Página Web

### Opción 1: GitHub Pages (Gratis y Fácil)

1. Sube tu código a GitHub
2. Ve a Settings > Pages
3. Selecciona la rama `main` y carpeta raíz
4. Tu sitio estará en: `https://tu-usuario.github.io/integrix360eventos`

### Opción 2: Netlify (Gratis, con dominio personalizado)

1. Crea cuenta en [Netlify](https://www.netlify.com)
2. Arrastra la carpeta del proyecto al dashboard
3. ¡Listo! Obtienes un dominio gratis: `tu-sitio.netlify.app`
4. Opcional: Conecta tu dominio personalizado

### Opción 3: Hosting Tradicional (cPanel, Hostinger, GoDaddy)

1. Sube todos los archivos vía FTP
2. Asegúrate de que `index.html` esté en la raíz
3. La carpeta `css/` debe estar en el mismo nivel

## 📊 Optimización para Google (SEO Local)

### 1. Google My Business

Registra tu negocio en [Google My Business](https://business.google.com):
- Nombre: Integrix360 Eventos
- Categoría: Servicio de alquiler de equipos para fiestas
- Ubicación: León, Guanajuato
- Agrega fotos de los inflables
- Solicita reseñas a tus clientes

### 2. Palabras Clave Recomendadas

Ya están incluidas en el HTML, pero puedes agregar más contenido con:
- "renta de inflables León"
- "inflables para fiestas Guanajuato"
- "renta de brincolines León"
- "inflables profesionales León"

### 3. Schema.org (Ya Incluido)

El código ya incluye marcado Schema.org para aparecer mejor en búsquedas locales.

## 🎨 Personalización Avanzada

### Agregar Más Inflables

Copia y pega un bloque `product-card` completo en la sección de productos:

```html
<div class="product-card">
    <div class="product-card__image">
        <img src="images/nuevo-inflable.jpg" alt="Descripción del inflable">
        <span class="product-card__badge">Nuevo</span>
    </div>
    <div class="product-card__content">
        <h3 class="product-card__title">Nombre del Inflable</h3>
        <p class="product-card__description">Descripción breve y atractiva.</p>
        <ul class="product-card__features">
            <li><i class="fas fa-check"></i> Característica 1</li>
            <li><i class="fas fa-check"></i> Característica 2</li>
            <li><i class="fas fa-check"></i> Característica 3</li>
        </ul>
        <a href="https://wa.me/52477XXXXXXX?text=Quiero%20cotizar%20NOMBRE"
           class="btn btn--secondary"
           target="_blank"
           rel="noopener">
            Cotizar ahora
        </a>
    </div>
</div>
```

### Cambiar Íconos

La página usa [Font Awesome 6](https://fontawesome.com/icons). Para cambiar un ícono:

1. Busca el ícono en fontawesome.com
2. Copia la clase (ej: `fas fa-star`)
3. Reemplaza en el HTML

## 📞 Configuración Avanzada de WhatsApp

### Mensajes Personalizados por Inflable

Ya están configurados. Cada producto tiene su propio mensaje:

```
Quiero cotizar el Inflable Castillo
Quiero cotizar el Inflable Unicornio
Quiero cotizar el Inflable Mario Bros
Quiero cotizar el Inflable Resbaladilla
```

Puedes personalizar estos mensajes en cada enlace `href="https://wa.me/..."`.

## ✅ Checklist Antes de Publicar

- [ ] Cambié TODOS los números de WhatsApp
- [ ] Actualicé el correo electrónico
- [ ] Actualicé el teléfono de contacto
- [ ] Cambié los enlaces de redes sociales
- [ ] Agregué imágenes reales de los inflables (opcional pero recomendado)
- [ ] Probé todos los botones de WhatsApp
- [ ] Revisé la página en móvil
- [ ] Configuré Google Analytics (opcional)
- [ ] Registré Google My Business

## 🛠️ Soporte Técnico

### Problemas Comunes

**Los estilos no se ven:**
- Verifica que `css/styles.css` exista
- Verifica la ruta en `<link rel="stylesheet" href="css/styles.css">`

**Los íconos no aparecen:**
- Verifica tu conexión a internet (Font Awesome se carga desde CDN)

**Los botones de WhatsApp no funcionan:**
- Verifica el formato del número: `5214771234567` (sin espacios, sin +)

## 📈 Métricas de Éxito

Después de publicar, monitorea:

1. **Conversiones por WhatsApp**
   - Cuántos mensajes recibes por día
   - Qué inflables son más cotizados

2. **Google Analytics**
   - Visitas diarias
   - Tiempo en página
   - Dispositivos más usados (móvil/desktop)

3. **Google Search Console**
   - Posiciones en búsquedas locales
   - Clics desde Google

## 📝 Licencia

Este código es propiedad de Integrix360 Eventos. Puedes modificarlo libremente para tu negocio.

---

**¿Necesitas ayuda?** Contacta a tu desarrollador web o consulta la documentación incluida en los comentarios del código.

**Hecho con ❤️ para Integrix360 Eventos - León, Guanajuato**
