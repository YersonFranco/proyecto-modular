# Café Aurora: sitio web multipágina

Proyecto modular del módulo de HTML y CSS del programa de Desarrollo de Software de Riwi (Cohorte 8+). Es un sitio web de tres páginas para una cafetería de especialidad ficticia en Medellín, construido con HTML semántico.

## Sitio publicado

[Ver el sitio en GitHub Pages](https://yersonfranco.github.io/proyecto-modular/index.html)

## Descripción

Café Aurora es un negocio de ejemplo para esta actividad: una cafetería de especialidad que sirve granos seleccionados de fincas colombianas. El sitio presenta el negocio, muestra sus servicios y su carta de bebidas, y permite enviar un mensaje de contacto mediante un formulario.

Los nombres, precios, horarios y correos son datos inventados con fines académicos.

## Páginas

| Página    | Archivo          | Qué muestra                                                                                                   |
| --------- | ---------------- | ------------------------------------------------------------------------------------------------------------- |
| Inicio    | `index.html`     | Presentación del negocio, lo más pedido y horario de atención                                                 |
| Servicios | `servicios.html` | Tres servicios (café en el local, reservas de mesa y pedidos para empresas) y la carta de bebidas con precios |
| Contacto  | `contacto.html`  | Formulario de contacto con validación y horario de atención                                                   |

Las tres páginas comparten el mismo menú y el mismo pie de página, y están enlazadas entre sí.

## Tecnologías

- HTML5 semántico: `header`, `nav`, `main`, `section`, `article`, `aside` y `footer`.
- Hoja de estilos externa: `css/styles.css` (en construcción).
- Git y GitHub para el control de versiones.
- GitHub Pages para la publicación.

## Framework de estilos

El sitio está en su fase de estructura. El framework de estilos (Bootstrap o Tailwind CSS) se elegirá y se justificará en la fase de diseño, y esta sección se actualizará con esa decisión.

## Accesibilidad

- Idioma del documento declarado con `lang="es"`.
- Un solo `h1` por página y encabezados en orden, sin saltos.
- Texto alternativo descriptivo en todas las imágenes.
- Enlaces con textos que se entienden fuera de contexto.
- Estructura con significado: el menú, el contenido principal y el pie están marcados con sus etiquetas.
- Elementos nativos (`a`, `button`, `input`) que se pueden usar con el teclado.
- Cada campo del formulario tiene su `label` asociada.

## Formulario y validación

El formulario de contacto usa solo validación nativa de HTML5, sin JavaScript:

| Campo              | Regla                                                          |
| ------------------ | -------------------------------------------------------------- |
| Nombre completo    | Obligatorio, mínimo 3 caracteres                               |
| Correo electrónico | Obligatorio, con formato de correo válido                      |
| Celular            | Opcional; si se escribe, 10 dígitos y debe empezar por 3       |
| Motivo             | Obligatorio (reservar, pedido para empresa o consulta general) |
| Mensaje            | Obligatorio, mínimo 10 caracteres                              |

El formulario no envía los datos a ningún servidor: al ser un sitio estático, la recepción real de los mensajes se construirá en módulos posteriores.

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

## Cómo ver el proyecto en local

1. Clona el repositorio:
   ```bash
   git clone https://github.com/YersonFranco/proyecto-modular.git
   ```
2. Abre la carpeta en VS Code.
3. Ejecuta `index.html` con la extensión Live Server, o ábrelo directamente en el navegador.

## Control de versiones

El historial usa Conventional Commits con el formato `tipo: descripción`. Los tipos que se usan son `feat` (algo nuevo), `fix` (una corrección), `docs` (documentación), `style` (estilos) y `chore` (tareas de orden).

## Autor

Yerson Franco, coder de Riwi. Módulo de Desarrollo de Software, actividad académica.
