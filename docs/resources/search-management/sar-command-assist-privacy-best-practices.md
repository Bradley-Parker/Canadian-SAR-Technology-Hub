---
title: "SAR Command Assist (SCA) Privacy & Data Security Best Practices"
description: "Field-tested best practices for managing data security, cloud sync, police file handoff, and subject PII sanitization in SAR Command Assist (SCA)."
category: "Search Management"
jurisdiction:
  - "National"
tags:
  - "sar-command-assist"
  - "privacy"
  - "search-management"
maintainer: "Canadian SAR Tech Hub Community"
date_updated: 2026-10-24
---

# SAR Command Assist (SCA) Privacy & Data Security Best Practices

[SAR Command Assist (SCA)](sar-command-assist.md) has become an essential tool for Canadian Ground Search and Rescue (GSAR) Incident Management Teams (IMTs). It automates ICS paperwork, coordinates team assignments, and manages operational periods in real time.

Because SCA handles sensitive search data—including missing subject profiles, medical notes, team logs, and investigative clues—proper data security and privacy management are critical.

This guide outlines practical, field-proven information management habits gathered from operational Standard Operating Procedures (SOPs) across Canadian SAR jurisdictions. It explains how to collaborate safely during a search, deliver official records to police, and permanently sanitize files before long-term storage.

!!! important "Best Practice Guide vs. Local SOPs & Provincial Policies"
    These recommendations reflect common field practices developed across multiple Canadian ground search teams and partner agencies. **They are an educational best practice guide, not a formal Standard Operating Procedure (SOP).**

    Privacy laws (such as provincial FOIP, FIPPA, or ATIPP acts), provincial association standards (e.g., BCSARA, OSARVA, etc.), and agreements with your local Police of Jurisdiction (RCMP, OPP, Sûreté du Québec, or municipal police) always take precedence. If your jurisdiction has specific data-handling policies, always follow their directions.

---

## 1. Data Security & Storage Requirements

SCA gives Incident Management Teams flexible options for sharing data between computers—both within an Incident Command Post (ICP) and over the internet. Understanding the distinction between **live collaboration** and **long-term storage** is essential.

### Internet Sync is for Collaboration ONLY, NOT Long-Term Storage

When a search requires remote collaboration (such as bringing in off-site search managers or coordinating with a regional coordination centre), SCA offers an optional **Internet Sync** feature.

!!! warning "Sync Servers Are Not Data Archives"
    **SAR Assist Internet Sync is strictly designed for live operational collaboration between active incident management devices during a task. It is NOT a suitable long-term data storage platform.**

    Data is **NOT** maintained long-term on the sync server:

    - **Regular Server Purge**: Any task data stored temporarily on the cloud sync server is automatically deleted on a regular basis. 
    - **Canadian Hosting**: Internet Sync collaboration operates through a cloud-based Microsoft Azure server physically located within Canada, protected by 256-bit end-to-end encryption. The server stores only encrypted data blocks and cannot read incident contents.
    - **Never Rely on Cloud Sync for Backup**: Teams must never treat the cloud sync server as a backup, an archive, or a repository for past searches.

### Where Master Files Must Live (Local Hard Drives)

To ensure operational control, chain of custody, and privacy compliance:

- **Local IMT Hard Drives**: Master SCA incident files must be maintained directly on the local hard drives of the GSAR Incident Management Team (IMT) computers running the command post or other long-term approved team storage.
- **Local Network Collaboration (LAN Sync)**: Whenever possible, collaborate across command post computers using SCA's built-in Local Area Network (LAN) mode. LAN sync shares the live task across your command post Wi-Fi or router without routing any data over the public internet. This keeps all subject data within the physical perimeter of your ICP (and works offline).

### Search Manager Responsibility

The **Search Manager / Incident Commander** is responsible for ensuring all required data cleanups and file deletions are completed at the conclusion of each search.

This includes:
1. Confirming that all temporary internet sync sessions are concluded and disconnected.
2. Ensuring that all personnel—including searchers, field team leaders, and command staff—delete retained incident data, downloaded briefing sheets, and task photos from their personal and team devices (laptops, tablets, and mobile phones) where not needed for the purposes of the task.

---

## 2. Closing the Task: Official Documentation Handoff to Police of Jurisdiction (POJ)

Ground search teams operate under the authority and direction of a tasking agency—usually the Police of Jurisdiction (POJ) or incident tasking authority (e.g., RCMP, OPP, Sûreté du Québec, municipal police, or Parks Canada).

When field operations conclude, formal legal and investigative documentation must be delivered directly to the POJ/IC for the official case file and potential court or coroner proceedings.

### Generating the Official SCA PDF Package

Upon conclusion of the task, generate a master summary PDF through [SAR Command Assist (SCA)](sar-command-assist.md) and transmit it electronically to the POJ/IC.

This official documentation package must contain:

- [x] **Incident Action Plans (IAPs)** for all operational periods.
- [x] **Briefings (SMEAC)** for all operational periods.
- [x] **Team assignments and debriefs (ICS 204)** for all operational periods.
- [x] **Position logs and communications logs (ICS 309 / unit logs)**, if available.
- [x] **Clue documentation (ICS 204C / clue logs)**.

If your team also used [CalTopo](../mapping-gis/caltopo.md) for live mapping during the task, export your completed search tracks and clue waypoints as a standard GPX, KML, or GeoJSON package to accompany the SCA PDF for the police investigator.

---

## 3. Sanitizing Records Before Long-Term Storage (The 'Finish Incident' Step)

After the official documentation package has been transmitted to the Police of Jurisdiction, SAR teams often keep an archived copy of the incident for internal operational analysis, search theory research, training debriefs, and tracking annual volunteer service hours.

However, **ground SAR teams must never retain sensitive citizen personal information indefinitely on team or personal computers.**

### Mandatory Subject PII Deletion

Prior to long-term storage of any SCA data on SAR team devices, all **Personally Identifying Information (PII)** related to the subject(s) must be permanently deleted from all SCA entries, including profiles, briefings, notes, and attachments:

- **Subject full name**
- **Date of birth and exact age**
- **Home address and phone numbers**
- **Subject photographs**
- **Any other identifying information** (employer notes, vehicle license plates, personal medical details, or family contact records)

### How to Strip PII in SCA ('Finish Incident')

Stripping this data is built directly into [SAR Command Assist](sar-command-assist.md) through a dedicated feature:

```
Finish Incident
```

1. Open the completed incident file in **SAR Command Assist**.
2. Click the **Finish Incident** option in the top right (by Operational Period selection).
3. Select the **Secure** tab in the top navigation menu.
4. Follow the prompt to permanently purge subject identifying information.

### What 'Finish Incident' Does

The **Finish Incident** tool permanently strips all personal subject identifiers while **preserving all operational search records**:

| What is Permanently Deleted | What is Preserved for Team Records |
| :--- | :--- |
| • Subject name and nicknames | • Search segment boundaries and task numbers |
| • Date of birth, age, and phone numbers | • Team assignments and debrief notes (ICS 204) |
| • Home address and location notes | • Volunteer search hours and attendance records |
| • Uploaded photographs and personal media | • Communications logs and radio check-in records |
| • Personal medical and behavioural notes | • Weather observations, equipment lists, and timelines |

This enables your team to preserve a complete operational history for reporting, provincial funding, and training review without retaining private citizen data on team hard drives.

---

## Operational Checklist: Data Security & Incident Closeout

Follow this checklist at the command post when closing out any search:

### During Active Operations
- [ ] **LAN First**: Use Local Area Network (LAN) sync for multiple laptops in the command post whenever possible.
- [ ] **Collaborative Internet Sync**: If using Internet Sync, share the session key only with verified command personnel. Remember that sync is for live collaboration, not storage.
- [ ] **Local Master Files**: Ensure working files are saved directly to local IMT hard drives (Not just SCA Sync servers).

### At Incident Conclusion
- [ ] **Deliver Police Package**: Transmit the complete SCA PDF package (IAPs, briefings, ICS 204 assignments/debriefs, comms logs, and clue documentation) to the POJ/IC.
- [ ] **Deliver GIS Data**: Export searcher tracks and clue coordinates (GPX/GeoJSON) to the POJ if requested.
- [ ] **Lock Down CalTopo**: Set shared operational CalTopo maps to **Private**.
- [ ] **Run 'Finish Incident'**: In SCA, click **Finish Incident** and go to the **Secure** tab to permanently strip all subject PII before archiving the file.
---

## Related Resources

- [:material-clipboard-text-clock: SAR Command Assist (SCA) Overview](sar-command-assist.md): Overview of features, ICS forms, reflex tasking, and setup walkthroughs.
- [:material-shield-account: CalTopo Privacy & Information Management Best Practices](../mapping-gis/caltopo-privacy-best-practices.md): Guidance on protecting subject privacy, clue coding, and permission roles on cloud maps.
- [:material-map-legend: CalTopo Incident Map Template & Folder Standard](../mapping-gis/caltopo-sar-incident-template.md): Recommended folder hierarchy and GeoJSON templates aligned with SCA map exports.

---

## Thanks & Credits

These information management practices reflect operational Standard Operating Procedures and data governance policies developed by Canadian Ground Search and Rescue teams, search managers, and partner police services across Canada. 
