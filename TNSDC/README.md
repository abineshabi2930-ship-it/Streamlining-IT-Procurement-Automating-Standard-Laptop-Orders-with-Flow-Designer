# Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

A ServiceNow project that automates the creation and assignment of a laptop configuration Catalog Task when a Standard Laptop item is requested through the Service Catalog.

## Project
- Platform: ServiceNow
- Main tool: Flow Designer
- Flow: `Standard laptop task`
- Application: `Global`
- Run as: `System User`
- Trigger: `Service Catalog`
- Action: `Create Catalog Task`
- Assignment Group: `Hardware`

## Workflow

Service Catalog → Standard Laptop → Request → Approval → Flow Designer → Create Catalog Task → Hardware Assignment → Verify Catalog Task

## Catalog Task configuration

| Field | Value |
|---|---|
| Request Item | Requested Item Record |
| Table | Catalog Task |
| Short Description | Laptop need to Configured |
| Description | Laptop need to Configured |
| Assignment Group | Hardware |
| Approval | Approved |

## Repository contents

- `docs/` – project and implementation documentation
- `servicenow/` – ServiceNow configuration blueprint
- `demo/` – demonstration/voice-over notes
- `screenshots/` – place for project screenshots

## Important

This project is primarily a **ServiceNow low-code configuration project**, not a conventional Python/Java source-code project. The uploaded project document describes the Flow Designer configuration but does not contain a deployable ServiceNow update-set XML or application source export.

For deployment to another ServiceNow instance, export the actual Flow/Application/Update Set from your ServiceNow instance and add the exported files to `servicenow/`.

## Demonstration

1. Open Flow Designer.
2. Create `Standard laptop task`.
3. Configure the Service Catalog trigger.
4. Add `Create Catalog Task`.
5. Configure Requested Item Record, description, Hardware assignment and Approved.
6. Save and activate.
7. Assign the flow to the Standard Laptop catalog item.
8. Order Standard Laptop from Service Catalog.
9. Approve the request.
10. Verify the generated Catalog Task.

## Project documentation

The repository is intended to accompany the six project phases and Phase 7 demonstration documentation.
