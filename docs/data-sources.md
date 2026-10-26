# Data Sources

## How to fill in this file

Use SharePoint Copilot to document the SharePoint lists used by the project.

1. Open the SharePoint site containing the project lists.
2. Open Copilot in SharePoint.
3. Replace the list placeholders in the prompt below with the SharePoint lists used by the project.
4. Paste the prompt into Copilot.
5. Save the generated result as `data-sources.md` and replace this instruction file in the project repository.

## Prompt for SharePoint Copilot

```text
Generate a Markdown file called data-sources.md documenting the SharePoint lists related to this project/SharePoint Site.

Include these SharePoint lists start with the list name "UK-XX-XXX-"

Column type is important and make sure its filled in otherwise dont work on this.

For each list, create a table showing only user-created columns. Do not include standard SharePoint system columns unless they have been customised for this project.

For each column include:
- Display name
- Column/internal name
- Column type
- Available choice values, where applicable
- Lookup source, where applicable. Specify the SharePoint list and column it looks up to.

Organise the output by SharePoint list and keep it simple and factual.

Do not guess missing information. If a property cannot be determined, mark it as "Unknown".

Return the result as Markdown suitable for saving directly as data-sources.md.
```
