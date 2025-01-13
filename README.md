# Project Mapper Templates

This repository contains templates for the project-mapper tool. It is designed to be used as a git submodule in projects that use project-mapper.

## Structure

```
templates/
  ├── base.xml          # Default template with core rules
  ├── python.xml        # Python-specific template (optional)
  └── typescript.xml    # TypeScript-specific template (optional)
```

## Usage

1. As a submodule:
   ```bash
   cd your-project
   project-mapper --setup-templates
   ```
   This will prompt you to either use the default templates or specify your own.

2. Creating your own templates:
   - Fork this repository
   - Modify existing templates or add new ones
   - Use your fork's URL when running `project-mapper --setup-templates`

## Template Format

Templates are XML files that define:
1. Code documentation rules
2. Project structure mapping
3. Relationship tracking

See `templates/base.xml` for the core template structure. 