{
  "name": "shadcn-ui",
  "private": true,
  "description": "Build a component library with accessibility at its core.",
  "workspaces": [
    "apps/*",
    "packages/*"
  ],
  "scripts": {
    "build": "turbo build",
    "dev": "turbo dev",
    "lint": "turbo lint",
    "test": "turbo test",
    "typecheck": "turbo typecheck",
    "clean": "turbo clean",
    "format": "prettier --write \"**/*.{ts,tsx,md,mdx,json}\"",
    "changeset": "changeset",
    "version-packages": "changeset version",
    "release": "turbo build --filter=./packages/cli && changeset publish"
  },
  "devDependencies": {
    "@changesets/cli": "^2.26.2",
    "prettier": "^3.0.3",
    "turbo": "^1.10.16"
  },
  "packageManager": "pnpm@8.9.0",
  "engines": {
    "node": ">=18"
  }
}