# HATCAT Traveller — Experiencia Interactiva Scrollytelling 3D

Una landing page interactiva y editorial de comercio electrónico diseñada para presentar el sombrero **HATCAT Traveller**, fusionando estética tipográfica de alta gama, microinteracciones fluidas y visualización fotorrealista 360° impulsada por scroll.

---

## ✨ Características Principales

- **Scrollytelling 3D Fotograma a Fotograma:** Sincronización del scroll con la rotación y acercamiento del producto a través de una secuencia de 240 fotogramas WebP transparentes renderizados en `<canvas>`.
- **Desplazamiento Ultra Suave:** Integración con [Lenis](https://github.com/darkroomengineering/lenis) para una física de scroll inercial suave y refinada.
- **Llamadas y Puntos de Interés Dinámicos:** Callouts interactivos calculados sobre coordenadas de imagen que se anclan con precisión a los detalles del sombrero en cualquier resolución.
- **Visor 360° Arrastrable:** Visor interactivo en la sección de compra con control táctil/mouse (*drag to rotate*) y desaceleración inercial mediante el ticker de GSAP.
- **Configurador de Producto:** Selector dinámico de acabados y colores con filtros en tiempo real, selección de tallas internacionales (cm / US) y feedback háptico/animado al añadir a la bolsa.
- **Avanzada Dirección de Arte:** Iluminación focal interactiva (*spotlight radial*), textura de grano procedural, y tipografía editorial clásica combinada con fuentes monoespaciadas (*Bodoni Moda*, *Hanken Grotesk* e *IBM Plex Mono*).
- **Rendimiento y Ligereza:** Construido sin dependencias pesadas ni frameworks de frontend; HTML5, CSS y JavaScript modernos con gestión de densidad de píxeles (`devicePixelRatio`) y caché progresivo de imágenes.

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 & CSS3:** Variables CSS, maquetación Grid/Flexbox y soporte para modo oscuro nativo.
- **JavaScript (ES6+):** Lógica reactiva de eventos, cálculos espaciales y renderizado en Canvas 2D.
- **[GSAP 3.12](https://gsap.com/):** Orquestación de animaciones de entrada, escalado de detalle y fijado de escena (*pinning*).
- **[ScrollTrigger](https://gsap.com/scrolltrigger/):** Control de progreso de animación vinculado a la posición del scroll.
- **[Lenis](https://lenis.darkroom.engineering/):** Smooth scrolling inercial moderno.

---

## 📁 Estructura del Proyecto

```text
├── index.html        # Estructura, estilos y lógica completa (HTML/CSS/JS)
├── README.md         # Documentación del proyecto
├── LEEME.txt         # Notas de desarrollo
└── frames/           # Secuencia de 240 cuadros en formato WebP (h001.webp - h240.webp)
```

---

## 🚀 Cómo Ejecutar el Proyecto Localmente

Para garantizar la correcta carga de los cuadros WebP en el `<canvas>` sin restricciones de política de origen local (CORS):

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/alberthrc/HATCAT.git
   cd HATCAT
   ```

2. **Iniciar un servidor local ligero:**
   - Con **Node.js**:
     ```bash
     npx serve .
     ```
   - O con **Python 3**:
     ```bash
     python -m http.server 8000
     ```

3. **Abrir en el navegador:**
   Visita `http://localhost:3000` (o `http://localhost:8000`).
