# [Project Name]

[Brief description of this Power Platform application]

## Repository structure

```text
.github/
    copilot-instructions.md
docs/
    project-overview.md
    business-rules.md
    development-workflow.md
src/
    canvas-yaml/
        app/
            App.OnStart.fx
            App.Formulas.fx
    solution/
        .gitkeep
working/
    input/
        .gitkeep
    output/
        .gitkeep
.gitignore
README.md
```

- `docs/`: project context, business rules, and delivery documentation.
- `src/solution/`: unpacked Power Platform solution source for the PAC CLI workflow.
- `src/canvas-yaml/`: clean Canvas App screen/component YAML and Power Fx reference material; preserved by default during Copilot troubleshooting.
- `src/canvas-yaml/app/`: application-level App.OnStart and App.Formulas Power Fx; initially comments only.
- `working/input/`: disposable snippets to troubleshoot.
- `working/output/`: disposable proposed corrections or local export packages to review.

Temporary contents of both working folders are ignored by Git; `.gitkeep` files retain the folders.

Reference `.fx` and YAML files do **not** automatically synchronise with a live Power App.

Never put passwords, tokens, credentials, or sensitive business data in this repository or troubleshooting snippets.

## Project documentation

- [Project overview](docs/project-overview.md)
- [Business rules](docs/business-rules.md)
- [Data sources](docs/data-sources.md)
- [Development workflow](docs/development-workflow.md)
