# Centro Arraigo — Sitio web

Sitio estático (HTML/CSS/JS puro, sin dependencias) para el centro de bienestar y salud mental de Martin Travella.

## Estructura

```
centro-arraigo/
├── index.html      → Página principal
├── blog/
│   └── como-mejorar-habilidades-sociales-adolescentes.html
└── README.md
```

## Pendientes antes de publicar

1. **Web3Forms**: ir a https://web3forms.com, ingresar el correo donde quieren recibir las consultas y copiar la Access Key. En `index.html`, reemplazar `TU_ACCESS_KEY_AQUI` por esa clave.
2. **Foto de Martin**: reemplazar el placeholder en la sección "Quién atiende".
3. **Dirección del centro**: actualizar en la sección de contacto y en el Schema.org del `<head>`.
4. **Dominio**: cuando tengan el dominio (verificar disponibilidad en https://nic.cl), actualizar las URLs `centroarraigo.cl` en los meta tags de ambas páginas.

## Cómo publicar en GitHub + Vercel (15 minutos)

### Paso 1 — Subir a GitHub
1. Crear cuenta en https://github.com (si no tienen).
2. Crear un repositorio nuevo llamado `centro-arraigo` (público o privado, da igual).
3. En la página del repo, usar **"uploading an existing file"** y arrastrar `index.html`, la carpeta `blog/` y este README. Confirmar con "Commit changes".

### Paso 2 — Conectar Vercel
1. Crear cuenta en https://vercel.com usando **"Continue with GitHub"**.
2. Clic en **"Add New → Project"** y seleccionar el repositorio `centro-arraigo`.
3. No cambiar ninguna configuración (Vercel detecta que es un sitio estático). Clic en **"Deploy"**.
4. En ~30 segundos el sitio queda publicado en una URL tipo `centro-arraigo.vercel.app`, con HTTPS automático.

### Paso 3 — Dominio propio (opcional, recomendado para SEO)
1. Comprar el dominio en https://nic.cl (~$10.000 CLP/año).
2. En Vercel: Project → Settings → Domains → agregar `centroarraigo.cl`.
3. Vercel indica los registros DNS a configurar en NIC Chile. Se propagan en algunas horas.

### Actualizaciones futuras
Cada vez que se edite un archivo en GitHub (se puede hacer desde el navegador con el lápiz ✏️), Vercel republica el sitio automáticamente en segundos.

## SEO post-publicación

- Dar de alta el sitio en **Google Search Console** (https://search.google.com/search-console) y solicitar la indexación.
- Crear el perfil de **Google Business Profile** del centro (clave para aparecer en búsquedas locales "psicólogo + comuna").
- Publicar 1–2 artículos de blog al mes apuntando a búsquedas reales de los clientes.
