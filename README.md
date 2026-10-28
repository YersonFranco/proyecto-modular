# Café Aurora: sitio web multipágina

Proyecto modular del módulo de HTML y CSS del programa de Desarrollo de Software de Riwi (Cohorte 8+). Consiste en un sitio web de tres páginas para una cafetería de especialidad ficticia en Medellín, desarrollado con HTML5 semántico y CSS3.

## Sitio publicado

[Ver Café Aurora en GitHub Pages](https://yersonfranco.github.io/proyecto-modular/index.html)

## Descripción

Café Aurora es un negocio ficticio creado con fines académicos. Representa una cafetería de especialidad que ofrece bebidas preparadas con granos seleccionados de fincas colombianas.

El sitio web presenta el negocio, muestra sus productos más pedidos, describe sus servicios, publica una carta de bebidas con precios y ofrece un formulario de contacto para consultas, reservas y pedidos empresariales.

Los nombres, precios, horarios y correos electrónicos utilizados son datos ficticios con fines académicos.

## Objetivos del proyecto

- Construir un sitio web multipágina utilizando HTML5 semántico.
- Organizar el contenido mediante una estructura clara y accesible.
- Aplicar estilos con una hoja de CSS externa compartida por las tres páginas.
- Implementar una identidad visual coherente mediante colores, tipografía, espacios y tarjetas.
- Utilizar CSS Grid para organizar los productos y servicios.
- Incorporar un diseño adaptable a diferentes tamaños de pantalla.
- Implementar un formulario con validación nativa de HTML5.
- Publicar el sitio mediante GitHub Pages y gestionar los cambios con Git.

## Páginas del sitio

| Página    | Archivo          | Descripción                                                                  |
| --------- | ---------------- | ---------------------------------------------------------------------------- |
| Inicio    | `index.html`     | Presentación de la cafetería, productos más pedidos y horario de atención.   |
| Servicios | `servicios.html` | Descripción de los servicios de la cafetería y carta de bebidas con precios. |
| Contacto  | `contacto.html`  | Formulario de contacto con validación nativa y horario de atención.          |

Las tres páginas comparten la misma hoja de estilos, un menú de navegación y una identidad visual consistente. También incluyen enlaces para facilitar la navegación entre las diferentes secciones del sitio.

## Tecnologías utilizadas

- **HTML5:** estructura del contenido mediante etiquetas semánticas.
- **CSS3:** diseño visual, colores, tipografía, espaciado, tarjetas y adaptación a diferentes pantallas.
- **CSS Grid:** distribución de las tarjetas de productos y servicios.
- **Variables CSS:** definición y reutilización de los colores y la tipografía del proyecto.
- **Git:** control de versiones.
- **GitHub:** alojamiento del repositorio del proyecto.
- **GitHub Pages:** publicación del sitio web.
- **Visual Studio Code:** editor de código utilizado durante el desarrollo.
- **Live Server:** visualización y prueba del sitio durante el desarrollo local.

## Diseño y estilos

El sitio utiliza CSS nativo, sin depender de frameworks externos como Bootstrap o Tailwind CSS.

Los estilos se encuentran centralizados en el archivo `css/styles.css`, que está enlazado desde las tres páginas HTML.

Las principales características del diseño son:

- **Paleta de colores:** tonos café, naranja, beige, blanco y gris oscuro.
- **Variables CSS:** permiten mantener los colores y la tipografía consistentes en todo el sitio.
- **Tipografía:** se utiliza Poppins como primera opción, con Arial y fuentes sans-serif como alternativas.
- **Encabezado:** fondo café oscuro, nombre de la cafetería y navegación con texto claro.
- **Tarjetas:** fondo blanco, bordes redondeados y sombras suaves.
- **Distribución:** CSS Grid organiza los productos y servicios en tres columnas en pantallas grandes.
- **Imágenes adaptables:** las imágenes conservan sus proporciones y se ajustan al espacio disponible.
- **Navegación interactiva:** los enlaces incluyen estados visuales al pasar el cursor, al recibir el foco del teclado y al identificar la página actual.
- **Diseño responsivo:** mediante media queries, las tarjetas pasan a una sola columna en pantallas de hasta 700 píxeles de ancho.

### Variables CSS principales

Las variables definidas en `:root` centralizan los valores visuales del proyecto:

| Variable           | Función                                                                            |
| ------------------ | ---------------------------------------------------------------------------------- |
| `--color-primario` | Color café principal de la identidad visual.                                       |
| `--color-acento`   | Color naranja utilizado como acento.                                               |
| `--color-texto`    | Color principal del texto.                                                         |
| `--color-fondo`    | Color de fondo general.                                                            |
| `--color-blanco`   | Color blanco utilizado en elementos como las tarjetas y los textos del encabezado. |
| `--fuente-base`    | Familia tipográfica principal y sus alternativas.                                  |

## Accesibilidad

El proyecto incorpora prácticas básicas de accesibilidad:

- El idioma del documento está declarado mediante `lang="es"`.
- Las páginas cuentan con un título principal (`h1`) y una jerarquía organizada de encabezados.
- Las imágenes informativas incluyen textos alternativos mediante el atributo `alt`.
- Se utilizan etiquetas semánticas como `header`, `nav`, `main`, `section`, `article`, `aside` y `footer`.
- Los enlaces tienen textos descriptivos que ayudan a comprender su propósito.
- El menú identifica la página actual mediante `aria-current="page"`.
- Los campos del formulario cuentan con etiquetas `label` asociadas.
- Los enlaces incluyen estados de interacción y foco para facilitar la navegación mediante el teclado.
- Se utilizan controles HTML nativos para aprovechar el comportamiento y la validación del navegador.

## Formulario y validación

El formulario de contacto utiliza validación nativa de HTML5, sin necesidad de JavaScript.

| Campo              | Validación                                                                              |
| ------------------ | --------------------------------------------------------------------------------------- |
| Nombre completo    | Obligatorio, mínimo 3 y máximo 60 caracteres.                                           |
| Correo electrónico | Obligatorio y con formato de correo válido.                                             |
| Celular            | Opcional; si se completa, debe contener 10 dígitos y comenzar por 3.                    |
| Motivo             | Obligatorio. Permite seleccionar entre reserva, pedido para empresa o consulta general. |
| Mensaje            | Obligatorio, mínimo 10 y máximo 500 caracteres.                                         |

El formulario incluye atributos como `required`, `minlength`, `maxlength`, `pattern` y `type="email"` para establecer las reglas de validación.

**Importante:** el formulario es únicamente demostrativo. Aunque el navegador valida los campos, el sitio no dispone actualmente de un servidor que reciba y procese los mensajes enviados.

## Estructura del proyecto

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
└── README.md
```

### Organización de los archivos

- `index.html`: contiene la página principal.
- `servicios.html`: presenta los servicios y la carta de bebidas.
- `contacto.html`: contiene el formulario de contacto.
- `css/styles.css`: centraliza los estilos visuales de todo el sitio.
- `img/`: almacena las imágenes utilizadas en las diferentes páginas.
- `README.md`: documenta el proyecto, sus tecnologías y las instrucciones de ejecución.

## Cómo ejecutar el proyecto en local

### Requisitos

- Tener instalado [Git](https://git-scm.com/).
- Contar con [Visual Studio Code](https://code.visualstudio.com/) o un editor de código equivalente.
- Disponer de un navegador web.
- Para utilizar Live Server, instalar su extensión en Visual Studio Code.

### Pasos

1. Clona el repositorio:

   ```bash
   git clone https://github.com/YersonFranco/proyecto-modular.git
   ```

2. Entra en la carpeta del proyecto:

   ```bash
   cd proyecto-modular
   ```

3. Abre la carpeta en Visual Studio Code:

   ```bash
   code .
   ```

4. Abre `index.html` y selecciona **Open with Live Server**.

5. Navega por el sitio y comprueba que los enlaces, las imágenes, los estilos y el formulario funcionen como se espera.

También es posible abrir `index.html` directamente en el navegador, aunque Live Server facilita las pruebas durante el desarrollo.

## Publicación en GitHub Pages

El sitio está publicado mediante GitHub Pages.

Para consultar la versión publicada, visita:

[https://yersonfranco.github.io/proyecto-modular/index.html](https://yersonfranco.github.io/proyecto-modular/index.html)

Los archivos HTML, la hoja de estilos y las imágenes deben permanecer organizados en el repositorio para que GitHub Pages pueda cargarlos correctamente.

## Control de versiones

El proyecto utiliza Git para registrar los cambios realizados durante el desarrollo.

Los mensajes de confirmación siguen una convención sencilla basada en Conventional Commits, con el formato:

```text
tipo: descripción breve del cambio
```

Los tipos utilizados incluyen:

- `feat`: incorporación de una funcionalidad o característica.
- `fix`: corrección de un error.
- `docs`: cambios en la documentación.
- `style`: ajustes de formato o presentación que no modifican la lógica del sitio.
- `chore`: tareas de mantenimiento y organización.

Ejemplos:

```bash
git add .
git commit -m "feat: agregar estilos a las tarjetas de productos"
git commit -m "fix: corregir la distribución de las tarjetas"
git commit -m "docs: actualizar el README del proyecto"
```

Para enviar los cambios al repositorio remoto:

```bash
git push origin main
```

## Mejoras futuras

Entre las posibles mejoras para próximas etapas del proyecto se encuentran:

- Implementar un mecanismo de recepción y procesamiento de los mensajes del formulario.
- Mejorar la presentación visual de la carta de bebidas.
- Incorporar nuevas funcionalidades según los requisitos de los siguientes módulos.
- Continuar verificando la accesibilidad y la adaptación a diferentes dispositivos.

## Autor

**Yerson Franco**  
Coder de Riwi — Cohorte 8+  
Módulo de Desarrollo de Software  
Proyecto académico de HTML y CSS.
