# Top Search Perú — Guía de actualización en GitHub y SEO

Este paquete es el **rediseño completo** del sitio, con el **mismo contenido y las mismas
direcciones (URLs)** que el sitio actual. Solo cambian el diseño, la hoja de estilos y
mejoras técnicas de SEO. Por eso, si sigue estos pasos, **no debería perder posición en Google**.

## 1. Antes de tocar nada — respaldo
En GitHub, entre a su repositorio `topsearchsite` y cree un respaldo:
- Opción simple: botón verde **Code → Download ZIP** (guarda una copia del sitio actual).
- Opción git: cree una rama de respaldo `git branch respaldo-antes-facelift`.

## 2. Reemplazar los archivos (manteniendo el mismo repositorio y dominio)
El paquete conserva `CNAME` (topsearch.pe) e incluye `.nojekyll`. Reemplace el contenido
del repo por el de este paquete. Con git en su computadora:

```bash
git clone https://github.com/<su-usuario>/topsearchsite.git
cd topsearchsite
# borre los archivos viejos del sitio (NO borre la carpeta .git)
git rm -r --ignore-unmatch index.html nosotros.html busqueda-*.html contacto.html insights en css images sitemap.xml robots.txt CNAME
# copie aquí TODO el contenido de este paquete (topsearch-site) y luego:
git add .
git commit -m "Facelift 2026: nuevo diseño, hreflang y datos estructurados (mismas URLs)"
git push
```

> Si prefiere no usar la línea de comandos, puede subir los archivos por la web de GitHub
> (arrastrar y soltar), pero es más cómodo hacerlo con git por la cantidad de archivos.

En **Settings → Pages** confirme que el dominio siga siendo `topsearch.pe` y que
**Enforce HTTPS** esté activado. El sitio se actualiza en 1–2 minutos.

## 3. Verificación posterior (5 minutos)
- Abra `https://topsearch.pe` y revise: la intro de entrada, la portada, el menú y WhatsApp.
- Abra 3–4 páginas internas y algún artículo de Insights (ES y EN).
- Revise el conmutador de idioma (English / Español) en varias páginas.

## 4. Por qué NO pierde SEO (lo que se preservó)
- **Las URLs son idénticas.** Cada página vive en la misma dirección (mismo nombre de archivo).
  Esto es lo más importante para conservar el ranking.
- **El contenido y los textos se conservan** (mismos títulos, párrafos y palabras clave).
- **Las etiquetas `canonical` se mantienen** exactamente como estaban.
- **`sitemap.xml` y `robots.txt`** se conservan y se actualizaron.

## 5. Mejoras de SEO que ya incluí en este paquete
- **hreflang ES/EN** en todas las páginas emparejadas: le dice a Google que la versión en
  español y en inglés son la misma página en dos idiomas. Antes NO existía — mejora su
  posicionamiento en búsquedas en inglés.
- **Datos estructurados (JSON-LD):** `ProfessionalService`/`Organization` en todo el sitio y
  `Article` en cada artículo de Insights. Ayuda a que Google entienda la firma y muestre
  resultados enriquecidos.
- **Open Graph / Twitter Cards:** al compartir un enlace por WhatsApp, LinkedIn o email, se
  verá con título, descripción y logo.
- **Sitio más liviano y rápido** (una sola hoja de estilos, sin recursos pesados heredados).
  La velocidad es factor de ranking, sobre todo en móviles.
- **`sitemap.xml` con alternantes de idioma** para que Google indexe ambos idiomas.

## 6. Acciones recomendadas DESPUÉS de publicar (para reforzar posición)
1. **Google Search Console** (search.google.com/search-console): verifique el dominio,
   envíe `https://topsearch.pe/sitemap.xml` y pida "Inspección de URL → Solicitar indexación"
   de la home. Repita en **Bing Webmaster Tools**.
2. **Perfil de Empresa de Google (Google Business Profile):** cree/actualice la ficha de
   "Top Search Perú" en San Isidro. Es lo que más mueve búsquedas locales tipo
   "headhunter Perú", "executive search Lima".
3. **Backlinks de autoridad:** pida a **InterSearch Worldwide** que el enlace al miembro de
   Perú apunte a topsearch.pe; enlace el sitio desde su perfil de **LinkedIn** (empresa y
   personal) y desde su bio de columnista en **Diario Gestión**.
4. **Descripciones (meta description) únicas** en las páginas que aún no tienen: cada una con
   una frase que incluya la palabra clave del servicio.
5. **Publicar Insights con constancia** (ya tiene una buena base): contenido fresco y
   enlazado internamente es una señal fuerte para Google.
6. **Eliminar `images/hero-video.mp4`** si ya no lo usa: la nueva portada usa una imagen fija
   (`images/hero-bulb.jpg`), así que ese video de 1.6 MB ya no es necesario y aligera el sitio.
7. **Alt text descriptivo** en imágenes nuevas que agregue (p. ej. "Socios de Top Search Perú").
8. Revise **Core Web Vitals** en Search Console tras unos días.

## 7. Una nota importante sobre el menú de Servicios
Mantuve **dos páginas separadas**: "Búsqueda de Ejecutivos" y "Búsqueda de Directorios",
con sus dos enlaces en el menú. Aunque en la vista previa (que era de una sola página) se
podían unir, en el sitio real **ambas páginas están indexadas en Google y tienen contenido
distinto**. Unirlas en una sola dejaría una de ellas "huérfana" y se perdería ese ranking.
Si aun así quiere unirlas, se hace correctamente con una **redirección 301** de una hacia la
otra para no perder posición — dígame y lo preparamos.

---
*Preparado para Armando Cavero G. — Top Search Perú · Miembro exclusivo de InterSearch Worldwide.*
