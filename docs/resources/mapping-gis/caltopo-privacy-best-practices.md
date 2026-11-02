---
title: "CalTopo Privacy and Information Management Best Practices"
description: "Field-tested best practices for protecting personal privacy, managing clues, and securing maps when using CalTopo on SAR operations in Canada."
category: "Mapping & GIS"
jurisdiction:
  - "National"
tags:
  - "mapping"
  - "caltopo"
  - "search-manager"
  - "guide"
  - "privacy"
maintainer: "Canadian SAR Tech Hub Community"
date_updated: 2026-10-24
---

# CalTopo Privacy and Information Management Best Practices

[CalTopo](caltopo.md) (including SARTopo) is one of the most popular mapping tools used by Canadian Ground Search and Rescue (GSAR) teams. It makes it easy to sketch search areas, share live tracking, and organize field teams in real time.

Because CalTopo is a cloud-based service hosted on servers outside of Canada, any data entered into a map is transmitted and stored across borders. In addition, digital maps can be shared, screenshotted, or exported across many devices during an incident.

To protect missing subjects, volunteer searchers, and police investigations, many SAR organizations and Police of Jurisdiction (POJ) agencies recommend keeping sensitive personal details off online maps. This guide shares common, practical habits developed across Canadian teams to help you run an effective search while keeping personal information safe.

!!! important "Local and Agency Policy Always Comes First"
    These recommendations reflect common field practices used across Canadian SAR teams and police partners. **They are not a formal Standard Operating Procedure (SOP).** 

    Privacy laws (such as provincial FOIP, FIPPA, or ATIPP acts) and your local Police of Jurisdiction (RCMP, OPP, Sûreté du Québec, or municipal police) or tasking agency agreements always take precedence. If your provincial association or local police agency has specific data handling rules, always follow their guidance.

---

## The Core Rule: "Need to Map" vs. "Need to Know"

When adding any piece of information to CalTopo, ask one simple question:

> **"Does a field searcher or pilot need this written on their map to navigate or stay safe?"**

If the answer is no, keep it off the map:

- **Keep on the map**: Search boundaries, safety hazards, searcher tracks, initial planning points, clue locations, and staging areas.
- **Keep in secure command records**: Subject medical history, full names, home phone numbers, personal notes, and detailed police interview notes. 

Detailed records belong in secure incident management tools—such as [SAR Command Assist](../search-management/sar-command-assist.md)—or in paper ICS forms filed at the Incident Command Post (ICP).

---

## 1. Keep Personal Information Off the Map

Map names, folder names, marker labels, and comments should never include personal or identifying information. 

| ❌ Information to Keep Off the Map | ✅ What to Use Instead |
| :--- | :--- |
| **Subject full names** | Use operational roles like `"Subject"`, `"Missing Hiker"`, or the task number. |
| **Searcher and volunteer full names** | Use assignment numbers and initials (e.g., `104 JD`) or team callsigns. |
| **Police and agency member names or badge numbers** | Use organizational titles (e.g., `"POJ Liaison"`, `"Parks Warden"`). |
| **Dates of birth, ages, and gender** | Keep these in the briefing notes or SMEAC sheet at the ICP. |
| **Personal home addresses and phone numbers** | Keep contact information on your sign-in sheets and ICS-204 forms. |
| **Police or tasking agency file numbers** | Use your internal SAR task number (e.g., `Task 26-104`). |
| **Medical notes and behavioural profiles** | Share during verbal briefings; do not paste them into map notes. |

Using operational codes instead of personal names ensures that anyone viewing the screen—whether on a tablet in the field or on a projector at the command post—only sees what is strictly necessary to complete their assignment.

---

## 2. Use Safe, Non-Identifying Map Names

When you start a new map in CalTopo, give it an operational name that describes the search location without revealing the person's identity or police file numbers.

- **Safe Examples**:
    - `Task 26-104 - Mount Douglas`
    - `Mission 26-031 - Pine River`
    - `Training 2026-11 - Swiftwater Exercise`
- **Avoid**:
    - `Search for Jane Doe - Missing Child`
    - `RCMP File 2026-44829 - John Smith`

A clean, non-identifying map title prevents sensitive names from popping up in browser histories, shared links, or exported file downloads.

---

## 3. Photos and Media Attachments

CalTopo allows users to attach photos directly to map markers. While convenient, map attachments are easily downloaded, forwarded, or synced to the cloud.

As a general best practice, **avoid attaching the following to CalTopo maps**:

- Photos of the missing subject.
- Photos that clearly identify searchers or members of the public.
- Photos of personal effects (driver's licenses, wallets, or identifiable personal items).
- Photos of sensitive clues that are clearly tied to a specific individual.

If a photograph is operationally necessary (for example, showing searchers a high-resolution drone photo of an impassable canyon or a cliff hazard), verify that the image contains no personal data and ensure the upload aligns with directions from your search manager and Police of Jurisdiction.

---

## 4. Clue Management & Alphanumeric Codes

When searchers find an item in the field, plot the location using an **alphanumeric clue identifier** rather than a full written description.

### Recommended Clue Code Format

`Clue [Assignment Number]-[Clue Number]` or `Clue [Letter Code][Number]`

- `Clue 104-1` (Assignment 104, first clue found)
- `Clue 104-2` (Assignment 104, second clue found)
- `Clue A03` (Search Team Alpha, clue 3)

```
[Clue 104-1]
Time: 14:15
Found by: Team 104
Status: Documented & Flagged
(Detailed description filed in ICP Command Log)
```

Keep descriptive notes (such as `"Brown leather wallet with ID belonging to subject"`) in your command post documentation system or ICS forms, referencing only `Clue 104-1`. 

If a clue is later ruled out by the investigation, do not delete it from your map. Follow the [CalTopo Incident Map Template](caltopo-sar-incident-template.md) guidelines: move the marker into the `Clues - Discounted` folder and hide the folder visibility. This preserves the operational audit trail for police and coroner reports while keeping your live map uncluttered.

---

## 5. Map Security Settings & Permission Roles

CalTopo controls access using two layers: **Base Permissions** (who can access the map URL) and **Access Types / Roles** (what people are allowed to do once they open it). For complete technical details, consult the [CalTopo Map Sharing & Permissions Documentation](https://training.caltopo.com/all_users/share/permissions).

### The 4 Base Permissions in CalTopo

When saving or managing a map in CalTopo, you choose one of four base permission settings:

| Base Permission | How CalTopo Handles It | Ground SAR Operational Role |
| :--- | :--- | :--- |
| **URL** *(Default)* | Anyone who has or guesses the 5-digit map ID in the URL can view the map. | **Not recommended for active SAR operations.** Because 5-digit map URLs can be forwarded or guessed, avoid leaving sensitive search maps on default URL permissions. |
| **Secret** | The map cannot be opened by URL alone. You must generate specific shareable links or QR access codes to grant access. | **Recommended during active operations.** Keeps access strictly controlled. You can create different access codes with different operational roles for field searchers vs. command staff. |
| **Private** | Only visible to you or members logged into your team account. No one else can open it, even with the URL. | **Recommended once the mission ends.** Changing a completed map to Private immediately cuts off access for all previously shared field links and bookmarks. |
| **Public** | Indexed by Google and displayed on CalTopo's public "Shared Maps" layer. | **NEVER use for SAR operations.** Makes all map data searchable and viewable by the entire public. |

---

### The 3 Access Roles as They Apply to SAR

When sharing a **Secret** (or URL) map via a shareable link or QR code, CalTopo lets you assign one of three permission levels:

1. **Read (View Only)**
   - *What it allows*: Searchers can view map features, toggle folders, and view layers. They cannot add, edit, or delete any objects.
   - *SAR Field Role*: Ideal for partner agency liaisons, ICP display screens, dispatchers, or searchers using the map strictly for reference.
2. **Update (Add & Edit Own Objects)**
   - *What it allows*: Searchers can record tracks and drop waypoints (such as clues or hazards), and modify objects they added themselves. They **cannot** delete or modify planning boundaries, search segments, safety zones, or tracks recorded by other teams.
   - *SAR Field Role*: **The recommended role for ground search teams and field team leads.** It lets teams record live tracks and report clues without any danger of accidentally wiping out command planning layers.
3. **Write (Full Editing Access)**
   - *What it allows*: Complete control to add, edit, and delete any object or folder across the entire map.
   - *SAR Field Role*: **Strictly reserved for Incident Command, Planning Section, and the GIS / Mapping Officer.**

---

### Closing Down Access After the Incident

Once a search wraps up or active field operations end:

1. Open the map in CalTopo.
2. Open the **Map Details / Sharing** dialog.
3. Change the base permission to **Private**.

Switching to **Private** immediately revokes access for all shareable links and QR codes distributed during the task, preventing former participants from viewing the archived map after leaving the field.

---

## 6. Information Sharing & External Participants

During major searches, incident commanders frequently work with mutual aid teams, partner agencies, and spontaneous or convergent volunteers.

Before sharing map links outside your primary response organization:

- **Confirm with Incident Leadership**: Ensure map distribution is approved by the Search Manager and aligns with guidelines from the Police of Jurisdiction.
- **Mutual Aid Teams**: When briefing assisting SAR teams, issue them a dedicated **Update** link or QR code for their field searchers rather than sharing full administrative credentials.
- **Convergent Volunteers**: If spontaneous community volunteers are deployed for a hasty search:
    - **Option A (Static Maps)**: Hand out printed paper task maps or georeferenced PDFs (for Avenza Maps) covering their designated search block only.
    - **Option B (Separate "Public" Map)**: Set up a completely separate, secondary CalTopo map that contains only their designated search blocks and safety points—completely isolated from your master operational map, investigative clues, and team tracks *(see future hub best practice guide on convergent volunteer mapping)*.
    - **Never share your master operational map link or QR code with convergent volunteers.**

---

## 7. Working with SAR Command Assist (SCA)

Many Canadian ground search teams pair CalTopo with [SAR Command Assist (SCA)](../search-management/sar-command-assist.md) to manage tasks, team tracking, and ICS paperwork.

Because SCA and CalTopo can synchronize data, it is essential to understand what information travels between the two systems:

1. **Avoid Sensitive Text in Synced Fields**: When entering assignment notes or safety messages in SCA that synchronize automatically to CalTopo labels or descriptions, ensure you do not include subject medical details, phone numbers, or private notes.
2. **Review Synchronization Direction**: Where possible, consider using one-way synchronization (pulling tracks and recorded field data from CalTopo into SCA) so that sensitive command records created on your local ICP laptop are not automatically broadcast up to the cloud map.
3. **Periodically Check Sync Settings**: At the start of a training session or new operational period, double-check your synchronization configuration to confirm that only required operational layers (such as team assignments, hazards, and search tracks) are pushed to the live map.

For more details on setting up tasks and offline operations, see the [SAR Command Assist Guide](../search-management/sar-command-assist.md).

---

## 8. Recommended Naming Conventions

Using consistent names keeps your map clear, readable, and free of sensitive personal data:

| Feature Type | Standard Format | Good Examples | What to Avoid |
| :--- | :--- | :--- | :--- |
| **Searcher Tracks** | `[Assignment #] [Member Initials]` | `104 JD`<br>`217 BM`<br>`305 SP` | `John Doe Track`<br>`104 - Smith & Jones` |
| **Clue Markers** | `Clue [Assignment #]-[Clue #]` | `Clue 104-1`<br>`Clue 104-2`<br>`Clue A03` | `Clue - John's Jacket`<br>`Jane's Prescription Bottle` |
| **Assignment Areas** | `[Assignment Number or Code]` | `104`<br>`217`<br>`A03` | `Area behind Jane's house`<br>`RCMP Priority Zone 1` |
| **Map Name** | `[Task #] - [General Location]` | `Task 26-104 - Mount Douglas`<br>`Mission 26-012 - Bear Creek` | `Search for Bobby Smith`<br>`File 2026-18923 Missing Person` |

---

## Field Checklist: 60-Second Privacy Check

Before sharing your map link with field teams or projecting it at briefing, run through this quick 60-second check:

- [ ] **Map Title**: Is the map title free of subject names and police file numbers?
- [ ] **Labels & Folders**: Are all tracks and search polygons labeled with assignment codes or initials rather than full names?
- [ ] **Clue Descriptions**: Are clues identified by alphanumeric codes with sensitive investigative details stored in command post logs?
- [ ] **Attachments**: Are there zero unapproved personal photos or subject pictures attached to markers?
- [ ] **Sharing & Permissions**: Is the map set to **Secret** with role-based access (**Update** for field searchers, **Write** for command), and switched to **Private** when the call ends?
- [ ] **SCA Sync**: Have you verified that only necessary spatial features are synced to the cloud?

---

## Related Resources

- [:material-shield-lock: SAR Command Assist (SCA) Privacy & Data Security](../search-management/sar-command-assist-privacy-best-practices.md): SOP-derived guidelines on data storage, Canadian cloud sync, police package handoff, and scrubbing subject PII in SCA.
- [:material-map-legend: CalTopo Incident Map Template & Folder Standard](caltopo-sar-incident-template.md): Recommended folder hierarchy, clean GeoJSON templates, and operational layer setups for live missions.
- [:material-clipboard-text-clock: SAR Command Assist (SCA)](../search-management/sar-command-assist.md): Field-tested offline ICS paperwork management, operational period planning, and CalTopo integration.

---
