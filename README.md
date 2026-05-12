# Rstack Renovate config

Shared Renovate config for Rstack projects.

## Usage

### Default preset

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>rstackjs/renovate"]
}
```

The default preset includes the security preset.

### Security preset

Use the security preset on its own to enable minimum release age checks:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>rstackjs/renovate:security"]
}
```
