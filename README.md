# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript and enable type-aware lint rules. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## Tailwind CSS

1. **Install Tailwind CSS**

    ```bash
    npm install tailwindcss @tailwindcss/vite
    ```

    Install tailwindcss and @tailwindcss/vite via npm.

2. **Configure the Vite plugin**
    ```bash
    import { defineConfig } from 'vite'
    import tailwindcss from '@tailwindcss/vite'

    export default defineConfig({
        plugins: [
            `tailwindcss(),`
        ],
    })
    ```

    Add the @tailwindcss/vite plugin to your Vite configuration.

3. **mport Tailwind CSS**
    ```bash
    @import "tailwindcss";
    ```

    Add an `@import` to your CSS file that imports Tailwind CSS.

4. **Start your build process**
    ```bash
    npm run dev
    ```
    Run your build process with `npm run dev` or whatever command is configured in your `package.json file.`

5. **Start using Tailwind in your HTML**
    ```bash
    <!doctype html>
    <html>
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <link href="/src/styles.css" rel="stylesheet">
        </head>
        <body>
            <h1 class="text-3xl font-bold underline">
                Hello world!
            </h1>
        </body>
    </html>
    ```

    Make sure your compiled CSS is included in the `<head>` (your framework might handle this for you), then start using Tailwind’s utility classes to style your content.

