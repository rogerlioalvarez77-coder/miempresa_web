# MIEMPRESA — Sitio Web

Sitio web de una sola página, listo para desplegarse en **GitHub Pages**.

---

## 📁 Archivos del proyecto

| Archivo | Descripción |
|---|---|
| `index.html` | ✅ **Este es el archivo que subes a GitHub Pages.** Contiene todo (fuentes, estilos, scripts) en un solo archivo. |
| `MIEMPRESA.dc.html` | Archivo fuente editable en el editor online. No es necesario para producción. |

---

## ✏️ Cómo hacer cambios en `index.html`

Abre `index.html` con **VS Code** (recomendado) o cualquier editor de texto.
Usa **Ctrl + H** (Windows/Linux) o **Cmd + H** (Mac) para buscar y reemplazar.

---

### 📞 Cambiar teléfono

Busca: `+503 7191-0611`
Hay **2 apariciones** — reemplaza ambas con tu número real.

También busca el enlace `tel:+50371910611` y reemplázalo con tu número sin `+` ni espacios (ej: `tel:+50312345678`).

---

### 📱 Cambiar el número de WhatsApp

El número de WhatsApp está en varios enlaces del tipo:
```
https://wa.me/50371910611?text=...
```
Busca `50371910611` — hay varias apariciones.
Reemplaza todas por tu número con código de país, sin `+` ni espacios.
Ej: El Salvador → `503` + tu número → `50312345678`

> 💡 Si en el futuro quieres números distintos por sección o botón, regresa al editor online y se los configuro individualmente.

---

### 📧 Cambiar el correo

Busca: `contacto@miempresa.com`
Hay **2 apariciones** — reemplaza con tu correo real.

---

### 🏢 Cambiar el nombre de la empresa

Busca: `MIEMPRESA`
Hay varias apariciones (encabezado, pie de página, etc.). Reemplaza todas.

---

### 🗺️ Cambiar la dirección / horario

Busca: `San Salvador, El Salvador — Lun a Vie, 8:00–18:00`
Reemplaza con tu dirección y horario real.

---

### 🎨 Cambiar los colores

Busca el bloque de variables CSS:
```css
:root{
  --marca:#0f2a4a;        /* azul navy principal */
  --acento:#e08a4b;       /* ámbar cálido */
  --crema:#faf6f0;        /* fondo principal */
  ...
}
```
Cambia los valores hexadecimales (`#0f2a4a`, etc.) por tus colores. El cambio se aplica automáticamente en toda la página.

---

### 🔤 Cambiar textos (eslogan, títulos, descripciones)

Busca el texto exacto que quieres cambiar y reemplázalo.
Por ejemplo, para cambiar el eslogan:

Busca: `Soluciones jurídicas y financieras a la medida de cada cliente`
Reemplaza con tu eslogan.

---

### 📸 Agregar una foto real (en lugar del placeholder)

Actualmente hay un placeholder de imagen en la sección principal (Hero).

**Opción A — Imagen online (más fácil):**
Sube tu foto a un servicio (Google Drive público, Imgur, etc.) y usa la URL directa.

Busca en `index.html`:
```html
imagen del equipo / oficina
```
Reemplaza el bloque `<div>` que lo contiene por:
```html
<img src="https://URL-DE-TU-IMAGEN.jpg" alt="Equipo MIEMPRESA"
     style="width:100%;height:100%;object-fit:cover;border-radius:22px">
```

**Opción B — Imagen local (para GitHub Pages):**
1. Crea una carpeta `img/` junto a `index.html` en tu repositorio.
2. Sube tu foto ahí, ej: `img/equipo.jpg`.
3. Busca `imagen del equipo / oficina` y reemplaza el `<div>` por:
```html
<img src="./img/equipo.jpg" alt="Equipo MIEMPRESA"
     style="width:100%;height:100%;object-fit:cover;border-radius:22px">
```

---

### 📊 Activar Google Tag Manager / Google Analytics

Busca: `GTM-XXXXXXX` (aparece **2 veces**) → reemplaza con tu ID de GTM.
Busca: `G-XXXXXXXXXX` (aparece **2 veces**) → reemplaza con tu ID de GA4.

---

### 🔗 Agregar links reales de redes sociales

Busca los botones de redes:
```html
aria-label="Facebook"
aria-label="Instagram"
```
En cada uno, cambia `href="#"` por la URL real de tu perfil.

Ej: `href="https://facebook.com/tupagina"`

---

## 🚀 Desplegar en GitHub Pages

1. Crea un repositorio en GitHub (ej: `miempresa-web`).
2. Sube `index.html` a la raíz del repositorio (y la carpeta `img/` si usaste imágenes locales).
3. Ve a **Settings → Pages → Branch: main → / (root) → Save**.
4. Tu sitio estará disponible en: `https://tu-usuario.github.io/miempresa-web/`

---

## 🔄 ¿Cómo pedir cambios más complejos?

Para cambios de diseño, estructura o nuevas secciones, regresa al editor online donde fue creado este sitio. Edita `MIEMPRESA.dc.html`, aplica los cambios y solicita un nuevo `index.html` compilado.

---

## 📌 Notas importantes

- **No edites** el archivo `MIEMPRESA.dc.html` directamente a mano — es el archivo fuente del editor online.
- Siempre haz una **copia de seguridad** de `index.html` antes de editar.
- Usa VS Code con la extensión **Live Server** para previsualizar cambios localmente.
