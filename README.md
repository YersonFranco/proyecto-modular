# Café Aurora — Proyecto modular de HTML y CSS

Café Aurora es un sitio web académico para una cafetería ficticia de Medellín. El proyecto fue creciendo semana a semana: primero se practicó HTML, luego se construyeron las páginas de la cafetería con HTML y CSS, y después se comparó el diseño propio con Bootstrap.

> **Sitio publicado:** [Ver Café Aurora](https://yersonfranco.github.io/proyecto-modular/index.html)

Los nombres, productos, precios, horarios y datos de contacto son ficticios. El sitio sirve para practicar y mostrar lo aprendido; no recibe pedidos reales.

## ¿Qué contiene el sitio?

El sitio principal tiene tres páginas conectadas entre sí:

| Página | Archivo | ¿Qué encontrarás? |
|---|---|---|
| Inicio | [`index.html`](index.html) | Presentación de Café Aurora, productos favoritos y horario. La sección de productos usa la grilla y algunas clases de Bootstrap. |
| Servicios | [`servicios.html`](servicios.html) | Servicios de la cafetería y carta de bebidas con precios. |
| Contacto | [`contacto.html`](contacto.html) | Formulario demostrativo para consultas, reservas y pedidos empresariales. |

También hay dos páginas de práctica en la carpeta `pruebas/`: una compara CSS propio con Bootstrap y la otra presenta una página demostrativa con componentes de Bootstrap.

## Recorrido del proyecto

### Semana 1 — HTML y CSS del proyecto modular

#### Día 1: perfil personal

Antes de empezar el proyecto modular, se hizo un ejercicio aparte: una página de perfil personal. Allí se practicaron elementos básicos de HTML, como títulos, listas, enlaces, imágenes y tablas. Ese ejercicio no está incluido en este repositorio.

#### Día 2: estructura de Café Aurora

Se construyó el contenido de las tres páginas del sitio. Se organizaron sus secciones con elementos de HTML que describen su función, como encabezado, navegación, contenido principal, secciones y pie de página. También se enlazaron las páginas para poder recorrer el sitio.

Se creó el formulario de contacto con campos para el nombre, el correo, el celular, el motivo y el mensaje. El navegador revisa los datos obligatorios y algunos formatos antes de permitir el envío.

#### Día 3: estilos con CSS

Se creó [`css/styles.css`](css/styles.css), una hoja de estilos compartida por las tres páginas. Allí se definieron los colores y otros detalles visuales para que el sitio tuviera una identidad común.

Se usaron Flexbox para alinear elementos, como la navegación, y Grid para ordenar grupos de tarjetas. También se añadieron ajustes para que el contenido se acomode en pantallas pequeñas.

### Semana 2 — Diseño adaptable y Bootstrap

#### Día 1: Flexbox, Grid y diseño adaptable

Se reorganizaron los estilos de `css/styles.css` con el enfoque **mobile-first**: los estilos base describen primero la vista de celular y las reglas para pantallas más anchas se aplican después. El sitio conserva sus distribuciones para celular, tableta y escritorio.

En palabras sencillas, Flexbox ayuda a alinear elementos en una dirección, mientras que Grid organiza elementos en filas y columnas.

#### Día 2: grilla y utilidades de Bootstrap

En la página de Inicio, la sección **“Lo más pedido”** pasó a usar la grilla adaptable y clases de espaciado de Bootstrap. El resto del sitio principal sigue usando los estilos propios del proyecto.

La página [`pruebas/comparativa-bootstrap.html`](pruebas/comparativa-bootstrap.html) muestra la misma sección de productos de dos maneras: con CSS propio y con la grilla y utilidades de Bootstrap. La tabla al final resume las diferencias observadas.

#### Día 3: componentes y personalización de Bootstrap

Se creó [`pruebas/landing-bootstrap.html`](pruebas/landing-bootstrap.html), una página de presentación que reúne en una sola vista una navegación que se pliega en pantallas pequeñas, tarjetas de productos, un formulario y una ventana modal (un mensaje que aparece encima de la página). Sus colores siguen la identidad de Café Aurora.

El formulario de esta página es solo una demostración: no envía ni guarda información. El botón abre el modal para mostrar el componente.

## Conceptos que se practicaron

| Concepto | Explicación sencilla | Dónde aparece |
|---|---|---|
| HTML | Organiza el contenido y explica qué función cumple cada parte. | En las páginas del sitio. |
| CSS | Define colores, tamaños, espacios y presentación. | En `css/styles.css` y en las páginas de práctica. |
| Flexbox | Alinea y distribuye elementos en una dirección, por ejemplo, en una fila. | Navegación, pie de página y algunos contenidos. |
| Grid | Ordena elementos en filas y columnas. | Tarjetas de productos y servicios. |
| Diseño adaptable | Ajusta la página a celulares, tabletas y pantallas grandes. | En las reglas responsive del CSS y la grilla de Bootstrap. |
| Mobile-first | Empieza con los estilos para celular y amplía el diseño para pantallas mayores. | En `css/styles.css`. |
| Bootstrap | Ofrece clases listas para maquetar grillas, espacios y componentes. | En “Lo más pedido” y en las páginas de `pruebas/`. |
| Git y GitHub | Guardan el historial de cambios y permiten compartir el proyecto. | En el repositorio y sus commits. |

## Archivos del proyecto

```text
proyecto-modular/
├── index.html
├── servicios.html
├── contacto.html
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
├── pruebas/
│   ├── comparativa-bootstrap.html
│   └── landing-bootstrap.html
└── README.md
```

- `index.html`, `servicios.html` y `contacto.html` son las páginas principales.
- `css/styles.css` contiene los estilos compartidos del sitio principal.
- `img/` guarda las fotografías usadas en las páginas.
- `pruebas/` contiene las demostraciones de Bootstrap hechas durante la semana 2.
- `README.md` explica el proyecto y cómo abrirlo.

## Ver las páginas publicadas

- [Inicio de Café Aurora](https://yersonfranco.github.io/proyecto-modular/index.html)
- [Servicios y carta](https://yersonfranco.github.io/proyecto-modular/servicios.html)
- [Contacto](https://yersonfranco.github.io/proyecto-modular/contacto.html)
- [Comparación de CSS propio y Bootstrap](https://yersonfranco.github.io/proyecto-modular/pruebas/comparativa-bootstrap.html)
- [Página demostrativa de componentes Bootstrap](https://yersonfranco.github.io/proyecto-modular/pruebas/landing-bootstrap.html)

## Abrir el proyecto en el computador

1. Clona el repositorio desde GitHub:

   ```bash
   git clone https://github.com/YersonFranco/proyecto-modular.git
   ```

2. Entra a la carpeta y ábrela en Visual Studio Code:

   ```bash
   cd proyecto-modular
   code .
   ```

3. Abre `index.html` con Live Server. Desde la página de Inicio podrás navegar a Servicios y Contacto.

Las páginas de práctica se pueden abrir directamente desde `pruebas/comparativa-bootstrap.html` y `pruebas/landing-bootstrap.html`.

**Conexión a internet:** las páginas que usan Bootstrap descargan sus estilos y componentes desde un servicio externo llamado CDN. Se necesita conexión para que esas partes se vean y funcionen. La página de presentación también carga JavaScript de Bootstrap para que funcionen el menú plegable y la ventana modal.

## Formularios y datos

El formulario de `contacto.html` usa validación incorporada en el navegador. El proyecto no tiene un servidor que reciba los mensajes, así que el formulario principal tampoco envía consultas a una cafetería real.

## Publicación y cambios

El sitio principal está publicado en internet con GitHub Pages. Git guarda cada avance como un punto del historial llamado commit, y GitHub conserva la copia del repositorio.

Los mensajes de commit usan el formato `tipo: descripción breve`, por ejemplo:

```bash
git add index.html
git commit -m "feat: se maqueta Lo más pedido con Bootstrap"
git push origin main
```

Los tipos más usados en este proyecto son `feat` para una mejora, `fix` para una corrección y `docs` para organizar la documentación.

## Autor

**Yerson Franco**  
Proyecto académico del módulo de Desarrollo de Software de Riwi, Cohorte 8+.


