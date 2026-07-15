# KaphiGames

> Plataforma de comercio electrónico en producción, diseñada, desarrollada y mantenida íntegramente por mí, con clientes reales, ventas activas y evolución continua basada en necesidades del negocio.

![Portada](img/logo_social_kaphigames_1.webp)

## 0. Estado del Proyecto

| Aspecto | Detalle |
|----------|----------|
| Estado | En producción |
| Tipo de proyecto | Producto propio |
| Clientes reales | Sí |
| Ventas activas | Sí |
| Productos publicados | +1.400 |
| Recursos multimedia | +70.000 imágenes en Amazon S3 |
| Infraestructura | VPS + Cloudflare + AWS (S3 y CloudFront) |
| Tecnologías principales | WordPress, WooCommerce, JetEngine, PHP, JavaScript |
| Mantenimiento | Evolución y mejora continua |

---

## 1. Resumen

KaphiGames es una plataforma de comercio electrónico desarrollada sobre WordPress y WooCommerce, creada con el objetivo de construir una solución escalable, optimizada y fácil de administrar.

Como fundador y responsable técnico del proyecto, participé en todo el ciclo de vida de la plataforma, incluyendo:

- Diseño de arquitectura.
- Desarrollo de funcionalidades.
- Infraestructura cloud.
- Optimización de rendimiento.
- SEO técnico.
- Mantenimiento y mejora continua.

El proyecto ha servido como un entorno de producción real para aplicar conocimientos de desarrollo web, infraestructura, optimización de rendimiento y SEO técnico, enfrentando desafíos propios de una plataforma con clientes reales y evolución continua basada en necesidades del negocio.

Actualmente, la plataforma se encuentra operativa en producción, gestionando un catálogo de más de **1.400 productos**, más de **70.000 recursos multimedia almacenados en Amazon S3** y atendiendo clientes reales, permitiendo validar decisiones técnicas y mejoras continuas sobre un producto en funcionamiento.


---

## 2. Objetivos del proyecto

- Construir una plataforma e-commerce mantenible y escalable.
- Gestionar un catálogo extenso de productos mediante estructuras dinámicas.
- Mejorar la velocidad de carga y experiencia de usuario.
- Implementar una infraestructura utilizando Cloudflare y AWS.
- Aplicar prácticas de SEO técnico para mejorar la indexación y visibilidad del sitio.
- Incorporar mejoras continuas basadas en métricas reales de uso y rendimiento.

---

## 3. Mi rol

Durante el desarrollo del proyecto fui responsable de:

| Área | Responsabilidades |
|------|-------------------|
| Arquitectura | Diseño de la solución y toma de decisiones técnicas |
| Desarrollo | WordPress, Elementor, WooCommerce, PHP, JavaScript y CSS |
| Infraestructura | Cloudflare, Amazon S3, CloudFront, VPS |
| Optimización | Rendimiento, WPO y Core Web Vitals |
| SEO Técnico | Search Console, Sitemap, indexación y estructura SEO |
| Operación | Mantenimiento, monitoreo y mejora continua |
| Producto | Priorización y evolución funcional |

---

## 4. Arquitectura de la solución

```text
Usuario
│
├── HTML / PHP
│       ↓
│   Cloudflare (DNS + Proxy + SSL + Caché)
│       ↓
│   VPS (WordPress + WooCommerce + JetEngine)
│
└── Imágenes
        ↓
    CloudFront (CDN)
        ↓
    Amazon S3
```

### 4.1 Componentes principales

- **Cloudflare**
  - DNS
  - SSL
  - Caché y optimización

Principalmente para seguridad y caché HTML.

- **WordPress + WooCommerce + JetEngine**
  - Gestión del catálogo
  - Administración del contenido
  - Comercio electrónico

Gestión de contenido dinámico, Custom Post Types y Custom Fields. 

- **Amazon S3**
  - Almacenamiento de recursos estáticos.

Almacenamiento de contenido multimedia para optimizar recursos de Hosting.

- **CloudFront**
  - Distribución global de recursos.
  - Reducción de tiempos de carga.

Distribución y velocidad del sitio.

---

## 5. Tecnologías utilizadas

| Categoría | Tecnologías |
|-----------|-------------|
| CMS | WordPress |
| E-commerce | WooCommerce |
| Constructor Visual | Elementor |
| Contenido Dinámico | JetEngine |
| Desarrollo | PHP, JavaScript, CSS |
| Infraestructura | Cloudflare, Amazon S3, CloudFront |
| SEO | Rank Math, Google Search Console |

---

## 6. Principales desafíos técnicos

### 6.1 Gestión de un catálogo extenso

La plataforma debía administrar más de mil productos manteniendo una estructura organizada y fácilmente mantenible.

#### Solución

- Uso de estructuras dinámicas mediante JetEngine.
- Organización mediante categorías y etiquetas.
- Automatización de proceso de compra.

---

### 6.2 Optimización de rendimiento

El crecimiento del catálogo y la cantidad de recursos estáticos generaban desafíos relacionados con la velocidad de carga.

#### Solución

- Hosting VPS con LiteSpeed Cache.
- Implementación de Cloudflare.
- Optimización de imagenes: Reescalado + Transformación a WebP.
- Recursos estáticos hacia Amazon S3.
- Distribución mediante Amazon CloudFront.
- Optimización continua de imágenes y recursos.

---

### 6.3 SEO técnico

La plataforma presentó desafíos relacionados con la gestión de un gran volumen de URLs, indexación de productos y resolución de problemas de contenido duplicado y URLs canónicas.

#### Solución

- Configuración de Rank Math SEO.
- Optimización de sitemap XML.
- Análisis y monitoreo mediante Google Search Console.
- Revisión de enlaces permanentes y URLs canónicas.
- Implementación de mejoras iterativas basadas en métricas de indexación.

---

### 6.4 Evolución continua del producto

La plataforma requiere mejoras constantes basadas en necesidades reales del negocio.

#### Solución

- Desarrollo de funcionalidades personalizadas.
- Mantenimiento continuo y resolución de incidencias.

---

## 7. Rendimiento y optimización web

El crecimiento del catálogo, la utilización de contenido dinámico mediante WooCommerce y JetEngine, junto con la gran cantidad de recursos multimedia, hicieron necesario implementar una estrategia de optimización continua para mantener una experiencia de usuario fluida.

### 7.1 Principales optimizaciones implementadas

- Implementación de Cloudflare para proxy, caché y optimización del tráfico.
- Configuración de LiteSpeed Cache para optimización de páginas y recursos.
- Migración de recursos estáticos hacia Amazon S3.
- Distribución de contenido mediante Amazon CloudFront.
- Conversión y optimización de imágenes a formato WebP.
- Evaluación de rendimiento mediante Lighthouse para identificar oportunidades de mejora.

### 7.2 Métricas de referencia

| Métrica | Escritorio | Móvil |
|----------|-------------|--------|
| Performance | 92 | ~70 |
| First Contentful Paint | 0.8 s | 3.0 s |
| Largest Contentful Paint | 1.5 s | 5.7 s |
| Total Blocking Time | 100 ms | 20 ms |
| Cumulative Layout Shift | 0.001 | 0 |

### 7.3 Resultados obtenidos

- Mejoras significativas en velocidad de carga y distribución de recursos.
- Reducción del consumo de almacenamiento y ancho de banda del servidor principal mediante Amazon S3.
- Mejor experiencia de usuario en escritorio y dispositivos móviles.
- Infraestructura preparada para soportar el crecimiento continuo del catálogo y del tráfico.

![PageSpeed Desktop](img/metrica_pagespeed.png)

---

## 8. Resultados

- Plataforma actualmente en producción.
- Más de **1.400 productos publicados**.
- Más de **70.000 recursos multimedia almacenados en Amazon S3**.
- Plataforma operando en producción con clientes reales y ventas activas.
- Implementación de infraestructura cloud mediante AWS.
- Obtención de métricas favorables de rendimiento.
- Habilitación de campañas publicitarias dirigidas directamente al sitio web.
- Reducción de la dependencia de canales externos para la operación del negocio.
- Optimización continua basada en métricas reales.
- Mejora progresiva en rendimiento e indexación.

---

## 9. Impacto del proyecto

La creación de la plataforma permitió centralizar la operación del negocio y reducir la dependencia de canales externos, habilitando nuevas posibilidades de crecimiento y administración.

Entre los principales impactos destacan:

- Plataforma actualmente operando en producción con clientes reales.
- Incremento de ventas pasivas mediante automatización y disponibilidad permanente.
- Posibilidad de realizar campañas publicitarias dirigidas directamente hacia el sitio web.
- Mayor capacidad de administración y escalabilidad respecto a la operación previa basada principalmente en redes sociales.
- Obtención de métricas reales de uso y comportamiento para orientar futuras mejoras.

---

## 10. Galería

### Página principal

![Home](img/pagina_principal.png)

---

### Página de producto

![Producto](img/pagina_producto.png)

---

### Search Console

![Search Console](img/rendimiento_search_console.png)

---

### AWS S3

![Amazon S3](img/metrica_aws_s3.png)

---

## 11. Aprendizaje

Este proyecto me permitió profundizar conocimientos en:

- Desarrollo WordPress y WooCommerce.
- Desarrollo de soluciones personalizadas orientadas a necesidades reales del negocio.
- Infraestructura cloud utilizando AWS.
- Optimización de rendimiento y WPO.
- SEO técnico e indexación.
- Desarrollo y mantenimiento de productos en producción.
- Toma de decisiones basada en métricas reales.
- Priorización y evolución continua de un producto digital.
- Gestión integral de un producto digital, desde infraestructura hasta evolución funcional.

---

## 12. Próximos pasos

- Continuar optimizando rendimiento y SEO técnico.
- Mejorar procesos de automatización y administración.
- Implementar nuevas funcionalidades orientadas a la experiencia de usuario.
- Escalar la plataforma para soportar un crecimiento significativo del catálogo.
- Continuar iterando el producto mediante análisis de métricas reales.

---

## 13. Contenido del repositorio

Este repositorio corresponde a un caso de estudio técnico y no incluye el código fuente completo del proyecto, debido a que la plataforma se encuentra en producción y contiene configuraciones e implementaciones específicas del negocio.

El objetivo es documentar la arquitectura, decisiones técnicas, desafíos y aprendizajes obtenidos durante el desarrollo y mantenimiento de la plataforma.

---

## 14. Enlaces

Sitio web: https://kaphigames.com
LinkedIn: https://www.linkedin.com/in/cristobal-sanchez-orellana/
GitHub: https://github.com/CrisKaphiri
