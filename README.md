# Tajana Fitness — sitio web

Sitio estático (HTML + CSS + JS puro, sin frameworks ni pasos de compilación).
Eso significa que no hay que instalar nada raro: se abre, se edita y se sube tal cual.

## Estructura

```
tajana-fitness/
├── index.html        → todo el contenido y las 3 secciones
├── css/styles.css     → estilos y colores
├── js/script.js       → menú mobile, efecto de scroll, año del footer
├── assets/
│   ├── logo.webp
│   └── hero.webp
└── README.md
```

## 1. Verlo en tu máquina

1. Abrí la carpeta `tajana-fitness` en VS Code (`File → Open Folder…`).
2. Instalá la extensión **Live Server** (ícono de extensiones a la izquierda, buscar "Live Server", instalar).
3. Click derecho sobre `index.html` → **Open with Live Server**. Se abre el navegador con el sitio.
4. Cada vez que guardes un cambio, se refresca solo.

## 2. Subirlo a GitHub

Desde la terminal, parado en la carpeta `tajana-fitness`:

```
git init
git add .
git commit -m "Primera versión del sitio"
```

Después creá un repositorio vacío en GitHub (sin README, sin .gitignore) y conectalo:

```
git remote add origin https://github.com/TU-USUARIO/tajana-fitness.git
git branch -M main
git push -u origin main
```

## 3. Publicarlo en Vercel

Como ya tenés Vercel conectado a tu cuenta de GitHub:

1. En vercel.com → **Add New → Project**.
2. Elegí el repo `tajana-fitness`.
3. Framework Preset: dejalo en **Other** (es HTML plano, no necesita build).
4. **Deploy**. En un minuto tenés una URL pública tipo `tajana-fitness.vercel.app`.

A partir de acá, cada vez que hagas `git push`, Vercel actualiza el sitio solo.

## 4. Qué falta completar

Busqué "TAJANA FITNESS" pero no encontré una ficha pública con los datos exactos, así que el
sitio quedó con **contenido de relleno marcado con comentarios `<!-- COMPLETAR: ... -->`** en
`index.html`. Los puntos pendientes son:

- Bajada/descripción corta de cada área (fitness, taekwondo, spa)
- Horarios reales de fitness y de taekwondo (por franja etaria si corresponde)
- Nombre y especialidad del profe de fitness
- Nombre y grado del profe de taekwondo
- Zonas y precios de depilación láser + packs
- Promos vigentes y próximas fechas/turnos del spa
- Dirección, teléfono/WhatsApp e Instagram para el pie de página
