_Summerville Admin Console › Manage System_

# Manage System

> Platform outage configuration and mobile-app deprecation management — the two operational levers for communicating planned downtime and enforcing build lifecycle policy.

## Step-by-Step Workflow

### Step 1: System Outages

The register of all outage events: Channel, Title, Outage Type, Frequency, Start and End times, and Status. All dates and times are in Pacific Standard Time — confirm your team is working in PST when scheduling outages to avoid off-by-one-hour errors on member-facing notifications.

![Step 1: System Outages](img/ms-01-system-outages-list.jpg)

### Step 2: Add Outage

The default settings are System Wide scope, One time frequency, and Pre-Outage Reminders enabled with Email delivery. This is the conservative baseline — start here and narrow the scope explicitly if the outage affects only a specific channel or module.

![Step 2: Add Outage](img/ms-02-add-outage.jpg)

### Step 3: Schedule Outage - Immediate

Toggle to Immediate to collapse the date and time fields to a single To field. This is the incident-response configuration — use it when an unplanned outage is already in progress and you need to push a member notification without the full scheduling workflow.

![Step 3: Schedule Outage - Immediate](img/ms-03-add-outage-immediate.jpg)

### Step 4: Outage Type - Channel Specific

Select the Channel radio to restrict the outage notification to Online, Mobile, or Voice. The NOTE: All Modules marker confirms that all features within that channel are affected — use this scope for IVR cutovers or mobile SDK rollouts where only one channel is impacted.

![Step 4: Outage Type - Channel Specific](img/ms-04-add-outage-channel-specific.jpg)

### Step 5: Outage Type - Module Specific

Select a Module Type from the dropdown — Pay Bills, Wire, ACH, and others — then use the plus icon to add sibling modules if multiple are affected, and select the applicable channels with the Online, Mobile, and Voice checkboxes. This is the narrowest scope and the right choice when only a specific payment flow is down while everything else remains available.

![Step 5: Outage Type - Module Specific](img/ms-05-add-outage-module-specific.jpg)

### Step 6: App Deprecation

The Mobile Banking Application Deprecation register. An empty "No app deprecation to display" state is expected during normal operations. Use Add Deprecation Notification when a mobile build needs to be retired — either by a soft nudge or a hard enforcement.

![Step 6: App Deprecation](img/ms-06-app-deprecation-landing.jpg)

### Step 7: Add Deprecation Notification - Recommended

Set Type of upgrade to Recommended to expose Start Date and End Date pickers. This is the soft-nudge path — members are encouraged to update during the window but not blocked if they don't, which makes it appropriate for routine patch releases and non-critical version changes.

![Step 7: Add Deprecation Notification - Recommended](img/ms-07-app-deprecation-recommended.jpg)

### Step 8: Add Deprecation Notification - Mandated

Toggle to Mandated to remove the date pickers — the hard cutoff takes effect on publish, blocking members on the deprecated build from accessing the app. Use Mandated only when Risk or InfoSec has confirmed that continuing to allow the old build creates an unacceptable security exposure.

![Step 8: Add Deprecation Notification - Mandated](img/ms-08-app-deprecation-mandated.jpg)

## Summary

Manage System has two distinct surfaces: System Outages for communicating planned and live-incident downtime to members, and App Deprecation for managing the mobile build lifecycle. Every outage record is a first-class object that drives in-channel banners and member-facing alerts — the scope and timing configuration here directly determines what members see and when.

## Key Use Cases

- Saturday wire-cut window for a core change: Module Specific outage, Wire module selected, pre- and post-notifications across Email and Push.
- IVR system cutover affecting Voice only: Channel Specific, Voice selected, Online and Mobile remain unaffected.
- Live unplanned incident: Immediate schedule, System Wide scope — push the notification first, investigate second.
- Critical TLS vulnerability on an old mobile build: App Deprecation, Mandated, publish immediately to block the affected build.
