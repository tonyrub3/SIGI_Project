# PlatinumWings – Luxury Private Jet Booking & Admin Management System

[![Figma Design Workspace](https://img.shields.io/badge/Figma-Design_Workspace-F24E1E?logo=figma&logoColor=white)](https://www.figma.com/design/NN3OKzkvAveVYPv5JvkVvs/Login?node-id=0-1&p=f&t=pV9AmxhKATXMimds-0)
[![University](https://img.shields.io/badge/University-UNIPR-003C71?logo=university&logoColor=white)](https://www.unipr.it)
[![Obsidian](https://img.shields.io/badge/Obsidian-Notes-7C4DFF?logo=obsidian&logoColor=white)](https://obsidian.md)

This repository contains the system architecture, UI/UX wireframes, and complete feasibility documentation for **PlatinumWings**, a premium private jet booking platform. 

Created as a final project for the **Sistemi Informativi e Gestione d'Impresa (SIGI)** (Information Systems and Business Management) course at the **University of Parma**, this project demonstrates how to take a legacy, manual business operation and re-engineer it into a modern, cloud-backed digital ecosystem.

---

## 💼 Professional Value & Skills Demonstrated

This project is a comprehensive showcase of end-to-end systems analysis, interactive product design, financial modeling, and IT governance—essential skills for roles such as **Product Designer (UI/UX)**, **Systems Analyst**, or **IT Project Manager**.

Through this project, the team acquired and demonstrated the following core professional competencies:

### 1. High-Fidelity UI/UX & Interaction Design (Figma)
* **Design Systems & Aesthetics**: Developed a premium, high-contrast dark mode design system matching luxury brand guidelines. Used clean layouts, structured typography, and AI-generated premium imagery to match the expectations of high-net-worth clients.
* **Component-Driven Design**: Built reusable components and interface variants in Figma, mapping complete user journeys from booking to payment and support.
* **Usability Benchmarking**: Researched and benchmarked competitive layouts, implementing a sticky, persistent navigation system (comparing low-cost Ryanair layouts and luxury VistaJet navigation models) to improve site discoverability.
* **Responsive Layouts**: Designed mobile-friendly web flows and synchronized mobile application screens to ensure seamless cross-device interactions.

### 2. Business Process Re-engineering (BPR)
* **Legacy Decoupling**: Analyzed an outdated, phone-based manual booking model and successfully decoupled its workflows into automated customer-facing app steps and administrative ERP tools.
* **API Integration & Partnership Mapping**: Modeled automated exchanges with third-party vendors (Nexi/PayPal for payment gateways, external partner platforms for private chauffeur booking, and luxury hotel portals offering customer discounts).

### 3. Financial Modeling & Feasibility Analysis
* **CapEx & OpEx Modeling**: Formulated detailed financial estimates comparing on-premises server hosting (high CapEx of 12.5k€–18k€ and OpEx of 15k€–19.6k€/year) against Cloud Hosting / Outsourcing (optimized CapEx of ~8.8k€ and OpEx of 5.6k€–7k€/year).
* **Software Development Budgeting**: Managed project scope by creating software sprint estimations (App development cost: €20,200 over 65 days; Web portal development: €28,925 over 92.5 days), predicting a total initial budget of **€49,125**.
* **Risk Management**: Conducted qualitative risk assessments for security vulnerabilities (ransomware mitigation via RAID/NAS backups), internet dependency, and organizational change barriers.

### 4. IT Governance & Sourcing Strategy
* **Sourcing Optimization**: Analyzed when to utilize *Outsourcing* (cloud scaling) vs. *Insourcing* based on local resource limits.
* **Service Level Agreements (SLAs) & Sourcing Contracts**: Applied sourcing frameworks (Contract-Out, Preferred Contractor, Buy-In, Preferred Supplier) to handle external vendor relations.
* **Security & Compliance Systems**: Designed administrative controls based on the **Least Privilege Principle** (role-based admin/support access levels) and E2E encryption standards (SSL certificates).

---

## 📄 Feasibility Study: Executive Summary

The complete feasibility study, detailed in [Sigi_Project.pdf](file:///C:/Users/Anton/Desktop/SIGI/Sigi_Project.pdf), evaluates the business model transformation of PlatinumWings:

### 1. Legacy Bottlenecks
PlatinumWings (founded in 2014 in Parma) initially grew via manual operations. As sales volumes increased, this process caused five critical issues:
* Manual phone coordination took excessive time, resulting in high customer drop-off.
* 24/7 phone operators experienced severe bottlenecks during peak holiday seasons.
* Legacy internal software had an outdated UI, leading to long onboarding cycles for new hires.
* Excessive cross-departmental hand-offs (operators, accounting, managers, suppliers) caused delivery delays.
* Customers lacked transparency, as they could not view real-time fleet schedules or choose custom extras.

### 2. The Cloud Hosting Sourcing Decision
The feasibility study evaluated whether to host the new system on local server hardware or in the cloud. **Cloud Hosting (Outsourcing)** was selected as the optimal path:
* **Lower Initial Cost**: €8.8k CapEx (cloud) vs. €12.5k–18k CapEx (in-house).
* **Lower Recurring Overhead**: €5.6k–7k OpEx (cloud) vs. €15k–19.6k OpEx (in-house).
* **SLA Reliability**: Outsources complex network troubleshooting, electrical costs (~800€/year), and database administration to cloud experts, allowing PlatinumWings to focus on its core luxury travel business.

---

## 🗺️ Key Features & Flows mapped in Figma

The interactive workspace, linked in [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf), implements two main portals:

### 1. Traveler Booking Application (Web & App)
* **Stepper Checkout**: One-way, round-trip, or multi-city booking with passenger data collection (ID/Passport uploads required for safety compliance).
* **Luxury Add-ons**: Driver services, gourmet catering experiences (Italian, Mexican, Japanese menus), and luxury hotel discounts.
* **Smart Cost Optimizer**: Suggests cheaper travel dates to help users save money.
* **Personal Area**: Secure digital wallet, flight history trackers (flights modifiable up to 1 month prior only), and loyalty card trackers.

### 2. Admin ERP Dashboard (Gestionale Admin)
* **Logistics & Dispatch**: Real-time flight tracking, pilot shift status, and fleet availability tables (Active, Standby, Hangar).
* **Maintenance Scheduler**: Logging past and upcoming aircraft maintenance events to ensure passenger safety.
* **Analytics Panel**: Multi-dimensional charts showing site traffic trends, app downloads, and sales revenue.
* **Support Ticket Hub**: Customer ticket assignment logs and a live chat console for 24/7 customer support operators.

---

## 📂 Repository Structure

* [README.md](file:///C:/Users/Anton/Desktop/SIGI/README.md) - This document.
* [Sigi_Project.pdf](file:///C:/Users/Anton/Desktop/SIGI/Sigi_Project.pdf) - The 42-page Feasibility Study, covering costs, infrastructure, risk modeling, and business canvas.
* [Wireframe.pdf](file:///C:/Users/Anton/Desktop/SIGI/Wireframe.pdf) - Comprehensive walkthrough of the Figma user flows, layout wireframes, and UI workflows.

---

## 👥 The Team

* **Antonio Rubino** ([tonyrub3](https://github.com/tonyrub3)) – **Author & Creator**
* **Fabio Germano** – **Contributor**
* **Paolo Senna** – **Contributor**
* **Geri Atija** – **Contributor**

---

*This project was developed for academic evaluation at the University of Parma.*
