# Guía Completa: Cómo Aparecer en Google Noticias (Google News)

> **Última actualización:** Mayo 2026  
> **Audiencia:** Editores, periodistas digitales, SEO specialists, dueños de medios  
> **Objetivo:** Lograr indexación y posicionamiento sostenido en Google News

---

## Índice

1. [¿Qué es Google Noticias?](#1-qué-es-google-noticias)
2. [Funcionamiento del Algoritmo](#2-funcionamiento-del-algoritmo)
3. [Requisitos Fundamentales](#3-requisitos-fundamentales)
4. [Arquitectura Profesional del Sitio](#4-arquitectura-profesional-del-sitio)
5. [Implementación Técnica](#5-implementación-técnica)
6. [Sitemap XML](#6-sitemap-xml)
7. [robots.txt](#7-robotstxt)
8. [Structured Data — Schema.org](#8-structured-data--schemaorg)
9. [Google Search Console](#9-google-search-console)
10. [Google Publisher Center](#10-google-publisher-center)
11. [Producción Editorial](#11-producción-editorial)
12. [Factores de Posicionamiento](#12-factores-de-posicionamiento)
13. [Errores Críticos](#13-errores-críticos)
14. [Flujo Profesional de Publicación](#14-flujo-profesional-de-publicación)
15. [Tecnologías Recomendadas](#15-tecnologías-recomendadas)
16. [Seguridad y Rendimiento](#16-seguridad-y-rendimiento)
17. [Monetización](#17-monetización)
18. [Métricas y KPIs](#18-métricas-y-kpis)
19. [Checklist de Lanzamiento](#19-checklist-de-lanzamiento)
20. [Recursos Oficiales](#20-recursos-oficiales)

---

## 1. ¿Qué es Google Noticias?

Google Noticias (**Google News**) es un agregador automatizado de contenido periodístico. A diferencia del buscador web tradicional, Google News clasifica, organiza y muestra **exclusivamente contenido noticioso** proveniente de fuentes editoriales.

### Diferencias clave con el buscador web estándar

| Aspecto | Google Search | Google News |
|---|---|---|
| Tipo de contenido | Cualquier página web | Solo contenido periodístico |
| Factor temporal | Relevancia general | **Actualidad** pesa más |
| Algoritmo principal | RankBrain, BERT | Freshness + Autoridad editorial |
| Indexación | Contenido perenne | Contenido sensible al tiempo |
| Formatos | Todos | NewsArticle, BlogPosting |

### Beneficios de aparecer en Google News

- **Aumento de tráfico orgánico** — Los artículos reciben exposición inmediata en el Top Stories.
- **Mejora de autoridad digital** — Ser indexado en Google News es una señal de calidad editorial.
- **Incremento de visibilidad** — Aparecer en la pestaña "Noticias" y en widgets de Google Discover.
- **Posicionamiento SEO transversal** — El tráfico de Google News impulsa señales que benefician el SEO general.
- **Construcción de reputación periodística** — El sello de Google News actúa como respaldo de credibilidad.

---

## 2. Funcionamiento del Algoritmo

El algoritmo de Google News evalúa múltiples dimensiones para determinar qué artículos mostrar y en qué posición.

### 2.1 Relevancia

Google analiza si el contenido coincide con **tendencias actuales** y consultas de búsqueda en tiempo real. Para maximizar la relevancia:

- Cubre temas de tendencia (**trending topics**) dentro de tu nicho.
- Utiliza palabras clave que reflejen el lenguaje de búsqueda actual.
- Relaciona el artículo con eventos en desarrollo.

### 2.2 Actualidad (Freshness)

El contenido reciente posee **prioridad algorítmica** dentro de Google News. El sistema distingue entre:

| Tipo | Ventana de publicación | Prioridad |
|---|---|---|
| Última hora | < 1 hora | Muy alta |
| Hoy | < 24 horas | Alta |
| Últimos 2 días | 24–48 horas | Media |
| Semana actual | 3–7 días | Baja |
| Anterior | > 7 días | Mínima (salvo actualizaciones) |

**Estrategia:** Publica contenido fresco constantemente. Si actualizas un artículo existente, usa `dateModified` en el schema para que Google lo reindexe como actualizado.

### 2.3 Autoridad del Sitio

Se evalúa mediante:

1. **Backlinks** — Cantidad y calidad de enlaces entrantes de sitios con autoridad.
2. **Menciones en medios** — Referencias de otros medios periodísticos.
3. **Antigüedad del dominio** — Los dominios con más de 6–12 meses tienen ventaja.
4. **Confiabilidad** — Historial de cumplimiento con las políticas de Google News.
5. **E-E-A-T (Experience, Expertise, Authoritativeness, Trustworthiness)** — Señales de que el contenido es creado por expertos reales.

### 2.4 Calidad Editorial

Google evalúa:

- **Originalidad** — Contenido único, no copiado ni sindicado sin valor añadido.
- **Claridad** — Redacción profesional, estructura jerárquica (titulares, subtítulos, párrafos cortos).
- **Profundidad** — Cobertura sustancial del tema, no artículos superficiales de 200 palabras.
- **Información verificable** — Fuentes citadas, datos contrastables, enlaces a documentos originales.
- **Autoría** — Artículos firmados por personas reales con biografía verificable.

---

## 3. Requisitos Fundamentales

### 3.1 Dominio Profesional

| Requisito | Especificación mínima | Recomendado |
|---|---|---|
| **HTTPS** | SSL/TLS válido | TLS 1.3, certificado no expirado |
| **Hosting** | Tiempo de actividad > 99.5% | 99.9%+ con SLA |
| **Dominio propio** | .com, .es, .org, etc. | Dominio de nivel superior (TLD) reconocible |
| **Velocidad** | < 3 segundos de carga | < 1.5 segundos (LCP < 2.5s) |
| **Almacenamiento** | SSD básico | NVMe con CDN |

### 3.2 Transparencia y Credibilidad

El sitio debe exponer claramente:

- **Página de contacto** — Correo electrónico, formulario, dirección física (opcional pero recomendada).
- **Autores visibles** — Cada artículo debe mostrar nombre del autor con enlace a su biografía.
- **Fechas de publicación** — Visibles y precisas (día, mes, año; opcionalmente hora).
- **Políticas editoriales** — Página que describa los estándares periodísticos del medio.
- **Información institucional** — Quiénes somos, misión, equipo directivo.
- **Correcciones y transparencia** — Política de corrección de errores y respuesta a lectores.

### 3.3 Contenido Original

Google **prioriza contenido auténtico y periodístico** generado por humanos.

#### Prácticas prohibidas o desaconsejadas:

- **Copy-paste** de otros medios sin valor editorial añadido.
- **Contenido duplicado** total o parcial (incluso interno).
- **Automatización masiva** sin supervisión editorial humana (contenido generado por IA sin revisión).
- **Clickbait** — Titulares engañosos que no reflejan el contenido real.
- **Granjas de contenido** — Sitios diseñados exclusivamente para captar tráfico sin valor periodístico.
- **Artículos traducidos automáticamente** sin revisión humana.

> **Nota:** Google News actualizó sus políticas en 2025–2026 para requerir **revelación explícita** cuando el contenido es generado o asistido por IA. Si utilizas herramientas de IA, debes indicarlo claramente y asegurar supervisión editorial humana.

---

## 4. Arquitectura Profesional del Sitio

### 4.1 Estructura de directorios

```
/
├── noticias/
├── politica/
├── economia/
├── tecnologia/
├── ciencia/
├── cultura/
├── deportes/
├── opinion/
├── autores/
│   ├── juan-perez/
│   ├── maria-garcia/
│   └── ...
├── contacto/
├── sobre-nosotros/
├── politicas-editoriales/
└── correcciones/
```

### 4.2 Buenas prácticas de URLs

| Correcto | Incorrecto |
|---|---|
| `/noticias/impacto-ia-industria` | `/post?id=72829` |
| `/economia/inflacion-2026` | `/article.php?slug=abc123` |
| `/tecnologia/lanzamiento-iphone-18` | `/p=1982` |
| `/autores/juan-perez` | `/author?uid=45` |

**Reglas de oro para URLs:**

1. Usa guiones (`-`) para separar palabras.
2. URLs cortas y descriptivas (3–6 palabras).
3. Incluye la categoría en la ruta.
4. Evita parámetros dinámicos (`?id=`, `&page=`).
5. Sin fechas en la URL (a menos que sea estrictamente necesario para tu CMS).
6. URLs en minúsculas, sin caracteres especiales.

### 4.3 Estructura de página individual

```
┌──────────────────────────────────────┐
│  Header (logo + menú + buscador)     │
├──────────────────────────────────────┤
│  Breadcrumb                          │
│  Inicio > Tecnología > [Artículo]    │
├──────────────────────────────────────┤
│  H1 — Título del artículo            │
│  Autor | Fecha | Tiempo de lectura   │
│  Imagen destacada (con crédito)      │
├──────────────────────────────────────┤
│  Cuerpo del artículo                 │
│  - Introducción (lead)               │
│  - Desarrollo (H2, H3)               │
│  - Citas, datos, multimedia          │
│  - Conclusión                        │
├──────────────────────────────────────┤
│  Compartir en redes                  │
│  Artículos relacionados              │
│  Comentarios (opcional)              │
├──────────────────────────────────────┤
│  Footer — enlaces institucionales    │
└──────────────────────────────────────┘
```

---

## 5. Implementación Técnica

### 5.1 Infraestructura de hosting

| Componente | Requisito mínimo | Recomendado |
|---|---|---|
| **Almacenamiento** | SSD | NVMe |
| **Protocolo** | HTTP/2 | HTTP/3 (QUIC) |
| **SSL** | Let's Encrypt | Certificado OV/EV |
| **CDN** | Opcional | Cloudflare, Fastly, BunnyCDN |
| **Caché** | Server-side | Redis + CDN + Browser |
| **PHP/Node** | Última versión estable | Versión LTS actual |

### 5.2 Configuración de HTTPS

```nginx
# Configuración de seguridad TLS
server {
    listen 443 ssl http2;
    server_name midominio.com;

    ssl_certificate     /etc/ssl/certs/midominio.crt;
    ssl_certificate_key /etc/ssl/private/midominio.key;

    ssl_protocols TLSv1.2 TLSv1.3;
    ssl_ciphers ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256;
    ssl_prefer_server_ciphers on;

    # HSTS (HTTP Strict Transport Security)
    add_header Strict-Transport-Security "max-age=63072000; includeSubDomains; preload";

    # Redirigir HTTP a HTTPS
    error_page 497 https://$host$request_uri;
}
```

### 5.3 Optimización de velocidad

| Técnica | Impacto | Implementación |
|---|---|---|
| **Compresión GZIP/Brotli** | Alto | `gzip on;` en Nginx, Brotli si está disponible |
| **Imágenes WebP + AVIF** | Alto | Convertir al subir, servir con `<picture>` |
| **Lazy loading** | Medio | `loading="lazy"` en imágenes y iframes |
| **Minificación** | Medio | HTML, CSS, JS minificados en build |
| **Caché navegador** | Medio | Cache-Control para recursos estáticos |
| **Preconnect/preload** | Medio | `<link rel="preconnect">` para recursos críticos |
| **Critical CSS** | Alto | Inline CSS crítico, diferir el resto |

**Ejemplo de configuración de caché en Nginx:**

```nginx
location ~* \.(jpg|jpeg|png|gif|ico|webp|avif|css|js|woff2)$ {
    expires 365d;
    add_header Cache-Control "public, immutable";
}

location / {
    # Para contenido HTML: caché corta pero válida
    expires 5m;
    add_header Cache-Control "public, must-revalidate";
}
```

### 5.4 Responsive Design

Google News prioriza sitios con excelente experiencia móvil. Requisitos:

1. **Viewport meta tag** correcto.
2. **Diseño fluido** — CSS Grid / Flexbox, sin dimensiones fijas en píxeles.
3. **Touch targets** — Botones y enlaces de al menos 48×48px.
4. **Tipografía legible** — Tamaño base ≥ 16px en móvil.
5. **Sin intersticiales** — Popups o banners que cubran el contenido.
6. **Mobile-first** — Diseñar primero para móvil y escalar hacia arriba.

**Ejemplo básico:**

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

```css
:root {
    font-size: 16px;
}

body {
    font-size: 1rem;
    line-height: 1.6;
}

@media (min-width: 768px) {
    body {
        font-size: 1.125rem;
    }
}

@media (min-width: 1200px) {
    body {
        font-size: 1.25rem;
    }
}
```

### 5.5 Core Web Vitals para Google News

| Métrica | Bueno | Necesita mejora | Pobre |
|---|---|---|---|
| **LCP** ( Largest Contentful Paint) | ≤ 2.5s | 2.5s – 4.0s | > 4.0s |
| **FID** ( First Input Delay) | ≤ 100ms | 100ms – 300ms | > 300ms |
| **CLS** ( Cumulative Layout Shift) | ≤ 0.1 | 0.1 – 0.25 | > 0.25 |
| **INP** ( Interaction to Next Paint) | ≤ 200ms | 200ms – 500ms | > 500ms |

**Recomendaciones para mejorar Core Web Vitals:**

- **LCP:** Pre-cargar la imagen destacada, servir en WebP/AVIF, usar un CDN.
- **FID/INP:** Diferir JavaScript no crítico, dividir bundles pesados con code splitting.
- **CLS:** Dimensiones explícitas en `<img>` y elementos embebidos, evitar inserciones tardías de anuncios sin espacio reservado.

---

## 6. Sitemap XML

El sitemap XML es el mecanismo principal para que Google News descubra y rastree tus artículos.

### 6.1 Estructura del sitemap de noticias

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9"
        xmlns:news="http://www.google.com/schemas/sitemap-news/0.9">
    <url>
        <loc>https://midominio.com/noticias/impacto-ia-industria</loc>
        <news:news>
            <news:publication>
                <news:name>Nombre del Medio</news:name>
                <news:language>es</news:language>
            </news:publication>
            <news:publication_date>2026-05-11T09:00:00Z</news:publication_date>
            <news:title>El impacto de la IA en la industria durante 2026</news:title>
            <news:keywords>inteligencia artificial, industria, automatización</news:keywords>
        </news:news>
    </url>
    <!-- más URLs -->
</urlset>
```

### 6.2 Buenas prácticas del sitemap de noticias

1. **Incluye solo artículos de los últimos 2 días** — Google News solo indexa contenido reciente. No incluyas artículos antiguos.
2. **URLs canónicas** — Cada artículo debe tener una única URL canónica.
3. **Actualización frecuente** — Genera y actualiza el sitemap cada vez que publiques.
4. **Tamaño máximo** — 50,000 URLs por sitemap (para News, raramente llegas a eso).
5. **Idioma correcto** — Usa códigos ISO 639-1 (`es`, `en`, `fr`, etc.).
6. **Notifica a Google** — Envía el sitemap desde Google Search Console.

### 6.3 Sitemap principal vs sitemap de noticias

```
Sitemap principal (todo el sitio):
https://midominio.com/sitemap.xml

Sitemap específico de noticias:
https://midominio.com/sitemap-news.xml
```

En tu `robots.txt`:

```
Sitemap: https://midominio.com/sitemap.xml
Sitemap: https://midominio.com/sitemap-news.xml
```

---

## 7. robots.txt

El archivo `robots.txt` debe permitir el rastreo de Googlebot-News y Googlebot.

### 7.1 Configuración recomendada

```txt
User-agent: *
Allow: /

# Permitir específicamente a Google News
User-agent: Googlebot-News
Allow: /

# Googlebot general (también rastrea noticias)
User-agent: Googlebot
Allow: /

# Desbloquear archivos CSS/JS para renderizado correcto
User-agent: Googlebot-News
Allow: /wp-content/uploads/
Allow: /assets/

# Sitemaps
Sitemap: https://midominio.com/sitemap.xml
Sitemap: https://midominio.com/sitemap-news.xml
```

### 7.2 Advertencias importantes

- **No bloquees Googlebot-News** en ninguna sección que contenga artículos.
- **Permite CSS y JS** — Google necesita renderizar la página para evaluar la experiencia de usuario.
- **No uses `Disallow: /`** sin una razón muy justificada.
- **Verifica** con el inspector de URLs en Search Console que Googlebot puede acceder.

---

## 8. Structured Data — Schema.org

Los datos estructurados son **obligatorios** para que Google News entienda tu contenido correctamente.

### 8.1 Tipo recomendado: `NewsArticle`

```json
{
    "@context": "https://schema.org",
    "@type": "NewsArticle",
    "headline": "Título completo del artículo",
    "url": "https://midominio.com/noticias/titulo-del-articulo",
    "mainEntityOfPage": {
        "@type": "WebPage",
        "@id": "https://midominio.com/noticias/titulo-del-articulo"
    },
    "image": [
        "https://midominio.com/imagenes/destacada-1200x630.jpg",
        "https://midominio.com/imagenes/destacada-800x450.jpg"
    ],
    "datePublished": "2026-05-11T09:00:00+02:00",
    "dateModified": "2026-05-11T14:30:00+02:00",
    "author": {
        "@type": "Person",
        "name": "Juan Pérez",
        "url": "https://midominio.com/autores/juan-perez",
        "jobTitle": "Periodista de tecnología",
        "sameAs": [
            "https://twitter.com/juanperez",
            "https://linkedin.com/in/juanperez"
        ]
    },
    "publisher": {
        "@type": "Organization",
        "name": "Nombre del Medio",
        "url": "https://midominio.com",
        "logo": {
            "@type": "ImageObject",
            "url": "https://midominio.com/logo.png",
            "width": 600,
            "height": 60
        }
    },
    "description": "Resumen breve del artículo, máximo 160 caracteres. Debe ser atractivo e informativo.",
    "articleBody": "Texto completo del artículo... (no obligatorio pero recomendado)",
    "articleSection": "Tecnología",
    "keywords": ["inteligencia artificial", "industria", "automatización"],
    "wordCount": 850,
    "inLanguage": "es",
    "isAccessibleForFree": true,
    "hasPart": {
        "@type": "WebPageElement",
        "isAccessibleForFree": false,
        "cssSelector": ".premium-content"
    }
}
```

### 8.2 Propiedades obligatorias

| Propiedad | Descripción |
|---|---|
| `@type` | Debe ser `NewsArticle` (o subtipo como `AnalysisNewsArticle`, `OpinionNewsArticle`, `ReportageNewsArticle`, etc.) |
| `headline` | Título del artículo. Máximo 110 caracteres recomendado. |
| `url` | URL canónica del artículo. |
| `image` | Una o más imágenes. Mínimo 1200px de ancho. |
| `datePublished` | Fecha y hora de publicación inicial en ISO 8601. |
| `dateModified` | Fecha de la última modificación sustancial. |
| `author` | Persona real con nombre completo. |
| `publisher` | Organización o medio responsable. |
| `description` | Resumen atractivo para el snippet. |

### 8.3 Tipos adicionales útiles

```json
{
    "@context": "https://schema.org",
    "@type": "ReportageNewsArticle",
    "headline": "Investigación: los costos ocultos de la inteligencia artificial",
    ...
}
```

Otros subtipos permitidos: `AnalysisNewsArticle`, `BackgroundNewsArticle`, `OpinionNewsArticle`, `ReviewNewsArticle`, `ReportageNewsArticle`.

### 8.4 FAQPage (para secciones de preguntas)

```json
{
    "@context": "https://schema.org",
    "@type": "FAQPage",
    "mainEntity": [{
        "@type": "Question",
        "name": "¿Cómo aparecer en Google News?",
        "acceptedAnswer": {
            "@type": "Answer",
            "text": "Necesitas cumplir requisitos técnicos (HTTPS, velocidad), editoriales (contenido original) y estructurales (schema.org, sitemap)."
        }
    }]
}
```

### 8.5 BreadcrumbList (migas de pan)

```json
{
    "@context": "https://schema.org",
    "@type": "BreadcrumbList",
    "itemListElement": [{
        "@type": "ListItem",
        "position": 1,
        "name": "Inicio",
        "item": "https://midominio.com"
    }, {
        "@type": "ListItem",
        "position": 2,
        "name": "Tecnología",
        "item": "https://midominio.com/tecnologia"
    }, {
        "@type": "ListItem",
        "position": 3,
        "name": "Título del artículo"
    }]
}
```

### 8.6 Validación

Usa estas herramientas para validar tu schema:

- **Rich Results Test** de Google: https://search.google.com/test/rich-results
- **Schema.org Validator**: https://validator.schema.org
- **Google Search Console** → Mejoras → Informes de datos estructurados

---

## 9. Google Search Console

Google Search Console es la herramienta central para monitorear y optimizar tu presencia en Google News.

### 9.1 Configuración inicial

1. **Registrar propiedad** — Añade tu dominio como propiedad.
2. **Verificar dominio** — Usa uno de estos métodos:
   - Archivo HTML en la raíz del sitio.
   - Registro TXT en DNS.
   - Proveedor de hosting (si es compatible).
3. **Enviar sitemap** — Ve a "Sitemaps" y añade la URL de tu sitemap.

### 9.2 Reportes específicos para Google News

Dentro de Search Console, enfócate en:

| Reporte | Qué buscar |
|---|---|
| **Rendimiento** | Impresiones, clics, CTR, posición promedio en News. |
| **Cobertura** | URLs indexadas, errores, excluidas, advertencias. |
| **Core Web Vitals** | LCP, FID/INP, CLS — métricas de experiencia de página. |
| **Mejoras** | Datos estructurados válidos, errores de schema. |
| **Inspección de URLs** | Probar URLs específicas para ver si Google puede indexarlas. |

### 9.3 Filtros útiles

En el reporte de Rendimiento, filtra por:

- **Tipo de búsqueda:** "Google News" (específico) o "Web" (general).
- **País:** Para ver rendimiento por región.
- **Dispositivo:** Móvil vs. escritorio vs. tablet.
- **Fecha:** Compara períodos para detectar tendencias.

### 9.4 Acciones frecuentes

- **Semanal:** Revisar nuevos errores de rastreo.
- **Mensual:** Analizar tendencias de CTR y posiciones.
- **Al publicar:** Inspeccionar URL del nuevo artículo.
- **Al actualizar:** Solicitar indexación si no aparece en 24 horas.

---

## 10. Google Publisher Center

El **Google Publisher Center** es el panel de administración para gestionar tu publicación en Google News.

### 10.1 Acceso

URL: https://partnerdash.google.com/partnerdash/d/news

### 10.2 Configuración obligatoria

| Elemento | Requisito | Recomendación |
|---|---|---|
| **Logo** | Formato PNG/SVG, fondo transparente | 600×60px o 400×400px para square |
| **Nombre del medio** | Debe coincidir con el nombre visible en el sitio | Consistente en todo el sitio |
| **Categorías** | Seleccionar secciones que definan la temática | Máximo 5 categorías relevantes |
| **Feed RSS/Atom** | URL del feed principal de noticias | Feed dedicado solo a contenido noticioso |
| **URLs del sitio** | Dominio principal verificado | Incluir subdominios si aplica |

### 10.3 Configuración de feeds

El feed RSS es crítico para que Google News descubra tu contenido rápidamente.

**Estructura de feed RSS recomendada:**

```xml
<?xml version="1.0" encoding="UTF-8"?>
<rss version="2.0"
     xmlns:atom="http://www.w3.org/2005/Atom"
     xmlns:media="http://search.yahoo.com/mrss/"
     xmlns:dc="http://purl.org/dc/elements/1.1/">
    <channel>
        <title>Nombre del Medio</title>
        <link>https://midominio.com</link>
        <description>Descripción del medio periodístico</description>
        <language>es</language>
        <lastBuildDate>Mon, 11 May 2026 09:00:00 +0200</lastBuildDate>
        <atom:link href="https://midominio.com/feed/news.xml" rel="self" type="application/rss+xml"/>

        <item>
            <title>El impacto de la IA en la industria durante 2026</title>
            <link>https://midominio.com/noticias/impacto-ia-industria</link>
            <guid isPermaLink="true">https://midominio.com/noticias/impacto-ia-industria</guid>
            <pubDate>Mon, 11 May 2026 09:00:00 +0200</pubDate>
            <dc:creator>Juan Pérez</dc:creator>
            <category>Tecnología</category>
            <description>Resumen del artículo de máximo 160 caracteres.</description>
            <media:content url="https://midominio.com/imagenes/destacada.jpg" medium="image"/>
        </item>
        <!-- más items -->
    </channel>
</rss>
```

### 10.4 Buenas prácticas en Publisher Center

1. **Mantén los feeds actualizados** — Cada nuevo artículo debe aparecer en el feed inmediatamente.
2. **No incluyas artículos duplicados** en diferentes feeds.
3. **Titulares consistentes** — El título en el feed debe coincidir con el H1 del artículo.
4. **Imágenes en el feed** — Incluye `media:content` para que Google asocie imágenes.
5. **Revisa notificaciones** — Publisher Center puede alertar sobre problemas de cumplimiento.

---

## 11. Producción Editorial

### 11.1 Frecuencia de publicación

| Tipo de medio | Frecuencia mínima | Frecuencia ideal |
|---|---|---|
| Medio generalista | 5–10 artículos/día | 15–30 artículos/día |
| Medio especializado | 3–5 artículos/día | 5–15 artículos/día |
| Blog periodístico | 1–3 artículos/día | 3–7 artículos/día |
| Medio local | 2–5 artículos/día | 5–10 artículos/día |

### 11.2 Tipos de contenido con mejor rendimiento

1. **Noticias de última hora** — Cobertura inmediata de eventos en desarrollo.
2. **Análisis y contexto** — Artículos que explican el "por qué" detrás de la noticia.
3. **Investigaciones originales** — Reportajes con datos propios, entrevistas exclusivas.
4. **Tendencias** — Contenido sobre temas emergentes antes de que sean mainstream.
5. **Informes de datos** — Visualizaciones, estadísticas, rankings.
6. **Entrevistas exclusivas** — Contenido que no se encuentra en ningún otro medio.
7. **Guías y tutoriales** — Contenido práctico con valor duradero.

### 11.3 Estructura de un artículo optimizado para Google News

```
TÍTULO (H1)
- Entre 50–110 caracteres
- Incluir palabra clave principal
- Ser descriptivo, no sensacionalista
- Sin signos de exclamación excesivos

LEAD / ENTRADILLA
- Máximo 2 párrafos
- Responde: ¿Qué? ¿Quién? ¿Cuándo? ¿Dónde? ¿Por qué?
- Engancha sin revelar todo

CUERPO
- Párrafos de 2–4 oraciones máximo
- Subtítulos H2 cada 200–300 palabras
- Listas, datos, citas intercaladas
- Multimedia relevante cada ~400 palabras

CIERRE
- Conclusión o resumen
- Llamada a la acción: leer relacionado, compartir, suscribirse
```

### 11.4 SEO On-Page para noticias

| Elemento | Práctica recomendada |
|---|---|
| **Title tag** | 50–60 caracteres, palabra clave al inicio |
| **Meta description** | 120–160 caracteres, incluir keyword y llamado a la acción |
| **H1** | Único por página, descriptivo |
| **H2/H3** | Incluir variaciones semánticas de la keyword |
| **Alt text** | Describir imágenes con contexto editorial |
| **Internal links** | 2–5 enlaces a artículos relacionados |
| **External links** | 1–3 enlaces a fuentes originales verificables |
| **URL slug** | 3–5 palabras con guiones |

### 11.5 Política de actualización de artículos

- **Artículos de noticias**: Actualizar solo si hay información nueva. Usar `dateModified`.
- **Artículos de análisis**: Se pueden actualizar periódicamente. Añadir nota de "Actualizado el [fecha]".
- **Artículos perennes** (guías): Actualizar cuando cambien los datos. Fecha de publicación original + fecha de revisión.

---

## 12. Factores de Posicionamiento

### 12.1 CTR (Click-Through Rate)

La tasa de clics influye directamente en la visibilidad dentro de Google News.

**Cómo mejorar el CTR:**

1. **Titulares atractivos pero precisos** — Sin clickbait, pero con gancho.
2. **Imágenes destacadas impactantes** — Alta calidad, relevantes al contenido.
3. **Fecha visible** — La actualidad es una señal de relevancia.
4. **Nombre del medio reconocible** — Construir marca para que los usuarios confíen.
5. **Rich snippets** — Datos estructurados correctos para que el snippet sea completo.

### 12.2 Tiempo de Permanencia (Dwell Time)

Google analiza cuánto tiempo permanece el usuario leyendo tu artículo.

**Técnicas para aumentar el tiempo de lectura:**

- Contenido sustancial (800+ palabras para artículos de análisis).
- Multimedia integrada (imágenes, videos, gráficos interactivos).
- Formato escaneable (subtítulos, listas, negritas estratégicas).
- Lectura relacionada al final (mantiene al usuario en el sitio).
- Evitar publicidad intrusiva que haga abandonar.

### 12.3 Freshness (Actualidad)

El contenido reciente tiene prioridad algorítmica. Estrategias:

- Programa publicaciones durante horas de alta actividad (mañana y mediodía).
- Cubre eventos en desarrollo con actualizaciones frecuentes.
- Reindexa artículos actualizados mediante `dateModified`.
- Mantén un flujo constante, evita pausas de más de 48 horas.

### 12.4 Autoridad del Sitio

Factores que construyen autoridad a largo plazo:

- **Backlinks naturales** de otros medios y sitios con autoridad.
- **Menciones en redes sociales** de cuentas verificadas.
- **Citas en otros artículos** — Ser referenciado como fuente.
- **Antigüedad** — La paciencia paga: los sitios con 1+ años tienen ventaja.
- **Consistencia temática** — Un sitio especializado en un nicho tiene más autoridad que uno genérico.

### 12.5 Señales de usuario

| Señal | Impacto | Cómo mejorarla |
|---|---|---|
| **Bounce rate** | Alto | Contenido relevante, buena velocidad, diseño limpio |
| **Páginas por sesión** | Medio | Enlaces internos, artículos relacionados |
| **Repetición de visitas** | Alto | Contenido de calidad constante, newsletter |
| **Compartidos en redes** | Medio | Botones de share visibles, contenido shar cable |
| **Comentarios** | Bajo–Medio | Moderación activa, responder a lectores |

---

## 13. Errores Críticos

### 13.1 Contenido duplicado

```
🚫 NO:
- Republicar el mismo artículo en diferentes URLs
- Usar contenido sindicado sin modificaciones sustanciales
- Tener versiones duplicadas (print, amp, móvil) sin canonical
- Copiar contenido de otros sitios aunque sea parcialmente

✅ SÍ:
- Usar rel="canonical" cuando sea necesario
- Añadir análisis original a contenido sindicado
- Diferenciar claramente versiones del mismo artículo
```

### 13.2 Clickbait y titulares engañosos

```
🚫 NO:
- "Lo que pasó después te sorprenderá"
- Prometer información que el artículo no entrega
- Signos de exclamación excesivos
- Mayúsculas sostenidas en titulares

✅ SÍ:
- Titulares informativos y descriptivos
- La promesa del titular debe cumplirse en el contenido
- Lenguaje claro y directo
```

### 13.3 Lentitud de carga

| Problema | Impacto |
|---|---|
| LCP > 4 segundos | Excluido de Top Stories en móvil |
| FID > 300ms | Mala experiencia, abandono |
| CLS > 0.25 | Penalización en ranking |
| TTFB > 800ms | Rastreo lento, menos páginas indexadas |

### 13.4 Publicidad excesiva

Google News penaliza sitios donde la publicidad interfiere con la experiencia de lectura:

- **Interstitial ads** que cubren el contenido al cargar.
- **Popups** que aparecen antes de poder leer.
- **Ratio contenido/anuncios** desbalanceado (> 30% anuncios).
- **Anuncios entre párrafos** que rompen el flujo de lectura.
- **Auto-play con sonido** extremadamente penalizado.

### 13.5 Automatización masiva sin supervisión

Desde 2025, Google News requiere:

- Revelación explícita de contenido generado o asistido por IA.
- Supervisión editorial humana antes de publicación.
- Responsabilidad del medio sobre la veracidad del contenido generado automáticamente.
- Políticas claras sobre el uso de IA en su sitio.

### 13.6 Falta de transparencia

```
🚫 Penalizable:
- No tener página de contacto
- Autores no identificados o con seudónimos no verificables
- Fechas de publicación ocultas o incorrectas
- Sin políticas editoriales visibles
- Sin información sobre la organización responsable
```

### 13.7 Errores técnicos comunes

| Error | Solución |
|---|---|
| HTTPS roto o caducado | Renovar certificado, forzar redirección 301 |
| Sitemap no actualizado | Generar dinámicamente al publicar |
| Schema markup inválido | Validar con Rich Results Test |
| robots.txt bloqueando Googlebot-News | Verificar reglas de rastreo |
| Canonical incorrecto | Revisar que cada URL tenga canonical propio |

---

## 14. Flujo Profesional de Publicación

### 14.1 Proceso completo

```
┌──────────────────────────────────────────────────────┐
│                     1. INVESTIGACIÓN                  │
│  - Identificar tendencias (Google Trends, redes)      │
│  - Verificar fuentes y datos                          │
│  - Definir enfoque y palabra clave principal          │
├──────────────────────────────────────────────────────┤
│                     2. REDACCIÓN                       │
│  - Escribir titular y lead                            │
│  - Desarrollar cuerpo con estructura jerárquica       │
│  - Incluir citas, datos, multimedia                   │
│  - Revisar y editar                                   │
├──────────────────────────────────────────────────────┤
│                   3. OPTIMIZACIÓN SEO                  │
│  - Title tag y meta description                       │
│  - URL slug optimizado                                │
│  - Alt text en imágenes                               │
│  - Internal / external links                         │
├──────────────────────────────────────────────────────┤
│                  4. METADATA Y SCHEMA                 │
│  - Generar JSON-LD NewsArticle                        │
│  - Verificar con validador                            │
│  - Añadir breadcrumb markup                           │
├──────────────────────────────────────────────────────┤
│                     5. MULTIMEDIA                      │
│  - Imagen destacada (≥1200×630px, WebP/AVIF)          │
│  - Video si aplica                                    │
│  - Infografías, gráficos                              │
├──────────────────────────────────────────────────────┤
│                     6. PUBLICACIÓN                     │
│  - Revisión final (ortografía, datos, fuentes)        │
│  - Publicar en CMS                                    │
│  - Verificar en frontend                              │
├──────────────────────────────────────────────────────┤
│              7. POST-PUBLICACIÓN                       │
│  - Inspeccionar URL en Search Console                 │
│  - Solicitar indexación si es necesario               │
│  - Verificar aparición en Google News (24-48h)        │
│  - Difundir en redes sociales                         │
└──────────────────────────────────────────────────────┘
```

### 14.2 Checklist de pre-publicación

- [ ] Titular revisado y aprobado
- [ ] Lead responde las 5W + H
- [ ] Fuentes verificadas y citadas
- [ ] Datos estructurados insertados y validados
- [ ] Imagen destacada ≥ 1200px de ancho, formato WebP/AVIF
- [ ] Alt text en todas las imágenes
- [ ] URL limpia y descriptiva
- [ ] Canonical configurado
- [ ] Tags/categorías asignadas
- [ ] Artículos relacionados enlazados
- [ ] Meta description personalizada (120–160 caracteres)
- [ ] Core Web Vitals verificados (Lighthouse)
- [ ] Vista previa móvil OK

### 14.3 Post-publicación (primeras 48 horas)

1. **0–1 hora:** Inspeccionar URL en Search Console.
2. **1–6 horas:** Monitorear si aparece en Google News (búsqueda site:midominio.com).
3. **6–24 horas:** Si no indexa, solicitar indexación manual.
4. **24–48 horas:** Analizar primeras impresiones y CTR.
5. **48+ horas:** Evaluar rendimiento y planificar siguiente artículo.

---

## 15. Tecnologías Recomendadas

### 15.1 Frontend

| Tecnología | Ventajas para Google News |
|---|---|
| **Next.js** | SSR/SSG, rendimiento excelente, fácil data estructurada |
| **Astro** | Zero JS por defecto, builds ultrarrápidos, ideal para contenido |
| **Nuxt.js** | Similar a Next.js pero con Vue, buena DX |
| **Eleventy** | SSG rápido, enfoque en contenido, flexibilidad total |

**Requisitos mínimos del frontend:**

- SSR o SSG (no CSR puro).
- Inyección de JSON-LD por página.
- Generación dinámica de sitemap XML.
- Optimización automática de imágenes.
- Soporte para RSS/Atom feeds.

### 15.2 CMS

| CMS | Plugin/recurso para Google News |
|---|---|
| **WordPress** | Yoast SEO, WP RSS agregator, Google News XML Sitemap |
| **Strapi** | Headless + plugin SEO, personalización total |
| **Ghost** | Especializado en publicaciones, SEO out-of-the-box |
| **Sanity** | Headless, estructura flexible, integración con Next.js |

### 15.3 Backend

| Tecnología | Caso de uso |
|---|---|
| **Node.js / Express** | APIs ligeras, SSR con Next.js |
| **Django** | CMS robusto, panel admin potente |
| **Laravel** | CMS en PHP, maduro y con ecosistema |
| **NestJS** | Arquitectura modular, TypeScript nativo |

### 15.4 Bases de Datos

| Base de datos | Mejor para |
|---|---|
| **PostgreSQL** | Datos estructurados, búsqueda (FTS), integridad referencial |
| **MySQL** | CMS tradicionales (WordPress, Laravel) |
| **MongoDB** | Contenido semi-estructurado, escalabilidad horizontal |

### 15.5 Infraestructura

| Servicio | Recomendación |
|---|---|
| **CDN** | Cloudflare, Fastly, BunnyCDN, KeyCDN |
| **Hosting** | VPS (DigitalOcean, Linode, Vultr) o PaaS (Vercel, Netlify) |
| **Caché** | Redis, Varnish |
| **Monitoreo** | Sentry, Datadog, UptimeRobot |

---

## 16. Seguridad y Rendimiento

### 16.1 Seguridad

El sitio debe cumplir con estándares de seguridad básicos:

| Medida | Implementación |
|---|---|
| **HTTPS/TLS 1.3** | Certificado SSL válido, redirección forzada |
| **Firewall** | WAF (Cloudflare, ModSecurity, AWS WAF) |
| **Backups automatizados** | Diarios + semanales, almacenados off-site |
| **Protección anti-DDoS** | Cloudflare, AWS Shield, Akamai |
| **Security headers** | HSTS, X-Frame-Options, CSP, X-Content-Type-Options |
| **Rate limiting** | Limitar peticiones por IP para evitar scraping |
| **2FA** | Autenticación de dos factores para el panel admin |

**Ejemplo de security headers:**

```nginx
add_header X-Frame-Options "SAMEORIGIN" always;
add_header X-Content-Type-Options "nosniff" always;
add_header X-XSS-Protection "1; mode=block" always;
add_header Referrer-Policy "strict-origin-when-cross-origin" always;
add_header Content-Security-Policy "default-src 'self'; img-src 'self' https:; script-src 'self'" always;
```

### 16.2 Rendimiento

| Métrica | Objetivo | Herramienta para medir |
|---|---|---|
| **LCP** | < 2.5s | PageSpeed Insights, Lighthouse |
| **FID/INP** | < 200ms | Chrome User Experience Report |
| **CLS** | < 0.1 | Lighthouse, Search Console |
| **TTFB** | < 500ms | WebPageTest, curl |
| **First Paint** | < 1.0s | Lighthouse |
| **Time to Interactive** | < 3.0s | Lighthouse |

**Estrategias de rendimiento:**

1. **Server-side rendering** para contenido estático.
2. **CDN** con edge caching para assets y HTML.
3. **Imágenes responsivas** con `<picture>`, `srcset`, formatos modernos.
4. **Font-display: swap** para tipografía web.
5. **Preload** recursos críticos (hero image, CSS above-the-fold).
6. **Bundle splitting** para JavaScript (cargar solo lo necesario).
7. **HTTP/2 o HTTP/3** para multiplexación de peticiones.

---

## 17. Monetización

### 17.1 Estrategias de monetización compatibles con Google News

| Estrategia | Compatibilidad | Mejores prácticas |
|---|---|---|
| **Display ads** | Alta | No intrusivos, formato nativo, lazy loading |
| **Programática** | Alta | Google Ad Manager, AdSense, Prebid |
| **Patrocinios** | Alta | Artículos patrocinados etiquetados claramente |
| **Afiliados** | Media | Enlaces de afiliados dentro de contenido relevante |
| **Suscripciones** | Alta | Modelo freemium, contenido exclusivo |
| **Contenido premium** | Alta | Paywall suave (metered), tagged correctamente |

### 17.2 Advertencias sobre monetización

```
⚠️ Google News penaliza:

- Anuncios que cubren el contenido principal
- Popups que aparecen inmediatamente
- Más de 1 anuncio por cada ~300 palabras de contenido
- Anuncios con auto-play de video con sonido
- Páginas con más anuncios que contenido
- Intersticiales que impiden la lectura
```

### 17.3 Suscripciones y paywall

Si implementas paywall:

1. Usa schema.org `isAccessibleForFree` para indicar qué contenido es gratuito.
2. Permite a Google indexar al menos 3–5 artículos completos sin suscripción.
3. Implementa metered paywall (X artículos gratis por mes).
4. Etiqueta correctamente el contenido premium en el sitemap.

```json
"isAccessibleForFree": false,
"hasPart": {
    "@type": "WebPageElement",
    "isAccessibleForFree": false,
    "cssSelector": ".premium-content"
}
```

---

## 18. Métricas y KPIs

### 18.1 KPIs principales

| KPI | Fórmula | Objetivo inicial | Objetivo avanzado |
|---|---|---|---|
| **Impresiones en News** | Search Console | 1,000/mes | 100,000+/mes |
| **Clics desde News** | Search Console | 100/mes | 10,000+/mes |
| **CTR en News** | (Clics / Impresiones) × 100 | > 3% | > 8% |
| **Posición promedio** | Search Console | < 15 | < 5 |
| **Tasa de indexación** | Indexados / Enviados × 100 | > 80% | > 95% |
| **Tiempo en página** | Analytics | > 2 min | > 4 min |
| **Páginas por sesión** | Analytics | > 1.5 | > 3.0 |

### 18.2 Dashboard recomendado

Configura en Google Looker Studio (antes Data Studio) o similar:

```
┌──────────────────────────────────────────────────────────┐
│  DASHBOARD GOOGLE NEWS                                   │
├─────────────────┬──────────────────┬─────────────────────┤
│  Impresiones    │  Clics           │  CTR                │
│  ┌─────────┐   │  ┌─────────┐     │  ┌─────────┐       │
│  │ 45.2K   │   │  │ 3.1K    │     │  │ 6.8%   │       │
│  └─────────┘   │  └─────────┘     │  └─────────┘       │
├─────────────────┴──────────────────┴─────────────────────┤
│  Top 10 artículos por impresiones en News                │
├──────────────────────────────────────────────────────────┤
│  1. /noticias/...       │ 12.4K impressions │ CTR 8.2%  │
│  2. /tecnologia/...     │ 8.7K              │ CTR 5.1%  │
│  3. /economia/...       │ 6.2K              │ CTR 7.3%  │
│  ...                                                    │
├──────────────────────────────────────────────────────────┤
│  Tendencias semanales                                    │
│  ┌──────────────────────────────────────────────────┐   │
│  │  📈 Impressions ▲ 23%  │  📉 CTR ▼ 1.2%        │   │
│  └──────────────────────────────────────────────────┘   │
└──────────────────────────────────────────────────────────┘
```

### 18.3 Reporte mensual

Cada mes, evalúa:

1. **Crecimiento de impresiones** vs. mes anterior.
2. **Artículos con mejor rendimiento** — ¿qué tienen en común?
3. **Tendencias de CTR** — ¿están mejorando o empeorando?
4. **Errores de cobertura** — ¿hay páginas no indexadas?
5. **Core Web Vitals** — ¿hay degradación?
6. **Nuevos backlinks** — ¿está creciendo la autoridad?

---

## 19. Checklist de Lanzamiento

### 19.1 Fase 1 — Preparación (semana 1-2)

- [ ] Registrar dominio profesional.
- [ ] Configurar hosting con SSD/NVMe y CDN.
- [ ] Instalar certificado SSL (HTTPS forzado).
- [ ] Verificar HTTP/2 o HTTP/3 habilitado.
- [ ] Elegir e instalar CMS o framework.
- [ ] Diseñar estructura de directorios (categorías, autores, etc.).
- [ ] Configurar entorno de desarrollo y staging.

### 19.2 Fase 2 — Configuración técnica (semana 2-3)

- [ ] Implementar diseño responsive.
- [ ] Configurar caché (server + browser + CDN).
- [ ] Optimizar imágenes (WebP/AVIF, lazy loading).
- [ ] Configurar compresión GZIP/Brotli.
- [ ] Minificar CSS, JS, HTML.
- [ ] Verificar Core Web Vitals (Lighthouse, PageSpeed).
- [ ] Crear y verificar sitemap XML.
- [ ] Configurar robots.txt.

### 19.3 Fase 3 — Contenido y datos estructurados (semana 3-4)

- [ ] Escribir y publicar 10–20 artículos de prueba (contenido real, no lorem ipsum).
- [ ] Implementar schema.org NewsArticle en cada artículo.
- [ ] Validar datos estructurados con Rich Results Test.
- [ ] Configurar generación dinámica de sitemap news.
- [ ] Crear feeds RSS/Atom.
- [ ] Verificar breadcrumbs markup.

### 19.4 Fase 4 — Registro y configuración en Google (semana 4)

- [ ] Registrar propiedad en Google Search Console.
- [ ] Verificar dominio (TXT record o archivo HTML).
- [ ] Enviar sitemap principal y sitemap de noticias.
- [ ] Solicitar indexación de artículos iniciales.
- [ ] Configurar Google Publisher Center.
- [ ] Subir logo y configurar nombre del medio.
- [ ] Agregar feeds RSS en Publisher Center.
- [ ] Seleccionar categorías.

### 19.5 Fase 5 — Monitoreo inicial (semana 4-6)

- [ ] Monitorear indexación diaria en Search Console.
- [ ] Verificar que los artículos aparecen en Google News.
- [ ] Revisar errores de rastreo y datos estructurados.
- [ ] Analizar primeras impresiones y CTR.
- [ ] Ajustar titulares si es necesario.
- [ ] Publicar contenido nuevo constantemente.

### 19.6 Fase 6 — Crecimiento (mes 2-6)

- [ ] Aumentar frecuencia de publicación gradualmente.
- [ ] Construir backlinks mediante relaciones con otros medios.
- [ ] Optimizar basado en datos de Search Console.
- [ ] Implementar estrategia de redes sociales.
- [ ] Considerar newsletter para retención de audiencia.
- [ ] Evaluar estrategias de monetización.

---

## 20. Recursos Oficiales

### Documentación de Google

| Recurso | URL |
|---|---|
| Google Search Console | https://search.google.com/search-console |
| Google Publisher Center | https://partnerdash.google.com/partnerdash/d/news |
| Políticas de Google News | https://news.google.com/about/publisher-policies |
| Sitemap de noticias | https://developers.google.com/search/docs/crawling-indexing/sitemaps/news-sitemap |
| Datos estructurados NewsArticle | https://developers.google.com/search/docs/appearance/structured-data/article |
| Core Web Vitals | https://web.dev/vitals/ |
| Guía de E-E-A-T | https://developers.google.com/search/docs/fundamentals/creating-helpful-content |
| Schema.org | https://schema.org/NewsArticle |
| Rich Results Test | https://search.google.com/test/rich-results |
| PageSpeed Insights | https://pagespeed.web.dev |

### Herramientas complementarias

| Herramienta | Propósito |
|---|---|
| **Google Trends** | Identificar temas y tendencias de búsqueda |
| **Google Analytics** | Analizar tráfico y comportamiento de usuarios |
| **Google Tag Manager** | Gestionar etiquetas y scripts sin modificar código |
| **Ahrefs / Semrush** | Análisis de backlinks, keywords y competencia |
| **Screaming Frog** | Auditoría técnica SEO, encontrar errores |
| **Lighthouse CI** | Monitoreo automatizado de Core Web Vitals |

---

## Apéndice A: Preguntas Frecuentes

### ¿Cuánto tiempo tarda en aparecer un artículo en Google News?

Normalmente entre 24 y 48 horas después de la publicación, siempre que el sitio cumpla con todos los requisitos técnicos. Sitios con autoridad pueden indexar en cuestión de horas.

### ¿Puedo aparecer en Google News con un sitio nuevo?

Sí, pero es más difícil. Los sitios nuevos sin historial necesitan demostrar consistencia, calidad y transparencia. Se recomienda publicar durante 2–3 meses antes de esperar indexación consistente.

### ¿Google News acepta contenido generado por IA?

Sí, siempre que sea revelado explícitamente, supervisado por humanos, y cumpla con los estándares de calidad editorial. Google actualizó sus políticas en 2025 para requerir transparencia sobre contenido generado o asistido por IA.

### ¿Los artículos en inglés tienen prioridad?

No. Google News es multilingüe. Cada país e idioma tiene su propio índice. La prioridad depende de la relevancia para la audiencia local.

### ¿Puedo tener múltiples medios en el mismo dominio?

No recomendado. Cada medio debe tener su propio dominio o subdominio claramente diferenciado. Google Publisher Center espera una publicación por propiedad verificada.

### ¿El tráfico de Google News cuenta para el SEO general?

Sí, indirectamente. El tráfico, las señales de usuario y los backlinks generados desde Google News contribuyen positivamente al perfil general del sitio.

### ¿Qué hago si mi sitio fue penalizado?

1. Identifica la causa en Publisher Center (notificaciones).
2. Corrige el problema detectado.
3. Solicita revisión desde Publisher Center.
4. Publica contenido de alta calidad durante el período de revisión.
5. Espera 2–4 semanas para la respuesta.

---

## Apéndice B: Glosario

| Término | Definición |
|---|---|
| **SERP** | Search Engine Results Page — página de resultados del buscador |
| **Top Stories** | Sección destacada de noticias en la SERP de Google |
| **Google Discover** | Feed personalizado de contenido en móvil Android y Google App |
| **E-E-A-T** | Experience, Expertise, Authoritativeness, Trustworthiness |
| **LCP** | Largest Contentful Paint — métrica de carga visual |
| **FID** | First Input Delay — métrica de interactividad |
| **INP** | Interaction to Next Paint — métrica de respuesta a interacciones |
| **CLS** | Cumulative Layout Shift — métrica de estabilidad visual |
| **TTFB** | Time to First Byte — tiempo de respuesta del servidor |
| **JSON-LD** | Formato de datos estructurados basado en JSON (recomendado por Google) |
| **Freshness** | Factor algorítmico que prioriza contenido reciente |
| **Canonical** | URL que Google debe considerar como la versión principal de una página |
| **Sitemap** | Archivo XML que lista las URLs del sitio para facilitar el rastreo |
| **Crawl** | Proceso de rastreo que realiza Googlebot para descubrir contenido |
| **Indexación** | Proceso de almacenar y organizar páginas en el índice de Google |
| **Paywall suave** | Modelo de suscripción que permite acceso limitado gratuito |

---

## Apéndice C: Tiempos Estimados por Fase

| Fase | Duración estimada | Resultado esperado |
|---|---|---|
| Preparación técnica | 1–2 semanas | Sitio funcional, rápido, seguro |
| Configuración SEO | 1–2 semanas | Sitemaps, schema, robots.txt |
| Producción de contenido inicial | 2–4 semanas | 20–50 artículos publicados |
| Indexación en Google News | 2–8 semanas | Artículos apareciendo en News |
| Posicionamiento consistente | 3–6 meses | Tráfico orgánico regular desde News |
| Autoridad establecida | 6–12 meses | Visibilidad consistente y crecimiento |

---

> **Nota final:** Esta guía se actualiza según los cambios en las políticas de Google News y las mejores prácticas de SEO. La fecha de la última revisión aparece al inicio del documento. Google modifica sus algoritmos y políticas periódicamente; se recomienda revisar la documentación oficial para mantenerse actualizado.

