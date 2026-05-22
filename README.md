# Sistema de Control de Temperatura Analógico

Blog explicativo del proyecto de **Electrónica Analógica** (UMG, Quinto Ciclo "B").
Sitio estático listo para **GitHub Pages**: cubre la **Fase I (diseño del circuito)** y la **Fase II (análisis de riesgos)**.

## 📁 Estructura

```
sistema-temperatura-analogico/
├── index.html              ← página principal (abre esta)
├── .nojekyll               ← evita que GitHub procese el sitio con Jekyll
├── README.md
└── assets/
    ├── css/style.css
    ├── js/main.js
    └── img/
        ├── diagrama-sensor.png
        ├── diagrama-visualizacion.png
        ├── diagrama-potencia.png
        ├── real-lm358.jpg
        ├── real-lm3914.jpg
        └── real-potencia.jpg
```

Las rutas son **relativas**, así que funciona igual en local y en GitHub Pages.

## 🚀 Subir a GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `control-temperatura`).
2. Sube **todo el contenido de esta carpeta** a la raíz del repo (que `index.html` quede en la raíz, no dentro de otra subcarpeta).
   ```bash
   git init
   git add .
   git commit -m "Sitio del proyecto de control de temperatura analógico"
   git branch -M main
   git remote add origin https://github.com/USUARIO/control-temperatura.git
   git push -u origin main
   ```
3. En GitHub: **Settings → Pages → Build and deployment**.
   - Source: **Deploy from a branch**
   - Branch: **main** · carpeta **/ (root)** → **Save**.
4. Espera ~1 minuto. El sitio quedará en:
   `https://USUARIO.github.io/control-temperatura/`

## 🖼️ Cambiar o agregar imágenes

Reemplaza los archivos dentro de `assets/img/` manteniendo el **mismo nombre**, o usa nombres nuevos y actualiza el `src` en `index.html`. Recomendado: JPG para fotos (<300 KB) y PNG para esquemáticos.

## ✏️ Personalizar

- **Colores y fuentes:** variables `:root` al inicio de `assets/css/style.css`.
- **Datos de riesgo:** objeto `RISKS` en `assets/js/main.js` (alimenta la matriz interactiva).
- **Tabla de presupuesto y textos:** directamente en `index.html`.
