# Café Aurora

Café Aurora es un sitio web académico para una cafetería ficticia de Medellín. Presenta sus productos, servicios, carta de bebidas y un formulario de contacto. El sitio se maquetó con Bootstrap y una hoja de estilos compartida para la paleta visual.

> **Sitio publicado:** [Ver Café Aurora en GitHub Pages](https://yersonfranco.github.io/proyecto-modular/)

Los nombres, productos, precios, horarios y datos de contacto son ficticios. El formulario permite practicar validación en el navegador, pero no envía ni almacena información.

## Páginas

| Página | Contenido |
|---|---|
| [Inicio](index.html) | Presentación, tarjetas de productos, carrusel y horario. |
| [Servicios y carta](pages/servicios.html) | Tarjetas de servicios y tabla de bebidas con precios. |
| [Contacto](pages/contacto.html) | Formulario Bootstrap con validación, modal y datos de atención. |
| [Comparación de layouts](pages/comparativa-bootstrap.html) | El mismo conjunto de tarjetas con CSS propio y con grid y utilidades Bootstrap. |

La navegación permite recorrer las páginas desde celular, tableta y escritorio. Los elementos interactivos —navbar colapsable, carrusel y modal— usan JavaScript de Bootstrap.

## Conceptos aplicados

- **Flexbox:** alinea el contenido del navbar y organiza elementos en una dirección.
- **Grid:** compara un layout de CSS propio con el sistema grid y utilidades responsivas de Bootstrap.
- **Diseño responsive:** las páginas se ajustan a distintos anchos mediante el sistema de breakpoints de Bootstrap y el CSS de comparación.
- **Bootstrap:** navbar, cards, grid, carousel, formulario validado, alertas, modal, tabla y utilidades de espaciado.
- **Identidad visual:** styles.css define la paleta y los estilos comunes de Café Aurora.

## Estructura del proyecto

```text
proyecto-modular/
├── index.html
├── pages/
│   ├── comparativa-bootstrap.html
│   ├── contacto.html
│   └── servicios.html
├── css/
│   └── styles.css
├── img/
│   ├── portada.jpg
│   ├── latte.jpg
│   ├── cappuccino.jpg
│   ├── filtrado.jpg
│   ├── servicio-local.jpg
│   ├── servicio-reservas.jpg
│   └── servicio-empresas.jpg
└── README.md
```

## Abrir el proyecto

1. Clona el repositorio:

   ```bash
   git clone https://github.com/YersonFranco/proyecto-modular.git
   ```

2. Abre la carpeta en Visual Studio Code y ejecuta index.html con Live Server.
3. Usa el navbar para visitar Servicios y Contacto, o el enlace de la portada para abrir la comparación.

Bootstrap se carga desde un CDN; hace falta conexión a internet para sus estilos y componentes interactivos.

## Historial de cambios

El proyecto conserva sus avances en Git y está publicado con GitHub Pages. Los commits describen los cambios realizados con el formato Conventional Commits.

## Autor

**Yerson Franco**
Proyecto académico del módulo de Desarrollo de Software de Riwi, Cohorte 8+.
