# Content v2 Minimal Starter

## Creation

```bash
$ npx nuxi init content-from-scratch -t content
Nuxi 3.0.0-rc.12                                                                                                                                                                                         12:29:42

 ERROR  (node:621084) ExperimentalWarning: The Fetch API is an experimental feature. This feature could change at any time                                                                               12:29:42
(Use `node --trace-warnings ...` to show where the warning was created)

✨ Nuxt project is created with content template. Next steps:                                                                                                                                            12:29:43
 › cd content-from-scratch-01                                                                                                                                                                            12:29:43
 › Install dependencies with npm install or yarn install or pnpm install --shamefully-hoist                                                                                                              12:29:43
 › Start development server with npm run dev or yarn dev or pnpm run dev

$ cd content-from-scratch
$ npm i
ls
$ npm run dev
```

## Commits

> Based on reading through docs and trying out stuff

- bedc8b6 initial commit
  - just as indicated in [Getting Started](https://content.nuxtjs.org/get-started) with catch-all route
- 98abbd8 regular nuxt page plus two markdown content pages with navigation
  - Moved index to /pages/index.vue and changed /content/index.md to /content/the-content.md
- 1f59048 added more content to content paths

All content available as [API](http://localhost:3000/api/_content/query) automatically

## Starter Doc

Look at the [Content documentation](https://content-v2.nuxtjs.org/) to learn more.

### Setup

Make sure to install the dependencies:

```bash
# yarn
yarn install

# npm
npm install

# pnpm
pnpm install --shamefully-hoist
```

### Development Server

Start the development server on http://localhost:3000

```bash
npm run dev
```

### Production

Build the application for production:

```bash
npm run build
```

Locally preview production build:

```bash
npm run preview
```

Checkout the [deployment documentation](https://v3.nuxtjs.org/docs/deployment) for more information.

## Initial commit
