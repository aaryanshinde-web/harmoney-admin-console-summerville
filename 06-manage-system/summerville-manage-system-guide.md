_Summerville Admin Console  ›  Manage System_

# Manage System

> Configure platform-level system preferences, limits, holiday calendars, and downstream integrations that apply to every member of the Summerville digital channel.

## Summary

Manage System is the platform-operations module of the Summerville Admin Console — the place where Summerville tells the commercial digital channel what is about to happen to it. Unlike Manage Content, which governs what a member reads on screen, Manage System governs the state of the platform itself: when the platform, a channel, or a module will be unavailable, and when a specific mobile-app version will stop being supported. It is the operations-facing twin of the marketing-facing notification module, specifically designed for platform events that have a start and end time rather than for messages that simply need to be broadcast.

The left-hand navigator opens to two surfaces. System Outages is the register of scheduled and completed outage events with Channel, Title, Outage Type, Frequency, Start Date, End Date, and Status columns — each entry is a first-class event that the platform uses to gate member actions and drive the outage banner in every channel. App Deprecation manages the lifecycle of mobile-app versions — which platform, which build, whether the upgrade is Recommended or Mandated, and the effective window communicated to members still on an old build. Manage System earns its keep against three concerns every commercial institution runs into weekly: planned-outage discipline, blast-radius control, and mobile-app lifecycle enforcement.

## Key Use Cases

Treasury Operations has a one-hour wire-cutoff change scheduled for next Saturday. The operator opens System Outages, clicks Add Outage, picks Module Specific with Module Type = Wire, uses One time, on with the exact Date & Time From/To, and enables Pre-Outage Reminders plus Post-Outage Notifications across Email and Push. The outage event gates wire initiation only in the scheduled window while leaving ACH, RTP, and the rest of the channel fully available to commercial customers.

The telephony team is cutting over to a new IVR provider and needs Voice banking disabled for 30 minutes. The operator opens Add Outage, picks Channel Specific with Channel = Voice, schedules the 30-minute window, and leaves Online and Mobile available. Channel Specific is the right control here — it keeps online and mobile channels servicing commercial customers during the cutover while isolating the Voice disruption to its actual blast radius.

Platform Engineering declares an incident and needs the commercial channel to reflect an immediate outage while Risk evaluates exposure. The operator opens Add Outage, leaves Outage Type on System Wide, switches Schedule Outage to Immediate, captures the title and message, and publishes. The Immediate option collapses the From/To picker to a single To field because the outage starts now, and the platform-wide banner fires before the first member page refresh.

After a quarter, Risk and Platform Operations reconcile every outage event that fired in the period against the change-management tickets that authorised them. The team opens System Outages, reviews the Completed rows, and matches each row's Channel, Outage Type, Frequency, and Start/End Date against the change ticket — because every outage is a first-class record, the reconciliation is deterministic rather than reconstructed from chat logs.

Information Security has decided that builds older than a certain version of the mobile app can no longer be supported due to a TLS or library issue. The operator opens App Deprecation, captures the Platform, sets Type of upgrade to Mandated, and submits — the Mandated path intentionally hides Start Date and End Date because a mandated deprecation is immediate and hard, and the member on the old build is blocked from the channel until they update.

## End-to-End Workflow

### Prerequisites

- Manage System role assigned to the operator via Manage Administrators.
- Change-management ticket or incident ticket approving the outage or deprecation event.
- For planned outages: agreed Date & Time window with the business unit and member-communications content approved.
- For App Deprecation: target Platform (iOS / Android) and the minimum supported build identifier confirmed with Mobile Engineering.

### Step-by-Step Flow

#### Step 1 — Open System Outages to review scheduled and completed events

From the Manage System navigator, click System Outages to land on the outage register. The register captures every outage as a first-class record with Channel, Title, Outage Type, Frequency, Start Date, End Date, and Status — and the timezone disclosure (All dates are in Pacific Standard Time) is displayed above the table so no reviewer ever has to guess which clock the window refers to.

![Step 1 — Open System Outages to review scheduled and completed events](img/ms-01-system-outages-list.jpg)

#### Step 2 — Open Add Outage and capture the baseline System-Wide event

Click Add Outage to open the form. The default shape is Outage Type = System Wide, Schedule Outage = One time, on, with Pre-Outage Reminders on and Outage Mode = Email — the conservative default for a credit union because it captures the broadest scope and the most reliable delivery channel, and you narrow the scope explicitly by switching the radio for specific outages.

![Step 2 — Open Add Outage and capture the baseline System-Wide event](img/ms-02-add-outage.jpg)

#### Step 3 — Toggle Schedule Outage to Immediate for an in-effect-now event

Toggle Schedule Outage from One time, on to Immediate — the Date & Time block collapses from a From/To pair to a single To field, because an immediate outage begins on publish and needs only an expected-restoration time. Use this shape during live incidents when Platform Engineering and Risk are deciding the restoration window in real time.

![Step 3 — Toggle Schedule Outage to Immediate for an in-effect-now event](img/ms-03-add-outage-immediate.jpg)

#### Step 4 — Pick Channel Specific to isolate Online, Mobile, or Voice

Switch Outage Type to Channel Specific — the form reveals a Channel radio row with Online, Mobile, and Voice, and a NOTE: All Modules marker that confirms every module on that channel is affected. This is the right scope when a single channel has a vendor dependency that needs to be taken down — typically a Voice IVR cutover or a Mobile SDK rollout — while leaving the remaining channels fully available.

![Step 4 — Pick Channel Specific to isolate Online, Mobile, or Voice](img/ms-04-add-outage-channel-specific.jpg)

#### Step 5 — Pick Module Specific for surgical outages against a single feature

Switch Outage Type to Module Specific — the form reveals a Module Type dropdown (Pay Bills, Wire, ACH, and so on), a plus icon to add sibling modules, and the Online / Mobile / Voice checkboxes that further scope which channels of that module are affected. This is the narrowest blast radius in the module and is the right shape for a planned Pay Bills maintenance window that should leave Wire, ACH, and RTP untouched.

![Step 5 — Pick Module Specific for surgical outages against a single feature](img/ms-05-add-outage-module-specific.jpg)

#### Step 6 — Open App Deprecation to manage mobile-build lifecycle

From the Manage System navigator, click App Deprecation to open the Mobile Banking Application Deprecation register. An empty No app deprecation to display state is the expected opening view when no deprecation campaign is currently scheduled, and the Add Deprecation Notification button is the entry point for every new lifecycle event.

![Step 6 — Open App Deprecation to manage mobile-build lifecycle](img/ms-06-app-deprecation-landing.jpg)

#### Step 7 — Capture a Recommended upgrade with Platform, Start Date, and End Date

Click Add Deprecation Notification and pick the Platform; leave Type of upgrade on Recommended — the form exposes Start Date and End Date pickers. A Recommended upgrade is the soft-nudge path: the member still has the old build available but is prompted to update during the window, which is the right shape for routine security patches and minor feature releases.

![Step 7 — Capture a Recommended upgrade with Platform, Start Date, and End Date](img/ms-07-app-deprecation-recommended.jpg)

#### Step 8 — Switch Type of upgrade to Mandated for a hard cut-off

Toggle Type of upgrade to Mandated — the Start Date and End Date fields disappear, because a Mandated deprecation is not a window, it is a hard cut-off that takes effect on publish. Use this path only when Information Security or Risk has decided that the old build can no longer be trusted on the platform, because a mandated upgrade will block any member still on an older build from completing authentication.

![Step 8 — Switch Type of upgrade to Mandated for a hard cut-off](img/ms-08-app-deprecation-mandated.jpg)
