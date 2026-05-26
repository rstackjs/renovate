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

The default preset includes the security, disableNodeEngines, and disablePeerDependencies presets.

### Security preset

Use the security preset on its own to enable minimum release age checks and GitHub Actions digest pinning:

```json
{
  "extends": ["github>rstackjs/renovate:security"]
}
```

### Disable Node engines preset

Use this preset to disable Node.js engine updates from npm:

```json
{
  "extends": ["github>rstackjs/renovate:disableNodeEngines"]
}
```

### Disable peer dependencies preset

Use this preset to disable peer dependency updates:

```json
{
  "extends": ["github>rstackjs/renovate:disablePeerDependencies"]
}
```
