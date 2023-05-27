# renovate-config

Shared renovate presets & defaults settings / best practices for my own repositories

## Usage instructions

To include all presets including my own personal bot preferences

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jwnmulder/renovate-config"
  ]
}
```

As an alternative, the following example will only include Renovate improvements without changing bot behavior. No personal preferences are included in these files

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "config:base",
    "github>jwnmulder/renovate-config:fixes",
    "github>jwnmulder/renovate-config:meta",
    "github>jwnmulder/renovate-config:pre-commit",
    "github>jwnmulder/renovate-config:replacements",
  ]
}
```
