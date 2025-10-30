# create-deepkit-starter

Scaffold a new [Deepkit Framework](https://deepkit.io) project with TypeScript, Vitest, and production-ready infrastructure.

This tool instantiates projects from the [deepkit-starter](https://github.com/eram/deepkit-starter) template repository.

## Usage

Create a new Deepkit project with one command:

```bash
# Using npx (recommended)
npx create-deepkit-starter my-app

# Using npm
npm init deepkit-starter my-app

# Using yarn
yarn create deepkit-starter my-app

# Using pnpm
pnpm create deepkit-starter my-app
```

Then follow the prompts to configure your project!

## What's Included

Your new project comes with:

- **Deepkit Framework** - Runtime type system with decorators and dependency injection
- **TypeScript** - ES2020 target with strict mode and Deepkit reflection
- **Vitest** - Fast testing with TypeScript support and coverage reporting
- **vite-node** - Fast TypeScript execution with hot-reload
- **Docker** - Multi-stage builds with Wolfi OS and security scanning
- **Biome** - Fast linter and formatter with opinionated configuration
- **CI/CD Ready** - Integration tests and release automation included

## Quick Start

After creating your project:

```bash
cd my-app

# Install dependencies
npm install

# Run in development mode (with hot-reload)
npm run dev

# Run tests
npm test

# Run tests in watch mode
npm run test:watch

# Build Docker image
npm run build
```

## Project Structure

```
my-app/
├── src/              - Application source code
│   ├── app.ts        - Main application with CLI commands
│   └── app.test.ts   - Unit tests
├── ci/               - Integration tests
│   ├── app.ci.test.ts - CI tests with TypeScript
│   └── test.ts        - Shared test types
├── script/           - Build and utility scripts
│   ├── release.js     - Semantic versioning and changelog
│   ├── run-ci-tests.js - CI test runner
│   └── run-vitest.js  - Vitest wrapper for faster execution
├── .vscode/          - VSCode debug configurations
├── Dockerfile        - Multi-stage Docker build
├── vite.config.js    - Vite configuration with Deepkit plugin
└── tsconfig.json     - TypeScript configuration
```

## Commands

- `npm run dev` - Run app in watch mode with hot-reload
- `npm run app` - Run application
- `npm test` - Run linter and tests
- `npm run test:unit` - Run tests with coverage
- `npm run test:watch` - Run tests in watch mode
- `npm run ci` - Run integration tests
- `npm run lint` - Check code quality
- `npm run lint:fix` - Fix linting issues
- `npm run build` - Build Docker image with tests and scanning
- `npm run release` - Create a new release with changelog

## Requirements

- Node.js >= 24.0.0
- Docker (optional, for containerized builds)

## Learn More

- [Deepkit Documentation](https://deepkit.io/documentation)
- [Deepkit Framework Guide](https://deepkit.io/library/framework)
- [Vitest Documentation](https://vitest.dev/)

## License

The scaffolding tool is licensed under Apache-2.0.

Generated projects can use any license you choose.
