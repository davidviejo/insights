# David Viejo Insights

Repositorio estático para `insights.davidviejo.com`.

## Estructura

- `/estudios/`: investigaciones y contenidos públicos indexables.
- `/clientes/`: entregables para clientes. Todos deben incluir `noindex`.
- `/assets/`: CSS, JavaScript e imágenes comunes.

## Crear un nuevo estudio

1. Duplica `/estudios/ejemplo-estudio/`.
2. Renombra la carpeta con un slug descriptivo.
3. Edita `index.html`.
4. Añade la nueva URL a `/estudios/index.html`.
5. Añade la URL a `sitemap.xml`.

Ejemplo:

`/estudios/visibilidad-marcas-chatgpt-2026/index.html`

## Crear un nuevo informe de cliente

1. Crea `/clientes/nombre-cliente/nombre-informe/index.html`.
2. Mantén en `<head>`:

```html
<meta name="robots" content="noindex, nofollow, noarchive">
```

3. No añadas URLs de cliente al sitemap ni a páginas públicas.

> Importante: `noindex` no equivale a protección mediante contraseña. Si el informe contiene información sensible, añade autenticación o control de acceso en la capa de hosting.

## Despliegue recomendado

GitHub → Vercel → `insights.davidviejo.com`
