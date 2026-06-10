# Rayfin Templates

Official project templates for scaffolding new Rayfin applications via `rayfin init`.

## Usage

Use these templates directly with the Rayfin CLI:

```bash
# Use the default template picker (discovers templates from this repo)
rayfin init

# Point directly at this repository
rayfin init -t https://github.com/microsoft/rayfin-templates.git

# Select a specific template non-interactively
rayfin init -t https://github.com/microsoft/rayfin-templates.git --template-name todoapp
```

## Available Templates

| Name | Description |
|------|-------------|
| `todoapp` | End-to-end Fabric-authenticated todo CRUD with Rayfin data model and per-user row-level security |

## Template Manifest

This repository uses a `rayfin-template.yml` manifest at the root to declare available templates.
The Rayfin CLI discovers and validates this manifest when fetching templates from git sources.

## Contributing

To add a new template:

1. Create a directory under `templates/`
2. Add the template source files (must include a `package.json`)
3. Add an entry to `rayfin-template.yml` pointing to the new directory
4. Tag a release so the CLI can pin to a stable ref

## License

MIT
