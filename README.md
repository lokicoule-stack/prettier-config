# @lokiverse/prettier-config

<div align="center">
 <img src="https://github.com/lokicoule-stack/prettier-config/blob/main/media/repo-header.svg?raw=true" alt="Lokiverse Prettier Configuration" />
</div>

Shareable Prettier configurations for TypeScript projects.

## Quick Start

```bash
npm install -D @lokiverse/prettier-config prettier
```

**package.json**

```json
{
  "prettier": "@lokiverse/prettier-config/lib"
}
```

## Configurations

| Config                           | Use Case     | Features                                 |
| -------------------------------- | ------------ | ---------------------------------------- |
| `@lokiverse/prettier-config`     | Base         | Minimal config, no plugins               |
| `@lokiverse/prettier-config/lib` | Libraries    | + package.json formatting                |
| `@lokiverse/prettier-config/app` | Applications | + HTML/JSX formatting + advanced sorting |

## Usage

### Base

```json
{
  "prettier": "@lokiverse/prettier-config"
}
```

### Library

```json
{
  "prettier": "@lokiverse/prettier-config/lib"
}
```

### Application

```json
{
  "prettier": "@lokiverse/prettier-config/app"
}
```

## What's Included

- Print width: 100
- No semicolons
- Single quotes
- Trailing commas (all)
- LF line endings

## License

MIT
