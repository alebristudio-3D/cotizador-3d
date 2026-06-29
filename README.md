# Cotizador 3D — Alebri Studio

Calculadora de cotizaciones para impresión 3D con exportación a PDF y PWA instalable.

## Deploy en GitHub Pages (5 minutos)

### Opción A — Nuevo repositorio (recomendado)

1. Ve a [github.com/new](https://github.com/new)
2. Nombre del repo: `cotizador-3d` (o el que prefieras)
3. Deja en **Public**, sin inicializar con README
4. Click en **Create repository**

5. Sube los archivos desde tu computadora:
   - En la página del repo, click en **uploading an existing file**
   - Arrastra todos los archivos de esta carpeta: `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`
   - Commit changes

6. Activa GitHub Pages:
   - Settings → Pages
   - Source: **Deploy from a branch**
   - Branch: `main` / `(root)`
   - Save

7. En ~1 minuto tu app estará en:
   `https://TU-USUARIO.github.io/cotizador-3d/`

---

### Opción B — Subir al repo existente `alebristudio-3d`

Si ya tienes el repo `alebristudio-3d.github.io`:

```bash
# En tu máquina, dentro del repo clonado
cp -r cotizador3d/* .
git add .
git commit -m "Add: cotizador 3D"
git push
```

La app quedaría en:
`https://alebristudio-3d.github.io/cotizador-3d/`
(si la pones en una subcarpeta `cotizador-3d/`)

---

## PWA — Instalar como app en celular

Una vez que esté en GitHub Pages:

1. Abre la URL en Chrome (Android) o Safari (iOS)
2. Android: menú ⋮ → **Agregar a pantalla de inicio**
3. iOS: botón compartir → **Agregar a inicio**

La app funciona **sin internet** después de la primera carga.

---

## Archivos

| Archivo | Descripción |
|---------|-------------|
| `index.html` | App completa (una sola página) |
| `manifest.json` | Configuración PWA |
| `sw.js` | Service worker (caché offline) |
| `icon-192.png` | Ícono para homescreen |
| `icon-512.png` | Ícono splash screen |

---

## Personalización rápida

Abre `index.html` y busca estos valores por defecto:

```
cfgNombre  → "Alebri Studio"
cfgWA      → "522217522601"
cfgCiudad  → "Puebla, México"
cfgHora    → 35   (costo hora máquina MXN)
cfgMargen  → 60   (% margen ganancia)
cfgMin     → 80   (mínimo de cobro MXN)
```

Todo se puede cambiar también desde la pestaña **Configuración** dentro de la app.

---

Alebri Studio · Puebla, México
