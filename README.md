# 🎨 Colorfly Studio

Aplicación web interactiva para generar paletas de colores dinámicas en formato **RGB** y **HSL**, con sistema de bloqueo de colores, detección automática de contraste y copia al portapapeles.

Proyecto desarrollado como proyecto para aprender lógica en JavaScript y flujo de trabajo con Git y GitHub.

---

## 🚀 Demo

🔗 Ver proyecto en vivo:  
https://hdmacias.github.io/ProyectoM1_HernanMacias/

---

## 🛠 Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript
- Git
- GitHub
- GitHub Pages

---

# 📖 Manual de Usuario (Instrucciones de uso)

## 🎛 1. Seleccionar cantidad de paletas
En el primer selector puedes elegir cuántos colores quieres generar:
- 6
- 8
- 9

## 🎨 2. Seleccionar formato de color
En el segundo selector puedes elegir el formato:
- RGB
- HSL

## 🔄 3. Generar colores
Presiona el botón **"Generar Paleta"** para crear colores aleatorios.

## 📋 4. Copiar color
Haz clic sobre cualquier color generado para copiar automáticamente su código al portapapeles.

## 🔒 5. Bloquear un color
Haz clic en el icono 🔓 para bloquear una paleta.
Cuando esté bloqueada 🔒, ese color no cambiará al generar una nueva paleta.

---

# 🧠 Manual Técnico (Decisiones técnicas)

## 🎲 Generación de colores
Se utiliza `Math.random()` para generar valores RGB entre 0 y 255:

```js
Math.floor(Math.random() * 256)
```

## 🔄 Conversión RGB → HSL
Se implementó una función personalizada `rgbAHsl()` para convertir los valores manualmente sin usar librerías externas.

## 🌗 Cálculo automático de contraste
Se usa la fórmula de luminancia relativa:

```js
(0.299 * r + 0.587 * g + 0.114 * b) / 255
```

Esto permite decidir si el texto debe ser blanco o negro según el fondo.

## 🔒 Sistema de bloqueo
Se usa `classList.toggle("bloqueado")` para evitar que una paleta cambie cuando el usuario genera nuevos colores.

## 📂 Manipulación del DOM
Se utilizan:
- `querySelector`
- `querySelectorAll`
- `addEventListener`
- `classList`
- `style`

Todo implementado en JavaScript.

---

# 💻 Cómo ejecutar la aplicación en local

## Opción 1 – Descarga manual

1. Descargar el repositorio como ZIP desde GitHub
2. Extraer la carpeta
3. Abrir `index.html` en el navegador

---

## Opción 2 – Clonar con Git

```bash
git clone https://github.com/hdmacias/Paleta-de-Colores.git
```

Luego:

1. Entrar en la carpeta del proyecto
2. Abrir `index.html` en el navegador

---

# 🌍 Cómo desplegar la aplicación (GitHub Pages)

1. Subir el proyecto a GitHub
2. Ir al repositorio
3. Entrar en **Settings**
4. Ir a **Pages**
5. En "Build and deployment":
   - Source → Deploy from a branch
   - Branch → main
   - Folder → / (root)
6. Guardar

GitHub generará automáticamente un enlace público.

Cada vez que se haga:

```bash
git add .
git commit -m "Descripción del cambio"
git push
```

La página se actualiza automáticamente.

---

# 📂 Estructura del proyecto

```
ProyectoM1_HernanMacias
│
├── index.html
├── Css/
│   └── Style.css
├── Js/
│   └── Script.js
└── README.md
```

---

# 🎯 Objetivo del proyecto

Este proyecto fue desarrollado como proyecto para:

- Manipulación avanzada del DOM
- Conversión de formatos de color
- Buenas prácticas con Git
- Flujo de trabajo profesional
- Despliegue en producción

---

# 👨‍💻 Autor

Hernán Macías  
Desarrollador Web en formación – 2026

---

⭐ Proyecto creado con fines educativos y de práctica.