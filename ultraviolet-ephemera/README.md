# Why ASTRO 
Astro was chosen for this project because it provides the right balance between structure and creative freedom. Its static-first architecture allows each animation to be developed using standard HTML, CSS, and JavaScript while avoiding unnecessary framework overhead. Each animation can remain self-contained, with its own assets, styles, and scripts, making experimentation and maintenance straightforward. At the same time, Astro provides a scalable foundation for organizing, showcasing, and expanding a growing animation library without limiting the use of custom SVG, canvas, or JavaScript-based interactions.

# Animation Guide
Plain html and css but really cool effects

## 1. CSS + SVG 
*Intro* :Using the SVG of a text, animating the border and shifting the initial and timig, a really cool effect can be achieved.
*Effect* : An SVG-style path drawing animation that resolves into filled text.
*Specific CSS Variables* :
  .experiment1 svg path{
    fill: transparent;
    stroke: blue;
    stroke-width: 1.2;
    stroke-dasharray: 270;
    stroke-dashoffset: 270;
    animation: textAnimation 3s ease-in forwards;
  }

  @keyframes textAnimation {
    0% {
      stroke-dashoffset: 270;
    }
    50% {
      fill: transparent;
    }
    100% {
      stroke-dashoffset: 0;
      fill: blue;
    }
  } 


# Astro Starter Kit: 

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src
│   ├── assets
│   │   └── astro.svg
│   ├── components
│   │   └── Welcome.astro
│   ├── layouts
│   │   └── Layout.astro
│   └── pages
│       └── index.astro
└── package.json
```

To learn more about the folder structure of an Astro project, refer to [our guide on project structure](https://docs.astro.build/en/basics/project-structure/).

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
