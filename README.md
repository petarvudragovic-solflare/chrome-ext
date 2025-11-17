# Chrome Extension Monorepo

This is a Turborepo monorepo for managing Chrome extension projects.

## Structure

```
.
├── apps/          # Applications (Chrome extensions, web apps, etc.)
├── libs/          # Shared libraries and packages
├── package.json   # Root package.json with workspace configuration
└── turbo.json     # Turborepo configuration
```

## Getting Started

1. Install dependencies:
```bash
npm install
```

2. Run all apps in development mode:
```bash
npm run dev
```

3. Build all apps:
```bash
npm run build
```

4. Lint all packages:
```bash
npm run lint
```

## Adding New Apps

Create a new directory in `apps/` with its own `package.json`. The workspace will automatically pick it up.

## Adding New Libraries

Create a new directory in `libs/` with its own `package.json`. These can be shared across apps.

## Workspace Commands

- `npm run build` - Build all apps and libs
- `npm run dev` - Run all apps in development mode
- `npm run lint` - Lint all packages
- `npm run format` - Format code with Prettier

