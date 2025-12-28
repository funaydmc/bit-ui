# Bit UI - Svelte Component Library

A modern Svelte component library with TypeScript support. This project provides reusable UI components that can be easily integrated into any Svelte application.

## Features

- 🧩 **Reusable Components**: Well-designed, accessible UI components
- 🎯 **TypeScript Support**: Full type safety and IntelliSense
- 📦 **NPM Package**: Easy installation and updates
- 🎪 **Live Demo**: Interactive component showcase
- 🔄 **Automated CI/CD**: GitHub Actions for testing and deployment

## Installation

```sh
npm install bit-ui
```

## Usage

```javascript
// Import components from the library
import { ComponentName } from 'bit-ui';
```

## Development

## Development

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```sh
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

The demo app in `src/routes` serves as a showcase for your components. Everything inside `src/lib` is part of your component library.

## Building

### Build Library Package

To build the component library for distribution:

```sh
npm run build
```

This creates the distributable package in the `dist/` directory, ready for publishing to npm.

### Build Demo Site

To build the static demo site:

```sh
npm run build:demo
```

This creates a static website in the `build/` directory showcasing your components.

You can preview the demo site with `npm run preview`.

### GitHub Actions Workflow

The project includes automated CI/CD that:

1. **On every push/PR**:
   - Builds and tests the library
   - Builds the demo site
   - Runs quality checks

2. **On main/master branch**:
   - Deploys demo site to GitHub Pages

3. **On version tags** (e.g., `v1.0.0`):
   - Automatically publishes library to npm

#### Setting up auto-publishing to npm:

1. Create an npm account and get an access token
2. Add the token to your repository secrets as `NPM_TOKEN`
3. Push a version tag: `git tag v1.0.0 && git push origin v1.0.0`

#### Setting up GitHub Pages:

1. Go to repository Settings → Pages
2. Select "GitHub Actions" as the source
3. The demo site will be automatically deployed

## Publishing

To manually publish your library to [npm](https://www.npmjs.com):

```sh
# Update version in package.json first
npm version patch  # or minor/major
npm run build
npm publish
```
