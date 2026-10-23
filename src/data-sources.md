# SharePoint list column reference

Use this template to document your project's SharePoint list structures. Replace the example lists and columns below with your project's details.

Includes lists whose names do not contain Test. Visible, writable columns only; system and read-only columns are excluded.

## UK-AM-SSO-MD-AppUsers

| Column name | Display name | Type | Choice values | Lookup target |
|---|---|---|---|---|
| Title | Title | Text | - | - |
| AppUser | AppUser | User | - | - |
| AppRole | AppRole | Choice | BasicUser, Admin | - |
| Attachments | Attachments | Attachments | - | - |

## UK-AM-SSO-MD-Infractions

| Column name | Display name | Type | Choice values | Lookup target |
|---|---|---|---|---|
| Title | Title | Text | - | - |
| InfractionDescription | Infraction Description | Text | - | - |
| Severity | Severity | Choice | Minor, Moderate, Serious, Critical | - |
| FixedPoints | Fixed Points | Number | - | - |
| AppliesTo | Applies To | Choice | ALL, EPT, Forklift (CB), Reach Truck (RT), Scissor Lift (SL) | - |
| OSHAReference | OSHA Reference | Text | - | - |
| Active | Active | Boolean | - | - |
| OSHAReferenceURL | OSHA Reference URL | URL | - | - |
| SeverityText | SeverityText | Text | - | - |
| Description | Description | Note | - | - |
| ManagerActionsNeeded | Manager Actions Needed | Note | - | - |
| Attachments | Attachments | Attachments | - | - |

## UK-AM-SSO-MD-Locations

| Column name | Display name | Type | Choice values | Lookup target |
|---|---|---|---|---|
| Title | Title | Text | - | - |
| LocationCode | Location Code | Text | - | - |
| LocationDescription | Location Description | Text | - | - |
| Attachments | Attachments | Attachments | - | - |

## UK-AM-SSO-TD-IssueRecords

| Column name | Display name | Type | Choice values | Lookup target |
|---|---|---|---|---|
| Title | Title | Text | - | - |
| ReportedBy | Reported By | User | - | - |
| ReportedDate | Reported Date | DateTime | - | - |
| EquipmentType | Equipment Type | Choice | EPT, Forklift, Reach Truck, Scissor Lift, Other | - |
| ReportedFor | Reported For | User | - | - |
| Reported_x002d_ForManager | Reported-For Manager | User | - | - |
| Location | Location | Lookup | - | UK-AM-SSO-MD-Locations → LocationCode |
| InfractionCode | Infraction | Lookup | - | UK-AM-SSO-MD-Infractions → InfractionDescription |
| Image1 | Image1 | Thumbnail | - | - |
| Image2 | Image2 | Thumbnail | - | - |
| Description | Description | Note | - | - |
| ActivePoints | Active Points | Number | - | - |
| ManagerActionsAccepted | Manager Actions Accepted | Boolean | - | - |
| Pointsremovedon | Points removed on  | DateTime | - | - |
| InfractionStatus | InfractionStatus | Choice | Created, Approved, Rejected, Manager actioned, Closed | - |
| ApprovalManagerComment | Approval Manager Comment | Note | - | - |
| Attachments | Attachments | Attachments | - | - |
