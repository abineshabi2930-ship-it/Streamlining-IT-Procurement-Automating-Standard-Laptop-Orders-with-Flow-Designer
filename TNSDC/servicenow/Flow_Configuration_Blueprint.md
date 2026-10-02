# ServiceNow Configuration Blueprint

## 1. Flow properties

**Flow name:** Standard laptop task  
**Application:** Global  
**Run as:** System User

## 2. Trigger

Select:

`Service Catalog`

## 3. Action

Select:

`Create Catalog Task`

### Action values

- Request Item: `Requested Item Record`
- Table: `Catalog Task`
- Short Description: `Laptop need to Configured`
- Description: `Laptop need to Configured`
- Assignment Group: `Hardware`
- Approval: `Approved`

## 4. Catalog item assignment

Open:

`Maintain Items → Standard Laptop → Process Engine`

Add the flow:

`Standard Laptop Task`

Save the catalog item.

## 5. Test procedure

Open:

`Service Catalog → Hardware → Standard Laptop → Order Now`

Then:

1. Open the Request Number.
2. Open the Approvers section.
3. Approve the request.
4. Open the Requested Item.
5. Open Catalog Tasks.
6. Open the generated task.
7. Verify the short description and Hardware assignment.

## 6. Deployment note

Do not treat this markdown file as a ServiceNow deployment artifact. For a real deployment, export the configured Flow/Application/Update Set from the ServiceNow instance and commit the official export.
