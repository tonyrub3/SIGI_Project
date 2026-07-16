# PlatinumWings – Luxury Private Jet Booking Platform & Business System Design

[![Figma Prototype](https://img.shields.io/badge/Figma-Prototype-F24E1E?logo=figma&logoColor=white)](https://www.figma.com/proto/NN3OKzkvAveVYPv5JvkVvs/Login?node-id=890-1107&t=JUG2TDHjGOo7JwKj-1&starting-point-node-id=743%3A974&show-proto-sidebar=1)
[![University](https://img.shields.io/badge/University-UNIPR-003C71?logo=university&logoColor=white)](https://www.unipr.it)
[![Obsidian](https://img.shields.io/badge/Obsidian-Notes-7C4DFF?logo=obsidian&logoColor=white)](https://obsidian.md)

This repository contains the system design, theoretical documentation, user experience wireframes, and interactive prototype link for **PlatinumWings**, a high-end private jet booking platform. 

The project was developed as a B.Sc. final project for the **Sistemi Informativi e Gestione d'Impresa (SIGI)** (Information Systems and Business Management) course at the **University of Parma**. It combines rigorous IT governance and corporate management theory with practical UI/UX design and database-backed workflow logic.

---

## ✈️ Project Overview: PlatinumWings

**PlatinumWings** is a luxury private jet rental service that integrates a traveler booking app with a comprehensive back-office management dashboard (Enterprise Resource Planning / CRM) for administrators, dispatchers, pilots, and customer support representatives.

The project structure is broken down into two main components:
1. **Interactive Figma Prototype**: A high-fidelity UI/UX prototype mapping out the entire passenger booking journey and the admin management console.
2. **System & Business Analysis**: A theoretical analysis of the enterprise system's lifecycle, sourcing strategies, organizational impacts, and alignment with course principles.

---

## 🗺️ System Architecture & User Flows

The interactive interface is detailed in [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf). It is split into two primary operational areas:

### 1. Customer-Facing Web & Mobile Application
Designed for high-net-worth individuals, providing a seamless, end-to-end luxury travel booking process:
* **Dynamic Booking Engine**: Users can search and book one-way, round-trip, or multi-city private flights by selecting dates, times, and traveler counts.
* **Smart Fleet Selection**: A comprehensive gallery and specifications for the three distinct private jet categories in the catalog.
* **Real-Time Dynamic Pricing**: Cost estimations calculate pricing based on seasonal demand density (e.g., peak holidays like New Year's Eve), jet class, and operational relocation costs.
* **Bespoke Luxury Customizations (Add-ons)**:
  * *Private Chauffeur Service*: Bookable for specific days or the entire duration of the trip (with complimentary basic airport transfers included by default).
  * *On-board Dining Experience*: Selection of curated Italian, Mexican, or Japanese menus for the outbound and return journeys.
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

## 📚 Systems Theory & Course Integration

The theoretical analysis, detailed in [SIGI.pdf](file:///C:/Users/Anton/Desktop/SIGI/SIGI.pdf), bridges the software implementation with modern corporate Information Systems (IS) principles:

```
                  ▲
                 / \
                /   \      Strategic Level (C-Level, Planning, S.d.F., Budgeting)
               /     \
              /       \
             /─────────\
            /           \    Tactical Level (Middle Mgmt, Fleet Maintenance, Analytics)
           /             \
          /───────────────\
         /                 \ Operational Level (Live Crew Scheduling, Ticket Resolution)
        /                   \
       /─────────────────────\
```

### 1. Anthony's Organizational Pyramid
The system aligns operations across three management tiers:
* **Operational Level**: Executed by ticketing agents, pilots, and support operators using real-time flight dashboards, checking jet availability, resolving support chats, and checking traveler IDs.
* **Tactical Level**: Handled by department managers monitoring annual sales reports, planning scheduled jet maintenance windows, analyzing model popularity, and managing crew shift rotations.
* **Strategic Level**: Managed by the executive suite making long-term fleet procurement decisions, evaluating outsourcing/sourcing strategies, and initiating Feasibility Studies (S.d.F.) for system upgrades.

### 2. Value Chain & Disintermediation (Porter's Model)
* **Value Chain Optimization**: ICT integration reduces friction across inbound logistics (maintenance supplies), operations (flight booking & dispatch), outbound logistics (passenger transport), and service (24/7 support chat).
* **Disintermediation**: Leveraging direct-to-consumer digital channels (direct figma prototype app/web) bypasses traditional travel agencies and distribution intermediaries, lowering operational costs and maximizing profit margins.

### 3. Information Intensity (Porter-Millar Grid)
Under the Porter-Millar framework, private aviation is classified as a service with high information intensity. PlatinumWings shifts into the premium quadrant by adding information to the physical product—enriching the core transport service with customizable digital experiences (catering, chauffeur logs, verified payment profiles, and partner hotel discounts).

### 4. Sourcing & IT Governance Strategy
The system outlines a clear IT governance roadmap for software acquisition and staffing:
* **Sourcing Spectrum**: Details the trade-offs of *Outsourcing* (lowering fixed costs but risking provider lock-in/knowledge loss) versus *Insourcing*.
* **Contractual Frameworks**: Employs *Contract-out* for standardized external integrations (e.g., Nexi/PayPal payment gateway), *Preferred Contractor* relations for long-term support infrastructure, *Buy-in* contracts to temporarily fill resource gaps on specialized modules, and *Preferred Supplier* structures for long-term developer collaborations.

### 5. Feasibility Study (Studio di Fattibilità - S.d.F.)
Any updates to the system follow a structured lifecycle:
1. **Objectives & Functional Specifications**: Aligning operational requirements with budget and timeline constraints.
2. **System Design & Organizational Impact Analysis**: Designing server architectures, evaluating scalability, reliability, and security while ensuring minimal friction for employees transitioning to the new systems.
3. **Economic Valuation**: Conducting cost-benefit analysis (comparing one-time acquisition costs vs. recurring maintenance/licensing fees, e.g. SaaS vs. Enterprise server licenses).
4. **Implementation Decision**: Generating the final project specification to guide technical developers, project leaders, and end-user onboarding.

---

## 🛠️ Repository Contents

* [README.md](file:///C:/Users/Anton/Desktop/SIGI/README.md) - This document.
* [SIGI.pdf](file:///C:/Users/Anton/Desktop/SIGI/SIGI.pdf) - Detailed systems management, outsourcing, IT governance, and feasibility study lecture notes (Exported from Obsidian.md).
* [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf) - Full UI/UX description of the booking application and admin dashboard flows.

---

## 👥 Contributors

* **Marco Rondelli** ([marco.rondelli@studenti.unipr.it](mailto:marco.rondelli@studenti.unipr.it)) – **Author**
* **Matteo Magnoni** – **Contributor**
* **Simone Candiani** – **Contributor**

---

*This project was developed for academic evaluation at the University of Parma.*
