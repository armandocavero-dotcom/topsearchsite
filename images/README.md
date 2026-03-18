# Top Search Perú - Sitio Web Estático

## Estructura del sitio
```
topsearch-site/
├── index.html              ← Página de inicio (español)
├── nosotros.html           ← Equipo / Armando, Guillermo, Fernanda
├── busqueda-ejecutivos.html
├── busqueda-directorios.html
├── contacto.html
├── css/
│   └── style.css
├── images/                 ← AQUÍ VAN LAS IMÁGENES (ver abajo)
│   ├── logo-top-search.png
│   ├── intersearch-badge.png
│   ├── hero-video.mp4
│   ├── busqueda-ejecutivos.jpg
│   ├── busqueda-directorios.jpg
│   ├── armando-cavero.jpg
│   ├── guillermo-van-oordt.jpg
│   └── fernanda-cavero.jpg
└── en/                     ← Versión en inglés (pendiente)
    └── index.html
```

## PASO 1: Descargar las imágenes de tu sitio actual

Abre cada URL en tu navegador, haz clic derecho → "Guardar imagen como..." 
y guárdala en la carpeta `images/` con el nombre indicado:

| Guardar como | URL para descargar |
|---|---|
| `logo-top-search.png` | https://topsearch.pe/wp-content/uploads/2024/08/final-logo-top-search-3.png |
| `intersearch-badge.png` | https://topsearch.pe/wp-content/uploads/2024/09/Memeber-of-InterSearch-300x64.png |
| `hero-video.mp4` | https://topsearch.pe/wp-content/uploads/2024/08/1-1.mp4 |
| `busqueda-ejecutivos.jpg` | https://topsearch.pe/wp-content/uploads/2024/09/topsearch-1024x902.jpg |
| `busqueda-directorios.jpg` | https://topsearch.pe/wp-content/uploads/2024/09/AdobeStock_814784513-scaled-600x338.jpeg |
| `armando-cavero.jpg` | https://topsearch.pe/wp-content/uploads/2024/08/armando-1.jpg |
| `guillermo-van-oordt.jpg` | https://topsearch.pe/wp-content/uploads/2024/08/Guillermo-van-Oordt-I.jpg |
| `fernanda-cavero.jpg` | https://topsearch.pe/wp-content/uploads/2024/08/FERNANDA-CAVERO-600.jpg |

## PASO 2: Optimizar imágenes (recomendado para GitHub Pages)

Para reducir el peso, puedes usar https://squoosh.app (gratis):
1. Abre squoosh.app
2. Arrastra cada imagen JPG/PNG
3. En el panel derecho, selecciona "WebP" o "MozJPEG"
4. Ajusta calidad a 80%
5. Descarga y reemplaza

Para el VIDEO (hero-video.mp4): Si pesa más de 10MB, súbelo a YouTube
como "no listado" y reemplaza el <video> en index.html por un iframe de YouTube.

## PASO 3: Subir a GitHub Pages (GRATIS)

1. Ve a https://github.com y crea una cuenta (si no tienes)
2. Crea un nuevo repositorio llamado: `topsearch-site` (público)
3. Sube todos los archivos (puedes arrastrarlos directamente en la web)
4. Ve a Settings → Pages
5. En "Source" selecciona: "Deploy from a branch" → branch: main → /(root)
6. Espera 2-3 minutos
7. Tu sitio estará en: https://TU-USUARIO.github.io/topsearch-site/

## PASO 4 (opcional): Dominio personalizado

Si quieres que topsearch.pe apunte a GitHub Pages:
1. En Settings → Pages → Custom domain, escribe: www.topsearch.pe
2. En tu registrador de dominio, agrega un registro CNAME:
   - Nombre: www
   - Valor: TU-USUARIO.github.io
3. Espera propagación DNS (hasta 24 horas)

## Botón de WhatsApp
Ya está incluido en todas las páginas. Aparece fijo en la esquina inferior
derecha con animación de pulso. Enlaza a: +51 934 912 540
