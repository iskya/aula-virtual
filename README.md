# 📚 Aula Virtual — Instrucciones para GitHub Pages

## Estructura de carpetas

```
aula-virtual/
├── index.html                  ← Página de inicio (con las 4 materias)
├── styles.css                  ← Estilos compartidos
├── README.md                   ← Este archivo
│
├── fisica-4to-d/
│   ├── index.html              ← Página de Física 4to D
│   ├── unidad-1.pdf            ← Tus PDFs van acá
│   └── ...
│
├── fisica-5to-d/
│   ├── index.html
│   └── ...
│
├── fisica-5to-e/
│   ├── index.html
│   └── ...
│
└── electrotecnia-4to-d/
    ├── index.html
    └── ...
```

---

## ✅ Paso a paso para publicar en GitHub Pages

### 1. Crear el repositorio en GitHub
1. Ingresá a [github.com](https://github.com) con tu cuenta
2. Hacé clic en **"New repository"** (botón verde, arriba a la derecha)
3. Escribí un nombre, por ejemplo: `aula-virtual`
4. Marcá **"Public"**
5. Hacé clic en **"Create repository"**

### 2. Subir los archivos
En la página de tu nuevo repositorio:
1. Hacé clic en **"uploading an existing file"** (o el botón **"Add file" → "Upload files"**)
2. **Arrastrá toda la carpeta** `aula-virtual` (o subí los archivos uno por uno respetando la estructura)
3. Hacé clic en **"Commit changes"**

### 3. Activar GitHub Pages
1. En tu repositorio, hacé clic en **"Settings"** (arriba, en el menú)
2. En el menú lateral, buscá **"Pages"**
3. En **"Source"**, elegí **"Deploy from a branch"**
4. En **"Branch"**, elegí **"main"** y la carpeta **"/ (root)"**
5. Hacé clic en **"Save"**

⏳ Esperá 1 o 2 minutos y tu sitio estará disponible en:
```
https://TU-USUARIO.github.io/aula-virtual/
```

---

## ➕ Cómo agregar un PDF a una materia

1. Entrá a tu repositorio en GitHub
2. Navegá a la carpeta de la materia (ej: `fisica-4to-d/`)
3. Hacé clic en **"Add file" → "Upload files"**
4. Subí el archivo PDF
5. Hacé clic en **"Commit changes"**

Luego editá el `index.html` de esa materia para agregar el enlace de descarga.
Buscá el comentario `<!-- AGREGÁ LOS ARCHIVOS AQUÍ ↓ -->` y agregá:

```html
<li class="archivo-item">
  <span class="archivo-nombre"><span>📄</span> Nombre que verán los alumnos</span>
  <a class="btn-dl" href="nombre-exacto-del-archivo.pdf" download>⬇ Descargar</a>
</li>
```

> ⚠️ El nombre en `href="..."` debe coincidir **exactamente** con el nombre del archivo PDF subido (respetando mayúsculas, minúsculas y espacios).

---

## 💡 Tips

- Usá nombres de archivo sin espacios ni tildes para evitar problemas (ej: `unidad-1-cinematica.pdf`)
- Cuando agregues varios PDFs, borrá o comentá el mensaje "Próximamente se agregarán los materiales"
- Para hacerlo: abrí el `index.html` de la materia en GitHub, buscá la línea con `placeholder-msg` y rodeala con `<!-- -->` o borrá ese bloque

---

¿Dudas? ¡Cualquier problema con el sitio se puede resolver fácilmente editando los archivos HTML desde GitHub directamente!
