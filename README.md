# Informe de Proyecto: Galería de Imágenes Responsivas

## Estudiante
**Nombre:** Daniel Hervás Muñoz  
**Asignatura:** Diseño de Interfaces Web  
**Curso:** 2º DAW

## Descripción del Proyecto
En este proyecto se ha creado una galería de imágenes responsiva utilizando HTML, CSS, JS y Bootstrap. El objetivo principal es mostrar cómo se pueden adaptar las imágenes a diferentes tamaños de pantalla utilizando técnicas de diseño responsivo.

### Estructura del Proyecto

#### **index.html**
El archivo principal `index.html` contiene la estructura básica del sitio. Se incluyen varias librerías y tecnologías para garantizar la correcta visualización de las imágenes en distintos dispositivos:

- **Fuentes personalizadas:** Se usan dos fuentes de Google Fonts: `Poppins` y `Playfair Display`.
- **Iconos Font Awesome:** Se ha integrado Font Awesome para agregar un icono de cámara al encabezado.
- **Bootstrap:** Para facilitar la creación de un diseño responsivo y atractivo, se incluye Bootstrap.
- **CSS personalizado:** Se ha añadido un archivo `style.css` para aplicar estilos adicionales.

#### **Cuerpo de la Página**
La página tiene un **encabezado** que contiene un ícono de cámara y un mensaje descriptivo: "Transformamos tus ideas en arte". A continuación, se encuentra un contenedor de imágenes organizado en un sistema de columnas que se adapta a la pantalla según el tamaño del dispositivo.

#### **Imágenes**
Cada imagen de la galería se muestra utilizando la etiqueta `<picture>`, lo que permite especificar diferentes fuentes de imagen para diferentes resoluciones y tamaños de pantalla. Las imágenes son adaptadas de la siguiente manera:

### Uso de Script para Generar Imágenes Responsivas

Para garantizar que las imágenes se muestren correctamente en diferentes dispositivos, se ha utilizado un script en Node.js con la librería `sharp` para generar versiones de las imágenes optimizadas para distintos tamaños de pantalla y densidades de píxeles.

- **Imágenes en 1x y 2x:** Se proporciona una versión de cada imagen para pantallas estándar (1x) y para pantallas de alta resolución (2x).
- **Media Queries:** Se usan para cargar imágenes diferentes según el tamaño de la pantalla:
  - Pantallas pequeñas (máximo 500px)
  - Pantallas medianas (máximo 768px)
  - Pantallas grandes (máximo 1024px)
  - Pantallas extra grandes (a partir de 1920px)
  
Esto asegura que las imágenes se cargan de forma eficiente según las capacidades de cada dispositivo.

#### **Diseño Responsivo**
El uso de **Bootstrap** junto con las clases de columna (`col-12`, `col-sm-6`, `col-md-4`, `col-lg-4`) permite que las imágenes se distribuyan en una sola columna en dispositivos pequeños y en varias columnas en pantallas más grandes.

### Uso de Modal y Script para Visualización de Imágenes

Para mejorar la experiencia del usuario, se ha implementado una funcionalidad que permite al usuario hacer clic en cualquier imagen de la galería y verla en grande en una ventana modal. Además, se incluye una flecha para volver a la galería.
