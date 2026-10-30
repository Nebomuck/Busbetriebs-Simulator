# 🚌 Depot Simulator for openOMSI

🇩🇪 [Deutsch](README.md) · 🇬🇧 **English**

Run your own bus company on an OMSI 2 map, and drive its duties yourself in
[openOMSI](https://github.com/turbo-devv/openOMSI).

You dispatch buses and drivers to the map's real timetable. You keep the fleet running with fuel
station, bus wash and workshop, win tenders and keep an eye on the finances. Any duty can be left to
the simulation or taken over by you. In that case the simulator starts openOMSI directly with your
bus, line and tour, and the two stay in sync. With friends you run the depot together, with roles,
company radio and a shared openOMSI server.

> **Note:** The program's user interface is currently in German.

---

## Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Features](#features)
- [Driving yourself in openOMSI](#driving-yourself-in-openomsi)
- [Playing together](#playing-together)
- [What the simulator does to your installation](#what-the-simulator-does-to-your-installation)
- [Questions and problems](#questions-and-problems)

## Requirements

- **Windows 10 or 11**
- **OMSI 2** (Steam). The simulator reads maps, timetables and buses from it.
- **openOMSI**, only if you want to drive yourself.

Players without OMSI 2 can still join and work as dispatchers.

## Installation

1. Download `betriebshof.exe` from [Releases](../../releases/latest).
2. Put it in any folder and run it. There is no installer.
3. The simulator finds OMSI 2 and openOMSI on its own. If it can't find OMSI 2, select the folder
   that contains `maps` and `Vehicles`.

On first start, an **introductory tour** (single or multiplayer) walks you through every button and
tab.

**Updates** arrive on their own. On start the simulator checks this page for a new version and shows
what's new. One click replaces the program file, verified against GitHub's SHA-256 checksum. Your
companies stay untouched.

## Features

### Your company

- **Any OMSI 2 map** with a timetable, including maps from openOMSI mods. Tours, trips, stops,
  fleet numbers and number plates come from the map.
- **Career mode**: your own company with name and logo, one tour and enough money for a used bus.
  Grow through tenders, company levels and daily goals.
- **Free play**: a full depot with every bus, driver and line of the map.
- **Three difficulty levels**. On "Realistic" you pay today's actual diesel price at the pump.
- **Real calendar** with the public and school holidays of your German state. Tours only run on
  their operating days, and openOMSI gets the same date.
- **Several companies** side by side, with an overview in the main menu.

### Dispatch and operations

- Assign buses to tours and drivers to duties, by hand or automatically. Rest periods, working-time
  limits, articulated-bus licences and type training are respected.
- **One bus per duty**: at a relief point, a different bus can take over.
- **Driver changes en route**, with control-centre messages for the players involved.
- **Disruptions**: roadworks, diversions, accidents and police operations delay lines. You can
  counter them with standby buses or cancelled trips.
- **Breakdowns and defects**: buses wear out. Drivers find defects at the departure check or on the
  road, and serious ones take the bus out of service.
- **Temp-driver agency** when a duty has no driver.
- **Live map** with streets, your line network and every bus on the road. Players appear at their
  real position from openOMSI.

### Fleet and depot

- **Depot plan** with fuel station, bus wash and workshop, each with limited bays and queues.
- **Buy used, buy new, lease or rent**. Every installed bus is available, including mods, in the
  livery of your choice.
- Roadworthiness tests, inspections, repairs and an automatic workshop.
- **Advertising** on your buses brings daily income.
- **Expansion**: more parking spaces, fuel pumps, wash lanes and workshop pits.

### Staff and passengers

- Applications, wages, holiday requests, satisfaction and sick days.
- Training: articulated-bus licence, type training, customer service and fuel-efficient driving.
- **Ticket inspectors** against fare dodgers.
- **Reputation from 0 to 5 stars**: passenger complaints and praise. A good reputation brings more
  passengers and a quality bonus.

### Finances

- Per-kilometre payments from the transport authority, fares, fines and advertising, against diesel,
  staff, workshop and depot costs. Everything is broken down item by item.
- **Tenders** against competitors, with contract term and price per kilometre.
- Loans, leasing and rental; contract penalties for cancelled trips.

## Driving yourself in openOMSI

- **One click starts openOMSI** with map, bus (fleet number, plate, livery, dirt), depot file,
  line, tour, time, date and your driver profile. No launcher, no menu.
- **Clocks in sync**: the simulation follows openOMSI's clock. Pause and time acceleration apply to
  both.
- **In-game board**: shows your current trip, next stops with expected times, the gap to the bus
  ahead and behind, control-centre messages and disruptions on your line. Buttons let you report to
  the control centre or report a defect.
- **Defects you can feel**: doors that reopen, engine in limp mode, failed alternator, broken
  indicator or low beam.
- **Real ticket sales**: tickets you sell on the bus count as revenue, at the map's own prices.
- **Journey log**: delays and trips driven are taken over from openOMSI.
- **Stop early**: if the shift is too long, the simulation drives the rest.
- **Life**: your own account with wage, flat, car, leisure, rest and mood.

## Playing together

- **Join by code**: no Steam and no port forwarding needed. Via Cloudflare, the host's IP address
  stays hidden.
- **Roles**:
  - The *boss* decides on purchases, staff and lines.
  - *Dispatchers* assign buses and drivers.
  - *Drivers* sign up for duties.
- **Company radio** with push-to-talk, control-centre priority, individual calls and call requests.
  The keys also work while openOMSI is in the foreground.
- **Shared openOMSI server**: the simulator starts it with the company's map, date and time, so
  everyone drives in the same world.
- **Personnel files** show who turns up for their duties on time.

## What the simulator does to your installation

- **OMSI 2 is only read**: maps, timetables, buses, liveries and ticket packs.
- In **openOMSI** the simulator only creates its own files:
  - the plugin `Plugins\betriebshof.lua` (clock, board, tickets, defects) with its data folder;
  - if needed, an extended `Holidays.txt` in openOMSI's own map folder.

  It never overwrites other files, and never your existing driver profiles.
- Saves, profiles and settings are stored in `%APPDATA%\BetriebshofSimulator`.

## Questions and problems

Found a bug or have an idea? Open an [issue](../../issues). Helpful details:

- the version (shown in the main menu under "Updates");
- the map and the bus;
- what you did and what happened.

---

© 2026 Nebomuck. All rights reserved. See [LICENSE.md](LICENSE.md).
OMSI 2 is a product of MR-Software / Aerosoft, and openOMSI is an independent project. The Depot
Simulator is not affiliated with either.
