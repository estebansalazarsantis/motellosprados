# Motel Los Prados — Sitio web estático

Primera versión lista para publicar con **GitHub Pages**. No requiere instalación, base de datos, Node.js ni frameworks.

## Archivos
- `index.html`: estructura, textos, posicionamiento SEO y enlaces de contacto.
- `styles.css`: diseño adaptable a celulares, tablets y computador.
- `script.js`: menú móvil, filtros fotográficos y ampliación de imágenes.
- `assets/`: fotografías optimizadas en WebP y logo original.
- `favicon.png`: icono del sitio.

## Ver en el computador
Abre `index.html` en el navegador. Opcionalmente ejecuta `python -m http.server 8000` desde esta carpeta para probar en `http://localhost:8000`.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub (por ejemplo, `motel-los-prados`).
2. Sube **el contenido de esta carpeta directamente a la raíz** del repositorio (no la carpeta contenedora).
3. En **Settings → Pages**, selecciona **Deploy from a branch**, rama **main** y carpeta **/(root)**. Guarda.
4. GitHub mostrará el enlace de prueba, similar a `https://USUARIO.github.io/motel-los-prados/`.
5. Comprueba versión móvil, imágenes, galería, botón de llamada y mapa.

## Vincular motellosprados.cl más adelante
Antes de cambiar DNS, verifica que el dominio esté registrado y bajo tu control.
1. En **Settings → Pages → Custom domain**, ingresa `motellosprados.cl` y guarda. GitHub creará/configurará CNAME del sitio.
2. En el proveedor del dominio, configura los **registros A** para el dominio raíz `@` con las IP de GitHub Pages vigentes de su documentación; habitualmente son:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
3. Para `www`, crea un registro **CNAME** que apunte a `USUARIO.github.io` (sustituir USUARIO por el titular real de GitHub).
4. Cuando DNS se haya propagado, activa **Enforce HTTPS** si GitHub lo permite.
5. Se recomienda verificar el dominio en GitHub para evitar reclamaciones de subdominio. Revisa la documentación actual: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

**Importante:** No creamos un archivo `CNAME` preconfigurado para no interferir con la etapa inicial de pruebas del sitio. Los metadatos `og:url`, `og:image` y el marcado estructurado ya anticipan el dominio final: se verán plenamente correctos una vez asociado.

## Información pendiente por confirmar antes de lanzar
- Tarifas y modalidades, si se quiere incluir una sección de precios.
- Horarios reales de atención y servicios/instalaciones concretos.
- Si habrá WhatsApp comercial y cuál es su número (por ahora se utiliza llamada al número indicado).
- Ubicación exacta del pin de Google Maps antes de hacer publicidad.
- Autorización de uso de todas las fotografías enviadas.

No se publicaron tarifas, estrellas, valoraciones, promesas de servicios u horarios sin respaldo.

## Imágenes
Se conservaron sus escenas originales; las fotos seleccionadas se procesaron suavemente para mantener sus colores y se convirtieron a WebP para acelerar la carga. La galería es adaptable y recorta visualmente mediante CSS sin destruir las fotos originales.
