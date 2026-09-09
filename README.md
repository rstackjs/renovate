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

For `.node-version`, the default preset preserves major-only versions (for example, `22` → `24`) and disables minor, patch, and pin updates. Set existing full versions such as `24.21.0` to a major-only value such as `24` to use this behavior.

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
