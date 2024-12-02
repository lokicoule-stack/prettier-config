# @lokiverse/prettier-config

<div align="center">
 <img src="https://github.com/lokicoule-stack/prettier-config/blob/main/media/repo-header.svg?raw=true" alt="Lokicoule Prettier Configuration" />
</div>

Opinionated Prettier configuration with package.json sorting capabilities.

## Installation

```bash
pnpm add -D @lokiverse/prettier-config
```

## Usage

Add to `package.json`:

```json
{
  "prettier": "@lokiverse/prettier-config"
}
```

## Configuration Details

```json
{
  // Use official Prettier schema
  "$schema": "https://json.schemastore.org/prettierrc",

  // Line length: 100 characters
  "printWidth": 100,

  // No semicolons
  "semi": false,

  // Use single quotes
  "singleQuote": true,

  // Quote style for object properties
  "quoteProps": "consistent",

  // One attribute per line in HTML/JSX
  "singleAttributePerLine": true,

  // HTML whitespace handling
  "htmlWhitespaceSensitivity": "ignore",

  // Automated package.json sorting
  "plugins": ["prettier-plugin-packagejson"]
}
```

### Package.json Sorting

```json
[
  // Package Identity
  "name",
  "displayName",
  "version",
  "private",
  "description",
  "publisher",
  "keywords",
  "categories",

  // Legal & Authorship
  "author",
  "license",
  "funding",
  "sponsors",

  // Documentation & Links
  "homepage",
  "repository",
  "bugs",
  "documentation",

  // Package Configuration
  "type",
  "main",
  "module",
  "types",
  "typesVersions",
  "exports",
  "imports",
  "files",
  "bin",
  "sideEffects",
  "engines",

  // Project Configuration
  "scripts",
  "workspaces",
  "packageManager",

  // Dependencies
  "dependencies",
  "peerDependencies",
  "peerDependenciesMeta",
  "optionalDependencies",
  "devDependencies",
  "bundledDependencies",

  // Release Management
  "np",
  "release-it",
  "standard-version",

  // Publishing
  "config",
  "publishConfig",
  "directories",

  // Package Resolution
  "overrides",
  "resolutions",
  "pnpm",

  // Development Tools
  "husky",
  "simple-git-hooks",
  "lint-staged",
  "commitlint",

  // Tool Configuration
  "eslintConfig",
  "eslintIgnore",
  "prettier",
  "browserslist",
  "babel",
  "jest",
  "postcss",
  "stylelint",

  // IDE & Extensions
  "icon",
  "activationEvents",
  "contributes",

  // Testing
  "c8",
  "nyc",
  "tap",
  "ava"
]
```
