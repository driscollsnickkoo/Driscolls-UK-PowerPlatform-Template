# Driscolls-UK-PowerPlatform-Template

Simple, beginner-friendly starting template for Microsoft Power Platform development.

## Start a project

On GitHub, choose **Use this template → Create a new repository**, name your project, then clone your new repository and open it in VS Code.
Fill in the documents under `docs/` before adding real application material.

## Structure

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

- `docs/`: project context, business rules, and the beginner guide.
- `src/solution/`: unpacked Power Platform solution source for the PAC CLI workflow.
- `src/canvas-yaml/`: clean Canvas App screen/component YAML and Power Fx reference material; preserved by default during Copilot troubleshooting.
- `src/canvas-yaml/app/`: application-level App.OnStart and App.Formulas Power Fx; initially comments only.
- `working/input/`: disposable snippets to troubleshoot.
- `working/output/`: disposable proposed corrections or local export packages to review.

Temporary contents of both working folders are ignored by Git; `.gitkeep` files retain the folders.
Never put passwords, tokens, or sensitive business data in this repository or troubleshooting snippets.

## Tools and next steps

**PAC CLI** authenticates to Power Platform and exports, unpacks, or packs solutions.
**Git** records reviewed changes locally; **GitHub** hosts and shares the committed history.
Reference `.fx` and YAML files do **not** automatically synchronise with a live Power App.

Read [Development workflow](docs/development-workflow.md), then complete the [Project overview](docs/project-overview.md) and [Business rules](docs/business-rules.md).
