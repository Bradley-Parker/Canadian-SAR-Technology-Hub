---
title: Tags & Taxonomy Standard
description: Standardized categories, tags, and jurisdiction labels for Canadian SAR resources.
---

# Tags & Taxonomy Standard

To ensure in-browser search and filtering remain clean and consistent, please use these standard categories, jurisdiction codes, and common tags when tagging resource pages.

---

## 1. Categories
Every resource belongs to one of these primary categories:

| Category | Description |
| :--- | :--- |
| **Mapping & GIS** | SARTopo/CalTopo, QGIS, GPS units, mapping layers, grid coordinates, datum standards. |
| **Communications** | VHF/UHF repeaters, radio codeplugs, satellite messengers, field networks, ICS comms plans. |
| **Search Management** | Lost Person Behavior, search theory, probability of detection (POD), incident command templates. |
| **Field Hardware** | RPAS/drones, night vision, forward-looking infrared (FLIR), trackers, power systems. |
| **Training & Standards** | Provincial SAR standards, CSA Z1620, operational checklists, training drills. |
| **Medical & Evacuation** | Wilderness first aid, hypothermia protocols, stretcher packaging, evacuation rigs. |

---

## 2. Jurisdictions
Use Canadian standard abbreviations in the `jurisdiction` frontmatter list:

- `National` (Applies across all Canadian jurisdictions)
- `BC` (British Columbia)
- `AB` (Alberta)
- `SK` (Saskatchewan)
- `MB` (Manitoba)
- `ON` (Ontario)
- `QC` (Quebec)
- `NB` (New Brunswick)
- `NS` (Nova Scotia)
- `PE` (Prince Edward Island)
- `NL` (Newfoundland and Labrador)
- `YT` (Yukon)
- `NT` (Northwest Territories)
- `NU` (Nunavut)

---

## 3. Tagging Discipline & Standards

Tags on the hub are intentional and structured so that in-browser search and tag menus remain clean and genuinely useful.

Aim for **up to 4 tags** per page (one per primary dimension), with an optional 5th tag only when there is a strong operational reason (e.g. highlighting that an app is `free` or `open-source`). Avoid going higher than 4 tags without a solid reason.

### Dimension 1: Category Tag (What broad domain is this?)
Allows users browsing or filtering by tags to discover resources by domain:
- `mapping`, `communications`, `search-management`, `field-hardware`, `training-standards`, `medical-evacuation`, `team-admin`

### Dimension 2: Tool / Platform (What is it about?)
Specific software, hardware, or platform covered by the resource:
- `caltopo`, `avenza`, `qgis`, `d4h`, `sar-command-assist`, `garmin`, `inreach`, `zoleo`, `rpas`, `flir`

### Dimension 3: Role / Operational Audience (Who uses it?)
The primary SAR practitioner role:
- `search-manager`, `ground-searcher`, `team-leader`, `incident-commander`, `equipment-officer`, `team-admin`

### Dimension 4: Resource Type (What kind of document is it?)
Only use one of these four standardized resource types:
- **`template`**: Downloadable operational assets, folder templates, map layers, or ICS sheets ready for mission use.
- **`guide`**: Step-by-step procedural how-tos, configuration guides, or field SOPs.
- **`review`**: Candid, practitioner-tested evaluations and field benchmarks of gear or software.
- **`overview`**: High-level introductions to a platform, tool, or system.

### Dimension 5: Special Descriptors (Optional 5th Tag)
Used sparingly when it provides major filtering value for teams:
- `free`, `open-source`, `offline-first`, `privacy`

---

### Tagging Rules
1. **Target 3 to 4 Tags**: Aim for one tag per core dimension (e.g., `["mapping", "avenza", "overview"]` or `["mapping", "caltopo", "search-manager", "template"]`).
2. **Limit**: Do not exceed 4 tags without good reason (such as adding `free` or `open-source`).
3. **No Fluff or Arbitrary Tags**: Never use vague junk tags like `handouts`, `tips`, `team-assignments`, or `forms`.
4. **Format**: All lowercase, hyphen-separated (e.g., `search-manager`, `open-source`).

