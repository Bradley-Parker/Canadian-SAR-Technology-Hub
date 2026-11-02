---
title: "CalTopo (SARTopo) Overview"
description: "A plain-language guide to CalTopo and SARTopo for Canadian Ground SAR teams, covering offline maps, team pricing, and key features."
category: "Mapping & GIS"
jurisdiction:
  - "National"
tags:
  - "mapping"
  - "caltopo"
  - "overview"
maintainer: "Canadian SAR Technology Hub"
date_updated: 2026-10-24
---

# CalTopo (SARTopo) Overview

**CalTopo** is an online and offline mapping platform built specifically for backcountry travel, wilderness navigation, and search and rescue (SAR) operations. Across Canada, hundreds of volunteer Ground SAR teams rely on it every week at the Incident Command Post (ICP) and in the field to plan search assignments, track ground teams, and print clear paper maps.

This guide gives a quick, plain-language overview of what CalTopo is, how it works, and what a Canadian SAR Manager needs to know before setting it up for their team.

---

## CalTopo vs. SARTopo: Are They Different?

**No. They are the exact same platform.**

You will often hear searchers in Canada use the names *CalTopo* and *SARTopo* interchangeably. Here is why:

- **The History:** SARTopo originally started as a search-and-rescue project created by developer Matt Jacobs. Over time, the developer merged CalTopo and SARTopo into one unified codebase and system.
- **The Websites:** If you go to `caltopo.com` or `sartopo.com`, you log in with the exact same account, see the same maps, and use the same data.
- **The Only Difference:** When you open a map at `sartopo.com`, it turns on search-and-rescue tools by default (such as search segments, clue markers, and search range rings). When you open `caltopo.com`, it opens in standard outdoor recreation mode.
- **You can switch anytime:** Inside any map, you can turn SAR tools on or off by clicking the gear icon or configuration menu in the left sidebar.

Whether your team calls it CalTopo or SARTopo, you are using the same tool.

---

## Why Canadian Ground SAR Teams Use It

CalTopo has become one of the most widely adopted mapping tools in Canadian search and rescue because it focuses on practical field needs:

### 1. Canadian Topo & Satellite Layers
CalTopo includes high-detail Canadian mapping sources, including:

- **NRCan CanMatrix & Toporama:** Official Canadian government topographic maps showing contour lines, elevations, logging roads, and waterways.
- **High-Resolution Satellite Imagery:** Clear aerial views to inspect forest canopy, cut blocks, wetlands, and recent developments.
- **Shaded Relief & Slope Shading:** Highlights steep cliffs, avalanche terrain, and gullies so team leaders can spot hazards before sending members into rough country.
- **Public Land & Forest Data:** Useful overlays for identifying crown land, park boundaries, and private property lines.

### 2. Live Team Collaboration
Multiple people can open and edit the same map at the exact same time:

- A Search Manager at the command trailer can draw a search box.
- A Planning Officer across the room (or a mutual aid coordinator in another town) sees the new search box appear on their screen within seconds.
- A field team reporting a clue over VHF radio can have their clue marker placed instantly by the radio operator.

### 3. Built-In Search & Rescue Tools
CalTopo includes tools tailored specifically for lost-person searches:

- **Search Segments:** Draw search areas with automatic size calculations (acres, hectares, square kilometers).
- **Range Rings:** Draw distance rings around the Last Known Point (LKP) or Initial Planning Point (IPP) to quickly see standard travel distances for lost persons.
- **Bearing Lines & Triangulation:** Plot compass bearings from multiple callers or cell tower azimuths to find an estimated location.
- **Custom Map Printing:** Generate high-resolution PDF maps with UTM, MGRS, or Lat-Long grid lines. Maps include scale bars and printable coordinate rulers so field searchers with compasses can navigate safely.

### 4. Field Tracking
Search managers can see where teams are searching in near real-time:

- **CalTopo Mobile App:** Searchers carrying smartphones can record and share their live track.
- **Garmin inReach & Satellite Messengers:** Direct feed connections allow search managers to see inReach devices moving across the map, even far beyond cell service.
- **Radio & GPS Bridges:** Integrates with automated tools like an APRS gateways to plot radio and GPS tracks directly onto the command map.

---

## Using CalTopo Offline (Zero Cell Coverage)

Much of the Canadian wilderness has no cellular reception. CalTopo handles remote operations in two practical ways:

### 1. Offline Mobile App (iOS & Android)
Searchers can download base maps, topo layers, and satellite imagery to their phone before leaving the hall or while connected to Wi‑Fi at the command post. [CalTopo Mobile App Offline](https://training.caltopo.com/all_users/mobile/offline)

- In the woods, the phone's internal GPS works without any cellular connection.
- Searchers can view their position, check their assigned search boundary, mark waypoints, and record tracks in airplane mode.
- When the searcher returns to cell range or connects to the command post Wi‑Fi, the app automatically syncs all logged tracks and waypoints back to the master incident map.

### 2. CalTopo Stand‑Alone Server (Command Trailers)
For major operations in deep valleys or remote regions with zero internet, teams can run CalTopo completely offline. [CalTopo Desktop](https://training.caltopo.com/all_users/desktop)

- CalTopo offers a local server software package that runs on a laptop, mini PC, or local network box inside a command trailer.
- The command post broadcasts its own local Wi‑Fi hotspot (using a simple travel router or vehicle router).
- Command staff connect their laptops and tablets to the trailer's Wi‑Fi and collaborate on the local map with no external internet connection required.

---

## Team Accounts & Volunteer Pricing

While individual searchers can create basic personal accounts, most Canadian SAR teams set up a **CalTopo Team Account**.

### Why Get a Team Account?
- **Shared Team Map Library:** Incident maps belong to the SAR organization rather than an individual member's personal email. When leadership changes, maps remain accessible to the team.
- **Member Management:** Team administrators can easily invite recruits, assign team roles, and remove members who leave.
- **Shared Offline Maps:** Team members get access to download high‑resolution satellite and topo layers to their mobile devices for offline deployment.
- **Group Tracking:** Simplifies setting up live tracking for team smartphones and shared satellite communicators.

### Preferred Pricing for Volunteer Teams
CalTopo offers discounted, preferred annual pricing specifically for all‑volunteer Ground Search and Rescue groups.

- **Why Get a Team Account?**
- **Preferred Pricing:** Discounted rates for all‑volunteer Ground SAR groups.
- **Pricing Model:** Annual flat‑rate based on team size, making it affordable for community‑funded volunteer societies.

To explore current pricing or apply for volunteer rates, visit the official [CalTopo Teams Page](https://caltopo.com/teams).

---

## Helpful CalTopo Guides on This Hub

<div class="grid cards" markdown>

-   :material-map-legend:{ .lg .middle } **[CalTopo Incident Map Template](caltopo-sar-incident-template.md)**

    ---

    A standardized incident folder structure (Planning, Operations, Resources, Clues) with downloadable Clean and Guided GeoJSON templates ready for your next callout.

    [:material-arrow-right: View Template Guide](caltopo-sar-incident-template.md)

-   :material-shield-account:{ .lg .middle } **[CalTopo Privacy & Information Management](caltopo-privacy-best-practices.md)**

    ---

    Field‑tested guidelines for protecting subject privacy, using secure clue codes, managing map permissions, and handling cross‑border data storage.

    [:material-arrow-right: View Privacy Guide](caltopo-privacy-best-practices.md)

-   :material-desktop-tower-monitor:{ .lg .middle } **[SAR Command Assist (SCA)](../search-management/sar-command-assist.md)**

    ---

    A free Windows command tool that connects directly to CalTopo maps to automate ICS paperwork, task assignments, and team sign‑in.

    [:material-arrow-right: View SAR Command Assist Guide](../search-management/sar-command-assist.md)

</div>

---

## Official Links & Resources

- **Official Website:** [caltopo.com](https://caltopo.com) / [sartopo.com](https://sartopo.com)
- **Official Documentation & User Guide:** [CalTopo Knowledge Base](https://training.caltopo.com)
- **First Responder / Team Information:** [CalTopo for First Responders & Teams](https://caltopo.com/teams)
