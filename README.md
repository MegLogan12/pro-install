 LOVING Salesforce Full Build (Skeleton)

This repository is a **starting point** for the LOVING Group Salesforce implementation.

It follows Salesforce DX source format and includes placeholder directories for:

- Objects
- Apex classes
- Lightning Web Components
- Flows
- Permission Sets

## Structure

```
force-app/main/default/objects/           # Custom object definitions
force-app/main/default/classes/           # Apex controllers and services
force-app/main/default/lwc/               # Lightning Web Components
force-app/main/default/flows/             # Flows and process definitions
force-app/main/default/permissionsets/    # Permission sets
manifest/package.xml                      # Deployment manifest
```

## How to use

1. **Clone this repo** into your Salesforce DX workspace.
2. Fill out each placeholder with metadata from the LOVING Salesforce Build Specification v3.
3. Deploy to your sandbox using the Salesforce CLI:

```sh
sf project deploy start --source-dir force-app --target-org <your-org-alias>
```

4. Commit your changes and push to GitHub.

This skeleton is intentionally minimal. You must add:

- Custom objects such as `Work_Order__c`, `Takeoff__c`, `Checklist__c`, etc.
- CPQ objects (`SBQQ__Quote__c` fields) and flows.
- Pipeline engine and status automation.
- Checklists and document templates.

Use the build specification for guidance.
