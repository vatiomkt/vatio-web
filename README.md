# VATIO · Sitio web

Sitio de VATIO, agencia creativa en Medellín: servicios, Índice VATIO, planes y medición gratis.
Es HTML estático y no necesita build.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página completa |
| `404.html` | Página de error ("0 W") |
| `favicon.svg` | Ícono de la pestaña del navegador |
| `apple-touch-icon.png` | Ícono cuando guardan la web en el celular |
| `og.png` | Imagen que sale al compartir el link por WhatsApp o redes |
| `robots.txt`, `sitemap.xml` | Para que Google encuentre la página |
| `_headers` | Cabeceras de seguridad de Cloudflare Pages |

## Publicar (primera vez)

### 1. GitHub
1. Crea en github.com un repositorio nuevo llamado `vatio-web`. Puede ser **privado**.
2. Entra a **Add file → Upload files**.
3. Arrastra todos los archivos de esta carpeta, no la carpeta en sí, y luego **Commit changes**.

### 2. Cloudflare Pages
1. En Cloudflare entra a **Workers & Pages → Create → Pages → Connect to Git**.
2. Conecta GitHub y elige el repositorio `vatio-web`.
3. Configuración:
   - Framework preset: **None**
   - Build command: *(vacío)*
   - Build output directory: `/`
4. Dale a **Save and Deploy**. En menos de un minuto queda en `vatio-web.pages.dev`.

### 3. Dominio vatiomkt.com
1. En Cloudflare entra a **Domain Registration → Register Domains**, busca `vatiomkt.com` y cómpralo.
2. Vuelve al proyecto de Pages y entra a **Custom domains → Set up a domain**.
3. Escribe `vatiomkt.com` y repite el paso con `www.vatiomkt.com`.
4. El candado (HTTPS) se activa solo.

### 4. Correo hola@vatiomkt.com
En el dominio, entra a **Email → Email Routing**, crea `hola@vatiomkt.com` y haz que reenvíe a tu Gmail.

## Hacer cambios después
Sube el archivo nuevo a GitHub con el mismo nombre. Cloudflare publica el cambio solo, en 1 minuto.

## Si el dominio no es vatiomkt.com
Busca `vatiomkt.com` en `index.html`, `robots.txt` y `sitemap.xml` y cámbialo por el dominio nuevo.
