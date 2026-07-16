# PlatinumWings – Luxury Private Jet Booking Platform & Business System Design

[![Figma Design](https://img.shields.io/badge/Figma-Design_Workspace-F24E1E?logo=figma&logoColor=white)](https://www.figma.com/design/NN3OKzkvAveVYPv5JvkVvs/Login?node-id=0-1&p=f&t=pV9AmxhKATXMimds-0)
[![University](https://img.shields.io/badge/University-UNIPR-003C71?logo=university&logoColor=white)](https://www.unipr.it)
[![Obsidian](https://img.shields.io/badge/Obsidian-Notes-7C4DFF?logo=obsidian&logoColor=white)](https://obsidian.md)

This repository contains the complete Feasibility Study, System Architecture, UI/UX Wireframe specifications, and the interactive Figma design workspace for **PlatinumWings**. 

Developed as a B.Sc. project for the **Sistemi Informativi e Gestione d'Impresa (SIGI)** (Information Systems and Business Management) course at the **University of Parma**, this project bridges corporate software design, IT governance, and financial feasibility models with high-fidelity UI/UX design.

---

## ✈️ Corporate Context: PlatinumWings

Founded in **2014 in Parma** by four aviation enthusiasts, **PlatinumWings** started as a boutique private jet charter firm. The company built its reputation on luxury aircraft, high-quality bespoke services, and close client communication. Historically, to minimize IT costs, PlatinumWings operated on a manual, operator-led booking model. 

### The Obsolete Legacy Process
1. **Consultation**: Customers initiated bookings via a phone call with a dedicated operator team.
2. **Internal Coordination**: Operators checked jet availability using a basic internal coordination tool and checked vendor availability for culinary/chauffeur packages. Bookings were logged in a local DBMS.
3. **Financial Validation**: The operator collected itemized costs and submitted them to the accounting department.
4. **Approval**: Accounting drafted a quote for the executive manager, who reviewed it, applied potential discounts, and signed off.
5. **Payment**: The customer received an email containing the quote and bank details (IBAN). They had **three days to pay via bank transfer** (during which they held right of first refusal) or the booking was cancelled.

---

## ⚠️ The Digital Urgency: 5 Critical Bottlenecks

As the company scaled, this manual booking process created severe operational inefficiencies:
1. **Obsolete Booking Model**: Competitors offered instant online booking. The manual phone-based flow led to high client drop-off.
2. **Peak Season Saturation**: The 24/7 operator team was overwhelmed during busy holiday periods, reducing customer service quality.
3. **Outdated Management Software**: The legacy system's unintuitive UI led to long training times for new hires.
4. **Inter-departmental Bottlenecks**: Booking a single flight required manual hand-offs between operators, accounting, management, and external suppliers, slowing down response times.
5. **Zero Customer Autonomy**: Clients could not view available jets, choose optional packages, or see live pricing changes in real-time.

---

## 🚀 The Digital Transformation Strategy

To address these bottlenecks, PlatinumWings designed a unified digital ecosystem composed of:
1. **Customer-Facing Web & Mobile Apps**: Standardizing reservations with real-time feedback and dynamic cost transparency.
2. **Modern Admin Panel (Gestionale Admin)**: An intuitive, role-based CRM/ERP to streamline scheduling, analytics, support, and fleet logistics.
3. **Cloud Sourcing Transition**: Moving from local database management to a secure, outsourced cloud architecture (AWS/Google Cloud).

---

## 🗺️ System Architecture & User Flows

The UI/UX wireframes, documented in [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf), outline the application workflows:

### 1. Customer Booking Application (Web & iOS/Android)
* **Dynamic Search Box**: Book one-way, round-trip, or multi-city flights by selecting date, time, and passenger count.
* **Smart Fleet Selector**: High-fidelity gallery and specifications for the three distinct private jet categories in the catalog.
* **Real-Time Dynamic Pricing**: Cost estimations calculate pricing based on seasonal demand density (e.g., peak holidays like New Year's Eve), jet class, and operational relocation costs.
* **Bespoke Luxury Customizations (Add-ons)**:
  * *Private Chauffeur*: Bookable for the entire trip or specific days (with complimentary basic airport transfers included by default).
  * *On-board Dining*: Curated Italian, Mexican, or Japanese menus for the outbound and return journeys (with allergen logging).
  * *Exclusive Hotel Partnerships*: Integrated pop-ups linking to partner 5-star and 7-star luxury hotels offering exclusive client discounts.
* **Cost Optimization Engine**: A smart dialog recommending alternative travel dates (cheaper slots) to help passengers optimize flight costs.
* **Passenger & Security Details**: Unified entry for passenger titles, names, and fiscal codes, with options to save frequent flyers and request accessibility assistance.
* **Secure Checkout**: Consolidated payment overview integrated with external payment providers (Nexi, PayPal, Apple Pay). PlatinumWings implements automated fraud/account verification checks when new payment accounts are linked.
* **Personal Portal (Area Personale)**:
  * *Profile Management*: Basic user information editing and mandatory official ID document uploads.
  * *Flight History*: Logging of past trips and tracking upcoming flights (with a strict policy allowing modifications up to 1 month prior only via customer support).
  * *Digital Wallet & Loyalty Hub*: Manage saved payment cards and track accumulated points/unlocked tier rewards through the PlatinumWings loyalty program.

### 2. Back-Office Management Dashboard (Gestionale Admin)
A unified interface dividing tasks between corporate administrators and customer support agents:
* **Active Flights & Crew Management**: Real-time tracking of active airborne jets, including route tracking, telemetry, and assigned flight crews. Includes a directory of all active pilots, highlighting their shift status (active/idle), ID, and last completed flight.
* **Platform & Marketing Analytics**: Multi-dimensional charts visualizing website traffic trends, mobile app downloads, annual sales revenue metrics, and jet model popularity.
* **Support Ticket Hub**: Tracking customer issues, ticketing timestamps, status (open/resolved), customer accounts, and assigned support agents.
* **Fleet Availability & Database**: A synchronized database table displaying the real-time operational status (active, standby, or hangar) of every private jet in the fleet.
* **Aircraft Maintenance Tracker**: Detailed log of past, in-progress, and scheduled maintenance checks to ensure absolute safety and compliance with civil aviation regulations.
* **Customer Support Portal**: A live chat console enabling customer support agents to respond to incoming 24/7 client inquiries from both the web and mobile applications.

---

## 📊 Feasibility Study: Sourcing & Infrastructure

The theoretical analysis, detailed in [Sigi_Project.pdf](file:///C:/Users/Anton/Desktop/SIGI/Sigi_Project.pdf), evaluates the hardware procurement, licensing, and operating expenses of the two primary hosting options:

### Sourcing Cost Analysis: In-House vs. Outsourced Hosting (Cloud)

#### Option 1: In-House Server Hosting
Purchasing and maintaining physical server infrastructure locally.
* **Capital Expenditures (CapEx) - Initial Hardware**:
  * Fujitsu Primergy RX2530 Medium Server: **~5,000€**
  * 3 QNAP TR-004 NAS (Disaster Recovery) + 12 WD Red Plus 4TB Disks: **1,920€** *(720€ NAS + 1,200€ Disks)*
  * RS PRO 3000VA Uninterruptible Power Supply (UPS): **1,297.43€**
  * Siemens Communications Router (6GK5816-1BA00-2AA2): **1,207.80€**
  * WatchGuard Firewall (Firebox M290): **2,095.98€**
  * 4 Cisco Managed Switches (WS-C2960S-48LPS-L): **412€**
  * Hisense Easy Smart 12000 Server Room Air Conditioner: **390.90€**
  * Annual SSL Encryption Certificate: **$50 - $200 (approx. 150€)**
* **Operational Expenditures (OpEx) - Annual Costs**:
  * Gigabit Internet Service Provider (Vodafone Business): **600€/year**
  * Server Room Electricity Bill: **~800€/year**
  * Technical Staffing & Training: **~8,000€ - 10,000€/year**
  * System Maintenance & Software Updates: **~10,000€ - 15,000€/year**
* **Financial Totals**:
  * **Initial CapEx**: **12,500€ - 18,000€**
  * **Annual OpEx**: **15,000€ - 19,600€**

#### Option 2: Cloud Hosting / Outsourcing (SELECTED STRATEGY)
Leveraging flat-fee/consumption-based VPS hosting from cloud providers (e.g., AWS, Google Cloud).
* **Capital Expenditures (CapEx) - Initial Setup**:
  * Data Migration & System Integration (One-time Software House Fee): **5,000€ - 7,000€**
  * Internal Security Hardware (Siemens Router, WatchGuard Firewall, Cisco Switches, 2 Mediacom 850VA UPS): **~3,700€**
  * *Optional*: 3 QNAP NAS + WD Red Disks (for local backup replication): **1,920€**
* **Operational Expenditures (OpEx) - Annual Costs**:
  * Cloud Hosting Fee (AWS/Google Cloud VPS Flat Package): **3,000€ - 6,500€/year**
  * Gigabit Internet Service Provider (Vodafone Business): **600€/year**
* **Financial Totals**:
  * **Initial CapEx**: **~8,800€** *(including network hardware and one-time migration)*
  * **Annual OpEx**: **5,600€ - 7,000€**

> [!TIP]
> **Outsourcing Sourcing Strategy**: The feasibility study selected Option 2. Outsourcing minimizes upfront Capital Expenditures, bypasses complex IT recruiting, ensures 24/7 provider-backed server recovery (SLA), and scales dynamically with seasonal demand.

---

## 📅 Software Development Timelines & Costs

The development plan splits the application builds into distinct project phases, calculated by software engineering complexity:

| Product | Phase | Complexity Metrics (Simple / Intermed. / Hard) | Days | Development Cost | Annual Maintenance |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Mobile App** | Designing | 10 / 7 / 2 | 14 | 5,600€ | - |
| | Realization | 5 / 10 / 4 | 37 | 11,100€ | - |
| | Verification | 14 / 5 / 2 | 14 | 3,500€ | - |
| *App Total* | | | **65 days** | **20,200€** | **4,040€** |
| **Web Portal** | Designing | 4 / 6 / 15 | 23 | 9,200€ | - |
| | Realization | 10 / 8 / 7 | 47 | 14,100€ | - |
| | Verification | 5 / 10 / 10 | 22.5 | 5,625€ | - |
| *Web Total* | | | **92.5 days** | **28,925€** | **5,785€** |
| **COMBINED** | | | **157.5 days** | **49,125€** | **9,825€** |

---

## 🔍 Market Benchmarking

To optimize the system design, the team analyzed competitors to resolve key industry challenges:
* **Booking Complexity**: Unlike legacy booking portals that require extensive multi-page forms, PlatinumWings implements a simple, progressive stepper checkout with instant email confirmations.
* **Pricing Transparency**: Solves the issue of hidden surcharges in luxury rentals. Standard rates are visible upfront, and dynamic surcharges (worst-case pricing buffer ensuring high margins, verified by accounting) are calculated in real-time.
* **User Navigation**: Implements a sticky, persistent Navbar (benchmarked against luxury brands like VistaJet and budget lines like Ryanair) to ensure easy site exploration.
* **Aesthetic Appeal**: Avoids stock templates by using custom, AI-generated imagery and a clean, luxury dark-mode theme to appeal to high-net-worth clients.

---

## 📚 Systems Theory & Course Integration

The project applies key concepts from the B.Sc. Sistemas Informativi course syllabus:
* **Anthony's Organizational Pyramid**:
  * *Operational level*: Live crew dispatch, pilot shift scheduling, passenger ID verification, and support ticket chat logs.
  * *Tactical level*: Fleet maintenance scheduling, sales analytics dashboard, and marketing performance tracking.
  * *Strategic level*: Cloud hosting sourcing strategy, fleet procurement plans, and systems feasibility studies (S.d.F.).
* **Porter's Value Chain**: How the new digital platform optimizes Operations (automated scheduling), Marketing & Sales (direct-to-consumer app booking), and Service (24/7 AI-assisted support).
* **Disintermediation**: Bypassing traditional retail brokers to offer booking directly to customers, maximizing operational profit margins.
* **Porter-Millar Information Intensity**: Transforming a physical aviation service into an information-rich experience by integrating custom catering, chauffeur scheduling, and partner hotel discounts directly into the booking process.
* **IT Sourcing Frameworks**:
  * *Contract-Out*: Nexi/PayPal/Apple Pay integration for secure payment processing.
  * *Preferred Contractor*: Long-term 24/7 IT helpdesk SLA.
  * *Buy-In*: Temporary software engineers hired for specific specialized integrations.
  * *Preferred Supplier*: Long-term software house contract for future app upgrades.

---

## 📂 Repository Structure

* [README.md](file:///C:/Users/Anton/Desktop/SIGI/README.md) - This document.
* [Sigi_Project.pdf](file:///C:/Users/Anton/Desktop/SIGI/Sigi_Project.pdf) - Detailed systems management feasibility study, including financial costs, risk analysis, and hosting evaluations.
* [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf) - UI/UX user flows, interface wireframes, and dashboard specifications.

---

## 👥 Contributors

* **Marco Rondelli** ([marco.rondelli@studenti.unipr.it](mailto:marco.rondelli@studenti.unipr.it)) – **Author**
* **Matteo Magnoni** – **Contributor**
* **Simone Candiani** – **Contributor**

---

*This project was developed for academic evaluation at the University of Parma.*
