# Presupuesto Interactivo: Tienda Inteligente para FINCA LA SEIS

## Descripción

Este proyecto es una página de aterrizaje (landing page) moderna y responsiva diseñada como una propuesta de presupuesto para el cliente "FINCA LA SEIS". La página presenta dos opciones para el desarrollo de una tienda e-commerce:

1.  **Opción Estándar:** Una tienda online completa y bien diseñada.
2.  **Opción Avanzada:** La tienda estándar, más la integración de un asistente virtual impulsado por Inteligencia Artificial (IA) para mejorar la atención al cliente y automatizar consultas.

La página está desarrollada por **Gannet labs** (anteriormente Agencia Web IA) y tiene como objetivo mostrar de forma clara y atractiva las características, beneficios y precios de cada opción.

## Tecnologías Utilizadas

*   **Framework:** [Astro](https://astro.build/) (Versión utilizada según `package.json`)
*   **Estilos CSS:** [Tailwind CSS](https://tailwindcss.com/) (Integrado con Astro)
*   **Animaciones:** [AOS (Animate On Scroll)](https://michalsnik.github.io/aos/)
*   **Favicon:** SVG simple.

## Estructura del Proyecto

El proyecto sigue la estructura estándar de Astro:

```
.
├── public/
│   └── favicon.svg
│   └── (otros assets estáticos)
├── src/
│   ├── components/         # Componentes reutilizables de Astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── PricingSection.astro
│   │   ├── ComparisonTable.astro
│   │   ├── TermsAndConditions.astro
│   │   ├── CallToAction.astro
│   │   └── Footer.astro
│   ├── layouts/            # Plantillas de página
│   │   └── Layout.astro
│   ├── pages/              # Páginas del sitio (rutas)
│   │   └── index.astro
│   └── styles/             # Estilos globales
│       └── global.css
├── astro.config.mjs        # Configuración de Astro
├── package.json            # Dependencias y scripts del proyecto
├── tailwind.config.cjs     # Configuración de Tailwind CSS
└── tsconfig.json           # Configuración de TypeScript
```

## Instalación y Uso

1.  **Clonar el repositorio (si aplica):**
    ```bash
    # git clone <url-del-repositorio>
    # cd <nombre-del-directorio>
    ```

2.  **Instalar dependencias:**
    Asegúrate de tener Node.js (preferiblemente una versión LTS) y npm instalados.
    ```bash
    npm install
    ```

3.  **Iniciar el servidor de desarrollo:**
    Esto iniciará un servidor local (generalmente en `http://localhost:4321`) con recarga en caliente.
    ```bash
    npm run dev
    ```

4.  **Construir para producción:**
    Esto generará los archivos estáticos del sitio en el directorio `dist/`.
    ```bash
    npm run build
    ```

5.  **Previsualizar la construcción (después de `npm run build`):**
    ```bash
    npm run preview
    ```

## Características Clave

*   **Diseño Moderno y Responsivo:** Adaptable a diferentes tamaños de pantalla (móvil, tablet, escritorio) utilizando Tailwind CSS.
*   **Dos Opciones de Presupuesto:** Presentación clara de dos planes de e-commerce para "FINCA LA SEIS".
*   **Detalles de Características:** Listado exhaustivo de lo que incluye cada plan.
*   **Tabla Comparativa:** Facilita la visualización de las diferencias entre los planes.
*   **Sección de Términos y Condiciones:** Con elementos desplegables para mejorar la legibilidad.
*   **Sección "¿Por qué una suscripción mensual?" Desplegable:** En cada plan, para reducir la cantidad de texto visible inicialmente.
*   **Llamada a la Acción (CTA):** Botón de WhatsApp para contacto directo, con mensaje predefinido.
*   **Animaciones Sutiles:** Implementadas con AOS para mejorar la experiencia de usuario al hacer scroll.
*   **Tema Oscuro Moderno:** Con una paleta de colores personalizada y scrollbar estilizado.
*   **Favicon Personalizado.**
*   **Integración de IA:** La Opción 2 destaca la inclusión de un asistente virtual con IA.

## Personalización

*   **Contenido del Cliente:** El contenido actual está enfocado en "FINCA LA SEIS". Para adaptarlo a otro cliente, se deben modificar los textos en los componentes (`.astro` files), especialmente en:
    *   `src/components/Hero.astro` (Título principal)
    *   `src/components/PricingSection.astro` (Detalles de los planes, precios)
    *   `src/components/CallToAction.astro` (Mensaje final, número de WhatsApp)
*   **Nombre de la Agencia:** Actualmente es "Gannet labs". Se puede cambiar en:
    *   `src/components/Header.astro`
    *   `src/components/Footer.astro`
*   **Estilos y Colores:** Se pueden ajustar en `tailwind.config.cjs` y `src/styles/global.css`.
*   **Número de WhatsApp y Mensaje Predefinido:** Configurado en `src/components/CallToAction.astro`.

---

Este README provee una guía básica del proyecto. Para detalles específicos de Astro o Tailwind CSS, por favor consulta sus documentaciones oficiales. 