# [Project Name]

[Replace this with a brief description of the Power Platform application.]

## Project documentation

- [Project overview](docs/project-overview.md)
- [Business rules](docs/business-rules.md)
- [Data sources](docs/data-sources.md)
- [Development workflow](docs/development-workflow.md)

## Repository structure

```text
.github/
    copilot-instructions.md
docs/
    project-overview.md
    business-rules.md
    data-sources.md
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

- `docs/`: project documentation.
- `src/solution/`: unpacked Power Platform solution source used with PAC CLI.
- `src/canvas-yaml/`: Canvas App YAML and Power Fx reference material.
- `src/canvas-yaml/app/`: `App.OnStart.fx` and `App.Formulas.fx`.
- `working/input/`: temporary material supplied to GitHub Copilot for troubleshooting.
- `working/output/`: temporary proposed corrections or generated material for review.

Temporary contents of both working folders are ignored by Git; `.gitkeep` files retain the folders.

## Important notes

- Reference `.fx` and YAML files do **not** automatically synchronise with the live Power App.
- Never store passwords, tokens, credentials, or sensitive business data in this repository or troubleshooting material.
