# Microsoft Power Platform project

- Prefer simple, practical solutions over complicated architecture.
- Preserve existing working logic wherever possible and make the smallest necessary change.
- Do not create folders without a clear reason or invent application logic.
- Keep explanations friendly to someone learning Git, GitHub, VS Code, and PAC CLI.
- Canvas Apps may use SharePoint or other data sources; do not assume Dataverse is the application's data source. Highlight it if Dataverse is used.
- Read `docs/project-overview.md` and `docs/business-rules.md` before recommending significant application changes.
- Treat `docs/data-sources.md` as the canonical reference for project data structures and data-source schema details when available.
- If `docs/data-sources.md` contains placeholders or is incomplete, clearly state assumptions and recommend updating it before structural data changes.
- Treat `src/solution/` as Power Platform solution source for the PAC CLI workflow.
- Treat `src/canvas-yaml/` as clean, protected Canvas App source/reference material.
- Screen and component YAML may live directly under `src/canvas-yaml/`.
- Application-level Power Fx belongs under `src/canvas-yaml/app/`, including `App.OnStart.fx` and `App.Formulas.fx`.

## Preserve source during troubleshooting

Requests such as "check this screen", "review this YAML", "find the problem",
"fix this Power Fx", "check this Power Fx", "why doesn't this control work?",
or "troubleshoot this screen" do not authorise edits to existing `src/canvas-yaml/` files.

First analyse the material and explain what appears wrong.
For a small Power Fx fix, clearly show the proposed replacement in the response.
For a larger YAML correction, create a proposed version under `working/output/` when useful.
Only directly edit an existing file under `src/canvas-yaml/` when the user clearly asks to apply, edit, or change the original source.

- Use `working/input/` and `working/output/` for temporary troubleshooting.
- You may analyse and modify temporary input files when the user asks to troubleshoot them; put a separate corrected version in output when useful.
- Working files are disposable, ignored by Git except for folder placeholders, and not authoritative application source.
- The user reviews proposed corrections and manually applies approved changes.
- Do not imply that manually maintained `.fx` or YAML reference files automatically synchronise with Power Apps.
- Do not automatically deploy to or overwrite a Power Platform environment from Git.
- Update relevant documentation when an actual structural or architectural decision changes.
- Do not include credentials or sensitive data in source or troubleshooting material.
