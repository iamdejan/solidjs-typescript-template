# SolisJS TypeScript Template

This is a repository for minimal SolidJS TypeScript template, adapted from [ts-minimal template](https://github.com/solidjs/templates/tree/main/ts-minimal).

The only difference with `ts-minimal` template is that ESLint is included in this template.

## Prerequisites

Before running this project, ensure you have the following installed:

1. **Node.js** (v18 or higher) - [Download](https://nodejs.org/)
2. **PNPM** - Package manager
   ```bash
   npm install -g pnpm
   ```

## Getting Started

1. **Install dependencies:**
   ```bash
   pnpm install
   ```

2. **Start the development server:**
   ```bash
   pnpm start
   ```
   This will start the Vite dev server at http://localhost:3000

## Available Scripts

| Command | Description |
|---------|-------------|
| `pnpm start` | Start the development server |
| `pnpm dev` | Start the development server (alias) |
| `pnpm build` | Build for production |
| `pnpm serve` | Preview the production build |
| `pnpm lint` | Run ESLint |
| `pnpm lint:fix` | Fix ESLint issues automatically |
| `pnpm test` | Run tests in watch mode |
| `pnpm test:ci` | Run tests once |
| `pnpm coverage` | Run tests with coverage report |
| `pnpm type:check` | Run TypeScript type checking |

## Project Tree Structure

```
Root/
├── .editorconfig        # Editor configuration for consistent coding styles across editors
├── .gitignore           # Specifies intentionally untracked files to ignore in Git
├── AGENTS.md            # Guidelines for AI assistant code generation and validation
├── eslint.config.js     # ESLint configuration for code linting
├── index.html           # HTML entry point - loads the SolidJS app
├── LICENSE.txt          # Project license (MIT)
├── package.json         # Project manifest with dependencies and scripts
├── pnpm-lock.yaml       # PNPM lockfile for reproducible builds
├── README.md            # This file
├── setupVitest.ts       # Vitest test setup - configures mocks and test environment
├── tsconfig.json        # TypeScript compiler configuration
├── vite.config.js       # Vite bundler configuration with SolidJS and ESLint plugins
├── .github/
│   └── workflows/
│       ├── pr-pipeline.yaml   # GitHub Actions workflow for pull requests
│       └── trunk-pipeline.yaml # GitHub Actions workflow for trunk-based development
├── .kilocode/
│   └── rules/           # (currently empty) Reserved for Kilo Code custom rules
└── src/
    ├── index.tsx        # Entry point - renders the App component to the DOM
    ├── App.tsx          # Main application component with counter logic
    ├── App.test.tsx     # Unit tests for the App component
    └── Comp.tsx         # Child component rendered by App
```

This section explains the purpose of each file in the repository:

### Root Directory Files

| File | Description |
|------|-------------|
| [`.editorconfig`](.editorconfig) | Defines coding styles for different editors to ensure consistent formatting |
| [`.gitignore`](.gitignore) | Lists files and directories that should not be tracked by Git (node_modules, dist, etc.) |
| [`AGENTS.md`](AGENTS.md) | Guidelines for AI assistant code generation, validation, and task execution |
| [`eslint.config.js`](eslint.config.js) | Configures ESLint with SolidJS, TypeScript, and Prettier support |
| [`index.html`](index.html) | HTML template with root div and script reference to entry point |
| [`LICENSE.txt`](LICENSE.txt) | MIT License for the project |
| [`package.json`](package.json) | NPM package manifest defining project metadata, scripts, and dependencies |
| [`pnpm-lock.yaml`](pnpm-lock.yaml) | Lockfile ensuring deterministic dependency installation |
| [`setupVitest.ts`](setupVitest.ts) | Vitest setup file that configures test environment and global mocks |
| [`tsconfig.json`](tsconfig.json) | TypeScript configuration with strict mode and SolidJS JSX settings |
| [`vite.config.js`](vite.config.js) | Vite configuration with SolidJS plugin, ESLint, and dev server settings |

### Source Files

| File | Description |
|------|-------------|
| [`src/index.tsx`](src/index.tsx) | Application entry point that mounts App to the DOM |
| [`src/App.tsx`](src/App.tsx) | Main component with increment/decrement counter functionality |
| [`src/App.test.tsx`](src/App.test.tsx) | Vitest test suite for App component |
| [`src/Comp.tsx`](src/Comp.tsx) | Simple child component demonstrating component composition |

### Configuration Directories

| File | Description |
|------|-------------|
| [`.github/workflows/`](.github/workflows) | CI/CD pipelines for automated testing and quality checks |
| [`.kilocode/rules/`](.kilocode/rules) | (currently empty) Reserved for Kilo Code custom rules |
