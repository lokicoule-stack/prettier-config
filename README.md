<div align="center">
  <img src="https://github.com/lokicoule-stack/prettier-config/blob/main/media/repo-header.svg?raw=true" alt="Lokicoule Prettier Configuration" />
</div>

Prettier configuration with minimal rules.

## Installation

```bash
pnpm add -D @lokiverse/prettier-config
```

## Usage

Update `package.json`:

```json
{
  "prettier": "@lokiverse/prettier-config"
}
```

## Configuration

```javascript
{
  // Use official Prettier schema for validation
  "$schema": "https://json.schemastore.org/prettierrc",

  // Line length before wrapping
  // Default: 80
  "printWidth": 100,

  // Use single quotes instead of double quotes
  // true  => const x = 'test'
  // false => const x = "test"
  "singleQuote": true,

  // If you quote a property, quote all properties
  // "as-needed"  => { foo: "bar", "quotedFoo": "bar" }
  // "consistent" => { "foo": "bar", "quotedFoo": "bar" }
  // "preserve"   => { foo: "bar", "quotedFoo": "bar" }
  "quoteProps": "consistent",

  // Put each HTML attribute on a new line
  // true:
  // <button
  //   class="btn"
  //   onClick={click}>
  //   Button
  // </button>
  "singleAttributePerLine": true,

  // Control whitespace sensitivity in HTML
  // "css"     => Respect CSS display property
  // "strict"  => Whitespace is considered significant
  // "ignore"  => Whitespace is considered insignificant
  "htmlWhitespaceSensitivity": "ignore"
}
```
