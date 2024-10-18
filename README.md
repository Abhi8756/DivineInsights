# DivineInsights 📄

![DivineInsights](public/DivineInsights-og.jpg)
[![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/community/file/1356898632249991861)
![Typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![GitHub](https://img.shields.io/github/license/ascendantaditya/divineinsights?color=%232F3741&style=for-the-badge)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white&style=for-the-badge)](https://conventionalcommits.org)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=for-the-badge)](http://commitizen.github.io/cz-cli/)

DivineInsights is a minimal, responsive, accessible and SEO-friendly Astro blog theme. This theme is designed and crafted based on [my personal blog](https://ascendantaditya.github.io/pfolio/).

This theme follows best practices and provides accessibility out of the box. Light and dark mode are supported by default. Moreover, additional color schemes can also be configured.

This theme is self-documented \_ which means articles/posts in this theme can also be considered as documentations. Read [the blog posts](https://divineinsights.pages.dev/posts/) or check [the README Documentation Section](#-documentation) for more info.

## 🔥 Features

- [x] type-safe markdown
- [x] super fast performance
- [x] accessible (Keyboard/VoiceOver)
- [x] responsive (mobile ~ desktops)
- [x] SEO-friendly
- [x] light & dark mode
- [x] fuzzy search
- [x] draft posts & pagination
- [x] sitemap & rss feed
- [x] followed best practices
- [x] highly customizable
- [x] dynamic OG image generation for blog posts [#15](https://github.com/ascendantaditya/divineinsights/pull/15) ([Blog Post](https://divineinsights.pages.dev/posts/dynamic-og-image-generation-in-DivineInsights-blog-posts/))

_Note: I've tested screen-reader accessibility of DivineInsights using **VoiceOver** on Mac and **TalkBack** on Android. I couldn't test all other screen-readers out there. However, accessibility enhancements in DivineInsights should be working fine on others as well._

## ✅ Lighthouse Score

<p align="center">
  <a href="https://pagespeed.web.dev/report?url=https%3A%2F%2Fdivineinsights.pages.dev%2F&form_factor=desktop">
    <img width="710" alt="DivineInsights Lighthouse Score" src="DivineInsights-lighthouse-score.svg">
  <a>
</p>

## 🚀 Project Structure

Inside of DivineInsights, you'll see the following folders and files:

```bash
/
├── public/
│   ├── assets/
│   │   └── logo.svg
│   │   └── logo.png
│   └── favicon.svg
│   └── DivineInsights-og.jpg
│   └── robots.txt
│   └── toggle-theme.js
├── src/
│   ├── assets/
│   │   └── socialIcons.ts
│   ├── components/
│   ├── content/
│   │   |  blog/
│   │   |    └── some-blog-posts.md
│   │   └── config.ts
│   ├── layouts/
│   └── pages/
│   └── styles/
│   └── utils/
│   └── config.ts
│   └── types.ts
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

Any static assets, like images, can be placed in the `public/` directory.

All blog posts are stored in `src/content/blog` directory.

## 📖 Documentation

Documentation can be read in two formats\_ _markdown_ & _blog post_.

- Configuration - [markdown](src/content/blog/how-to-configure-DivineInsights-theme.md) | [blog post](https://divineinsights.pages.dev/posts/how-to-configure-DivineInsights-theme/)
- Add Posts - [markdown](src/content/blog/adding-new-post.md) | [blog post](https://divineinsights.pages.dev/posts/adding-new-posts-in-DivineInsights-theme/)
- Customize Color Schemes - [markdown](src/content/blog/customizing-DivineInsights-theme-color-schemes.md) | [blog post](https://divineinsights.pages.dev/posts/customizing-DivineInsights-theme-color-schemes/)
- Predefined Color Schemes - [markdown](src/content/blog/predefined-color-schemes.md) | [blog post](https://divineinsights.pages.dev/posts/predefined-color-schemes/)

> For DivineInsights v1, check out [this branch](https://github.com/ascendantaditya/divineinsights/tree/divineinsights-v1) and this [live URL](https://divineinsights-v1.divineinsights.pages.dev/)

## 💻 Tech Stack

**Main Framework** - [Astro](https://astro.build/)  
**Type Checking** - [TypeScript](https://www.typescriptlang.org/)  
**Component Framework** - [ReactJS](https://reactjs.org/)  
**Styling** - [TailwindCSS](https://tailwindcss.com/)  
**UI/UX** - [Figma Design File](https://www.figma.com/community/file/1356898632249991861)  
**Fuzzy Search** - [FuseJS](https://fusejs.io/)  
**Icons** - [Boxicons](https://boxicons.com/) | [Tablers](https://tabler-icons.io/)  
**Code Formatting** - [Prettier](https://prettier.io/)  
**Deployment** - [Cloudflare Pages](https://pages.cloudflare.com/)  
**Illustration in About Page** - [https://freesvgillustration.com](https://freesvgillustration.com/)  
**Linting** - [ESLint](https://eslint.org)

## 👨🏻‍💻 Running Locally

You can start using this project locally by running the following command in your desired directory:

```bash
# npm 6.x
npm create astro@latest --template ascendantaditya/divineinsights

# npm 7+, extra double-dash is needed:
npm create astro@latest -- --template ascendantaditya/divineinsights

# yarn
yarn create astro --template ascendantaditya/divineinsights

# pnpm
pnpm dlx create-astro --template ascendantaditya/divineinsights
```

> **_Warning!_** If you're using `yarn 1`, you might need to [install `sharp`](https://sharp.pixelplumbing.com/install) as a dependency.

Then start the project by running the following commands:

```bash
# install dependencies
npm run install

# start running the project
npm run dev
```

As an alternative approach, if you have Docker installed, you can use Docker to run this project locally. Here's how:

```bash
# Build the Docker image
docker build -t DivineInsights .

# Run the Docker container
docker run -p 4321:80 DivineInsights
```

## Google Site Verification (optional)

You can easily add your [Google Site Verification HTML tag](https://support.google.com/webmasters/answer/9008080#meta_tag_verification&zippy=%2Chtml-tag) in DivineInsights using an environment variable. This step is optional. If you don't add the following environment variable, the google-site-verification tag won't appear in the HTML `<head>` section.

```bash
# in your environment variable file (.env)
PUBLIC_GOOGLE_SITE_VERIFICATION=your-google-site-verification-value
```

> See [this discussion](https://github.com/ascendantaditya/divineinsights/discussions/334#discussioncomment-10139247) for adding DivineInsights to the Google Search Console.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

> **_Note!_** For `Docker` commands we must have it [installed](https://docs.docker.com/engine/install/) in your machine.

| Command                              | Action                                                                                                                           |
| :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| `npm install`                        | Installs dependencies                                                                                                            |
| `npm run dev`                        | Starts local dev server at `localhost:4321`                                                                                      |
| `npm run build`                      | Build your production site to `./dist/`                                                                                          |
| `npm run preview`                    | Preview your build locally, before deploying                                                                                     |
| `npm run format:check`               | Check code format with Prettier                                                                                                  |
| `npm run format`                     | Format codes with Prettier                                                                                                       |
| `npm run sync`                       | Generates TypeScript types for all Astro modules. [Learn more](https://docs.astro.build/en/reference/cli-reference/#astro-sync). |
| `npm run lint`                       | Lint with ESLint                                                                                                                 |
| `docker compose up -d`               | Run DivineInsights on docker, You can access with the same hostname and port informed on `dev` command.                              |
| `docker compose run app npm install` | You can run any command above into the docker container.                                                                         |
| `docker build -t DivineInsights .`       | Build Docker image for DivineInsights.                                                                                               |
| `docker run -p 4321:80 DivineInsights`   | Run DivineInsights on Docker. The website will be accessible at `http://localhost:4321`.                                             |

> **_Warning!_** Windows PowerShell users may need to install the [concurrently package](https://www.npmjs.com/package/concurrently) if they want to [run diagnostics](https://docs.astro.build/en/reference/cli-reference/#astro-check) during development (`astro check --watch & astro dev`). For more info, see [this issue](https://github.com/ascendantaditya/divineinsights/issues/113).

## ✨ Feedback & Suggestions

If you have any suggestions/feedback, you can contact me via [my email](mailto:contact@ascendantaditya.dev). Alternatively, feel free to open an issue if you find bugs or want to request new features.

## 📜 License

Licensed under the MIT License, Copyright © 2023

---

Made with 🤍 by [Aditya Tomar](https://ascendantaditya.dev) 👨🏻‍💻 and [contributors](https://github.com/ascendantaditya/divineinsights/graphs/contributors).
