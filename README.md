# renovate-config

Shared renovate presets & defaults settings / best practices for my own repositories.

See <https://docs.renovatebot.com/config-presets> for detailed information and usage instructions.

## Usage instructions

To include all presets including my own personal bot preferences.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jwnmulder/renovate-config"
  ]
}
```

As an alternative, the following example will only include Renovate improvements, extending from config:base. No personal preferences are included in these files.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>jwnmulder/renovate-config:base"
  ]
}
```

which is similar to

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "config:base",
    "github>jwnmulder/renovate-config:fixes",
    "github>jwnmulder/renovate-config:meta",
    "github>jwnmulder/renovate-config:pre-commit",
    "github>jwnmulder/renovate-config:replacements"
  ]
}
```
