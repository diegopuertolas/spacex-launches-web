# SpaceX Launches 🚀

![Astro](https://img.shields.io/badge/Astro-BC52EE?style=for-the-badge&logo=astro&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

Proyecto desarrollado para mostrar información sobre los lanzamientos de SpaceX de forma visual y moderna.

## Tecnologías utilizadas

- **Astro** v5.16.6 — Framework moderno para construir sitios web rápidos y estáticos.
- **TypeScript** — Tipado estático para mayor robustez en el desarrollo.
- **Tailwind CSS** v4.1.18 — Utilidades CSS para estilos rápidos y responsivos.
- **API SpaceX** v5 — Consumo de la API pública de SpaceX para obtener datos de lanzamientos.
- **Vite** — Bundler rápido para desarrollo y producción.

## Requisitos previos

- [Node.js](https://nodejs.org/) >= 22.19.0
- [pnpm](https://pnpm.io/) >= 10.26.2

## Estructura de carpetas

```
curso-astro-demo/
├── public/                # Archivos estáticos (imágenes, favicon, etc.)
├── src/
│   ├── components/        # Componentes reutilizables (Header, Footer, CardLaunch, etc.)
│   ├── layouts/           # Layouts base para las páginas
│   ├── pages/             # Páginas principales y rutas dinámicas
│   ├── services/          # Lógica de consumo de la API SpaceX
│   ├── styles/            # Archivos CSS globales
│   └── types/             # Tipos TypeScript para la API
├── package.json           # Dependencias y scripts
└── README.md              # Documentación del proyecto
```

## API utilizada

Se utiliza la [SpaceX API v5](https://github.com/r-spacex/SpaceX-API) para obtener información actualizada sobre los lanzamientos espaciales.

- Últimos lanzamientos:  
  `https://api.spacexdata.com/v5/launches/query` (ordenados por fecha descendente)
- Lanzamientos más antiguos:  
  `https://api.spacexdata.com/v5/launches/query` (ordenados por fecha ascendente)
- Detalle de lanzamiento:  
  `https://api.spacexdata.com/v5/launches/{id}`

## Instalación y uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/diegopuertolas/spacex-launches-web.git
   cd spacex-launches-web
   ```
2. Instala las dependencias:
   ```bash
   pnpm install
   ```
3. Inicia el servidor de desarrollo:
   ```bash
   pnpm run dev
   ```
4. Accede a [http://localhost:4321](http://localhost:4321) en tu navegador.

## Autor

**Diego Puértolas Ruiz**  
Proyecto realizado siguiendo el [tutorial de astro](https://www.youtube.com/watch?v=RB5tR_nqUEw&t=57s) por [@midudev](https://github.com/midudev) con pequeños detalles extras añadidos para mejorar el proyecto.
---