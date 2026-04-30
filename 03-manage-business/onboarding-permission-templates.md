# Onboarding & Permission Templates

_Manage Businesses › Add a New Business_

## Manage Business: Onboarding & Permission Templates

> Onboarding adds a new business to digital banking using its exact Business ID. Permission Templates are the entitlement bundles every new business inherits on day one.

### Step-by-Step Workflow

#### Step 1: Add a New Business

Enter the exact Business ID to pull the legal-entity record from the core into the digital banking platform. The Matching Results screen flags any duplicates before they're created — a duplicate splits the audit trail and creates downstream issues, so always confirm there's no existing match before proceeding.

![Step 1: Add a New Business](../.gitbook/assets/mb-27-add-new-business.png)

#### Step 2: Permission Templates

The catalogue of entitlement bundles available to assign during onboarding: Business Template 1, Test Template, and any custom additions. Every new business inherits one of these templates as its starting point.

![Step 2: Permission Templates](../.gitbook/assets/mb-28-permission-templates-list.png)

#### Step 3: Permission Template Details

The full list of capabilities included in a given template: Bill Pay, Scheduled Transfers, Recipients, external transfers, and more. Review this before assigning to a new business to confirm the bundle matches the agreed services.

![Step 3: Permission Template Details](../.gitbook/assets/mb-29-permission-template-details.png)

#### Step 4: Edit Permission Template

Two-pane Available / Included editor that applies credit-union-wide. Any change here propagates into every future onboarding that uses this template, so treat each edit as a credit-union-wide change.

![Step 4: Edit Permission Template](../.gitbook/assets/mb-30-permission-template-edit.png)

#### Step 5: Delete Template

A confirmation modal appears before any template is deleted. Confirm a replacement is in place and that no in-progress onboarding depends on the template before deleting.

![Step 5: Delete Template](../.gitbook/assets/mb-31-delete-template-confirm.png)

### Summary

Onboarding maps a Business ID to the core record and assigns a Permission Template as the starting entitlement. Permission Templates are the credit-union-wide service tiers — editing one changes the starting point for every future onboarding that uses it, so template edits should be reviewed and approved like any other policy change.

### Key Use Cases

* New commercial loan closes and needs digital banking access: enter the Business ID, confirm no duplicate match, assign Business Template 1, the business is live with standard entitlements.
* Credit union launches a new treasury feature for all commercial businesses: edit Business Template 1 to include the feature — every future onboarding inherits it automatically.
