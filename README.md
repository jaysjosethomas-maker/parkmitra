# ParkMitra — Urban Parking Operating System

> **"Find it. Park it. Trust it."**  
> *The Connected Urban Parking Network for Indian Cities.*

ParkMitra is an evolution of the Spotit hackathon prototype into a full, production-quality parking marketplace, trust layer, and civic parking intelligence operating system.

It bridges **Drivers**, **Parking Hosts/Owners**, **Parking Operators**, and **Municipal Civic Authorities (BBMP)** into a cohesive, trusted urban infrastructure platform.

---

## 🚀 Key Platform Features

- **Four Integrated Product Surfaces**:
  1. **Driver OS**: Destination search across Bengaluru urban hubs, blueprint spatial map, confidence badges, geofence + QR check-in, active session management, and Continuity failure recovery.
  2. **Host / Owner OS**: 9-step space onboarding wizard, real-time occupancy monitoring, and opt-in dynamic pricing multipliers (1.0x to 1.5x).
  3. **Civic Command Centre (BBMP)**: Urban command centre with real-time ward telemetry, ANPR corridor tracking, parking zones, and citizen street violation triage.
  4. **Admin Operations**: Append-only audit logs, under-review lot reinstatements, and multi-modal dispute resolution with live reliability delta previews.

- **The Continuity Engine**:
  - Treats trust as a first-class citizen.
  - Implements an append-only `ContinuityEvent` ledger.
  - Never silently deletes or fails bookings; freezes them as `DISPUTED` to preserve evidence.
  - Enforces the capacity invariant `0 <= availableSpaces <= totalSpaces`.
  - Automatically identifies nearby high-confidence alternatives and issues simulated goodwill credits.

- **Design System & Visual Language**:
  - Follows the uploaded ParkMitra Pitch Deck: 80% Modern Mobility UX + 20% Architectural Blueprint Visual Language.
  - Color Tokens: Primary Deep Blue (`#0B4057`), Secondary Blue (`#1F617C`), Gold (`#D5A343`), Terracotta (`#C77F6C`), Slate (`#657783`), Background (`#F5F7F6`), Surface (`#FFFFFF`).
  - Subtle technical gridlines, registration marks (`⌖`, `+`), coordinate annotations (`12.9352° N, 77.6245° E`), and rectangular technical cards.

- **50+ Realistic Bengaluru Parking Nodes**:
  - Spans 5 core urban zones: **Koramangala**, **Indiranagar**, **HSR Layout**, **BTM Layout**, and **Jayanagar**.
  - Includes government multi-level complexes, private residential driveways, commercial garages, community lots, and enforced no-parking zones.

---

## 💻 Quick Start & Running the Application

### Option A: Launch the Standalone Application (Immediate & Zero-Dependency)
Open [index.html](file:///c:/Users/user/Downloads/Parkmitra/index.html) directly in any modern web browser (Edge, Chrome, Firefox).
- All 4 surfaces (Driver, Host, Civic, Admin) are fully functional.
- The Architectural Blueprint Map Engine runs 100% offline and locally.
- Test the 3 master demo scenarios directly from the top header dropdown:
  - **Scenario 1**: Driver Jays (KA01XX1234) End-to-End Booking Loop
  - **Scenario 2**: Parking Failure & Continuity Engine Recovery
  - **Scenario 3**: Host 9-Step Onboarding & Dynamic Pricing Monetization

### Option B: Backend & Spotit Codebase
The evolved codebase is located under [`Spotit-main/`](file:///c:/Users/user/Downloads/Parkmitra/Spotit-main):
- **Database Schema**: [`Spotit-main/backend/prisma/schema.prisma`](file:///c:/Users/user/Downloads/Parkmitra/Spotit-main/backend/prisma/schema.prisma) with extended models for `ParkingZone`, `CivicViolation`, and `DynamicPricingRule`.
- **Bengaluru Seed**: [`Spotit-main/backend/prisma/seed.ts`](file:///c:/Users/user/Downloads/Parkmitra/Spotit-main/backend/prisma/seed.ts) with 50+ real-world Bengaluru nodes.
- **Continuity Engine**: [`Spotit-main/backend/src/modules/continuity/`](file:///c:/Users/user/Downloads/Parkmitra/Spotit-main/backend/src/modules/continuity/).

---

## 📚 Technical Documentation Suite

1. **System Architecture**: [PARKMITRA_ARCHITECTURE.md](file:///c:/Users/user/Downloads/Parkmitra/docs/PARKMITRA_ARCHITECTURE.md)
2. **API & State Machines**: [PARKMITRA_API_AND_STATE_MACHINES.md](file:///c:/Users/user/Downloads/Parkmitra/docs/PARKMITRA_API_AND_STATE_MACHINES.md)
3. **Data Model & Entity Dictionary**: [PARKMITRA_DATA_MODEL.md](file:///c:/Users/user/Downloads/Parkmitra/docs/PARKMITRA_DATA_MODEL.md)
4. **Test Plan & Master Verification Runbook**: [PARKMITRA_TEST_PLAN.md](file:///c:/Users/user/Downloads/Parkmitra/docs/PARKMITRA_TEST_PLAN.md)
5. **Roadmap & Known Limitations**: [PARKMITRA_ROADMAP_AND_LIMITATIONS.md](file:///c:/Users/user/Downloads/Parkmitra/docs/PARKMITRA_ROADMAP_AND_LIMITATIONS.md)
6. **Design System Specification Artifact**: [PARKMITRA_DESIGN_SYSTEM.md](file:///C:/Users/user/.gemini/antigravity/brain/fa2d8523-759c-4051-b96d-e74c71433efd/PARKMITRA_DESIGN_SYSTEM.md)
