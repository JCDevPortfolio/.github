<h1 align="center">JCDevPortfolio · Microfrontends</h1>

<p align="center">
  Capa de <b>frontend con microfrontends Single SPA</b><br/>
  del portafolio y los productos de <b>Wilson Javier Arias Cardona</b>.
</p>

<p align="center">
  🌐 <a href="https://javiercardona.dev">javiercardona.dev</a>
  &nbsp;·&nbsp; 📚 <a href="https://storybook.javiercardona.dev">Storybook</a>
  &nbsp;·&nbsp; ⚙️ Backend: <a href="https://github.com/JCDevPortfolio-Back">JCDevPortfolio-Back</a>
</p>

---

## 🎯 Qué es

La capa de presentación del portafolio, construida como **microfrontends
independientes** con Single SPA: cada pieza (header, home, admin, auth…) se
desarrolla y despliega por separado, y `portfolio-root` las orquesta en una sola
aplicación.

## 🏗️ Arquitectura

![Arquitectura del portafolio](./diagrama_portafolio_arquitectura.svg)

- **`portfolio-root`** — contenedor/orquestador que monta los microfrontends.
- **Microfrontends** — `portfolio-header`, `portfolio-home`, `portfolio-footer`,
  `portfolio-admin`, `portfolio-front-auth`, `portfolio-payment`… desplegables de
  forma independiente.
- **`portfolio-styleguide`** — sistema de diseño compartido, documentado en
  [Storybook](https://storybook.javiercardona.dev).
- **Enrutamiento por path** con Cloudflare Tunnel hacia el backend
  (`api.javiercardona.dev`), sin nginx ni gateway adicional.

## ✨ Por qué microfrontends

- **Despliegues independientes:** cada equipo/feature se publica sin tocar el resto.
- **Escalabilidad organizativa:** repos pequeños y enfocados en lugar de un monolito.
- **Reutilización:** UI y estilos centralizados en el styleguide.

## 🛠️ Stack

`TypeScript` · `React` · `Next.js` · `Single SPA` · `Redux Toolkit` ·
`Styled Components` · `Storybook` · `Cloudflare`

## 📫 Contacto

**Wilson Javier Arias Cardona** — Desarrollador Full-Stack
🌐 [javiercardona.dev](https://javiercardona.dev) · ✉️ javiercardona.dev@gmail.com
