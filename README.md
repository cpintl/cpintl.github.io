# 👋 Mohammad Ariful Islam

**Health Systems Architect** | **Humanitarian Digital Infrastructure** | **Public Health Professional**

> *Designing technology that saves lives in crisis zones — specifically, the Rohingya refugee crisis in Cox's Bazar, Bangladesh.*

---

## 🎯 Mission

I architect **Health Information Systems (HIS)** and **humanitarian supply chain platforms** for the **Community Partners International (CPI) Bangladesh Mission**, serving **970,000+ Rohingya refugees** and vulnerable host communities in Cox's Bazar.

My work bridges clinical excellence, international health standards (FHIR, HL7, ICD-11), and the harsh realities of crisis-zone operations: no internet, no power, no margin for failure.

**Current Focus:** Building **ZarishLog** (supply chain & inventory management) and **ZarishHIS** (health information system) for offline-first, resource-constrained humanitarian operations.

---

## 📊 At a Glance

| Area | Detail |
|------|--------|
| **Current Role** | Health Program Manager, CPI Bangladesh Mission |
| **Location** | Cox's Bazar, Bangladesh (Camp 1W, Camp 4) |
| **Population Served** | 970,000+ Rohingya refugees (world's largest refugee settlement) |
| **Expertise** | FHIR/HL7, HIS design, supply chain systems, crisis informatics |
| **Experience** | 15+ years: clinical practice → systems architect |
| **Technical Stack** | Go, PostgreSQL, FHIR R5, Docker, GitHub, Google Workspace |

---

## 🏥 Focus Areas

### **Primary Projects**

🩺 **ZarishHIS** — Health Information System for Rohingya Refugee Health Programs
- **Scope:** Electronic Medical Records (EMR), patient registry (FCN-based), HCV treatment cascade, CVD/NCD management
- **Architecture:** Offline-first, FHIR R5 compliant, national DHIS2 integration
- **Users:** Health Post staff, Community Health Workers, Medical Officers
- **Status:** V1 Requirements gathering & system design

📦 **ZarishLog** — Supply Chain & Inventory Management System
- **Scope:** Warehouse operations, asset tracking, pharmacy inventory, logistics
- **Architecture:** Real-time synchronization, barcode/RFID support, cold chain tracking
- **Users:** Warehouse staff, logistics coordinators, pharmacy managers
- **Status:** Technical blueprint completed (see attached documentation)

🤝 **CPI Bangladesh Health Programs**
- **HCV Program:** WHO 90-90-90 cascade (testing, diagnosis, treatment, cure verification)
- **CVD/NCD Program:** Hypertension & diabetes screening, treatment, follow-up
- **Health Outreach Program (HOP):** 1,000+ Community Health Workers, doorstep screening
- **Health System Strengthening (HSS):** District hospital partnerships, clinical capacity building

---

## 🛠️ Tech Stack

**Languages:**  
Go · Python · YAML · Markdown · SQL

**Standards & Frameworks:**  
FHIR R5 · HL7 · ICD-11 · SNOMED CT · OpenHIE · DHIS2

**Platforms & Tools:**  
GitHub · Docker · PostgreSQL · Google Workspace · Cloudflare · KoboToolbox · ActivityInfo

**Methodologies:**  
No-code first · Open-source · Offline-first · Zero-trust security · FHIR-first design

---

## 📚 Education & Background

| Qualification | Institution | Year |
|---|---|---|
| **Masters of Public Health (MPH)** | Bangladesh Open University | 2023 |
| **Post Graduation Diploma in Management (PGDM) — HR** | Bangladesh Open University | 2023 |
| **Health Financing & Wealth Inequalities** | Swiss School of Public Health (SSPH+) | 2023 |
| **Project Management in Global Health** | University of Washington | 2022 |
| **Global Mental Health** | University of Washington | 2021 |
| **Bachelor of Public Health Nutrition** | Primeasia University | 2018 |
| **Diploma in Medical Faculty** | State Medical Faculty, Bangladesh | 2013 |

**Key Certifications:**
- International Humanitarian Law (IHL) — Humanitarian Leadership Academy (2021)
- Health Cluster Coordination — WHO (2020)
- Health Facility Design — WHO (2020)
- Building a Better Response — Humanitarian Academy at Harvard (2020)
- Gender Equality in Humanitarian Action — IASC (2020)
- Field Management Course — MSF (2018)
- Mass Casualty Management — MSF (2018)
- BLS with CPR Certification — First Aid Centre of Sweden (2020)

---

## 💼 Professional Experience

**15+ years in humanitarian health leadership:**

- **Strategic Planning & Program Management** — End-to-end cycle management from needs assessment to M&E in 8+ countries
- **Data-Driven Decision Making** — Epidemiological analysis for rapid response and resource allocation
- **Crisis Management & Security** — Operating in high-risk environments; managing security operations protocols
- **System Design & Architecture** — HIS architecture, database design, interoperability frameworks, FHIR implementation
- **Team Leadership** — Multidisciplinary teams (medical, technical, field) in resource-constrained environments
- **Partnership Management** — Government liaison, NGO coordination, donor compliance, MOU development
- **Clinical Practice** — Frontline care delivery; medical education; emergency response

---

## 🌍 Working Context: Cox's Bazar Refugee Settlement

### **The Crisis**
- **Population:** 970,000+ Rohingya refugees across 33–34 camps
- **Displaced:** Mass displacement from Myanmar beginning August 2017
- **Density:** 47,000 people/km² — world's highest population density in a humanitarian setting
- **Scale:** Kutupalong camp system (~23 camps) = world's largest refugee camp
- **Accessibility:** 60% of Cox's Bazar district becomes inaccessible during monsoon season

### **Key Challenges**
- ⚠️ **Connectivity:** Intermittent mobile broadband; many areas without coverage
- ⚠️ **Infrastructure:** Limited power, limited devices, limited storage capacity
- ⚠️ **Language:** Rohingya, Bangla, English language coordination complexity
- ⚠️ **Security:** Armed group activity, frequent access restrictions, staff safety concerns
- ⚠️ **Governance:** UNHCR-led coordination; government liaison (RRRC, DGHS); inter-NGO coordination

### **CPI Bangladesh Response**
Operating since 2017 across two primary camps (Camp 1W, Camp 4) with:
- 1 main health post (200+ daily OPD visits)
- 1,000+ community health workers
- HCV treatment program (700+ patients in care)
- CVD/NCD screening & management
- 250-bed district hospital partnership (Emergency Department support)
- WASH infrastructure (water systems, sanitation)
- Education & livelihoods programs

---

## 🏗️ Current Architecture: CPI Bangladesh HIS

### **Design Philosophy**
> *"The distance between high-level policy (WHO guidelines) and working tools available to health workers is a structural failure that causes real-world harm. Humanitarian digital infrastructure should be not just software—it should be foundational technology for civilization."*

### **Core Principles**
1. **Offline-First** — System works without internet; syncs when connected
2. **FHIR-First** — All data models built on FHIR R5 for interoperability
3. **No Vendor Lock-in** — Data exportable in open standards; open-source codebase
4. **Zero-Cost** — No trial periods, no freemium paywalls; always free tiers
5. **Patient-Centered** — UNHCR Family Card Number (FCN) as universal patient ID
6. **Scalable** — From single health post to national health system

### **System Components**

**Tier 1 — Community (CHWs)**
- Mobile app: household visit logs, RDT screening, referrals
- Offline-first: captures data even without connectivity
- Syncs via WhatsApp/SMS backup if internet unavailable

**Tier 2 — Health Post (Clinic)**
- EMR: patient registration, OPD encounters, clinical notes
- HCV module: screening, diagnosis, treatment enrollment, SVR tracking
- NCD module: BP/glucose screening, medication refills, follow-up visits
- Lab integration: sample tracking, result recording

**Tier 3 — Program Management**
- Patient line lists, referral tracking, performance dashboards
- M&E indicators (HCV 90-90-90, NCD control rates, CHW productivity)
- Donor reporting (UNHCR, ECHO, USAID)

**Tier 4 — National Integration**
- DHIS2 auto-push: monthly aggregate health statistics
- HeRAMS: facility assessment & resource tracking
- EWARS: early warning & disease surveillance (weekly reports)
- 4W mapping: partner activity coordination

---

## 📋 Documentation & Resources

### **Repositories**
- **[zarishlog](https://github.com/cpintl/zarishlog)** — Supply chain & inventory management system
- **[zarishhis](https://github.com/cpintl/zarishhis)** — Health information system (FHIR-based)
- **[cpintl-standards](https://github.com/cpintl/cpintl-standards)** — Health standards & interoperability documentation
- **[cpintl.github.io](https://github.com/cpintl/cpintl.github.io)** — This profile & organizational hub

### **Key Documents**
- 📄 **[ZarishLog Technical Blueprint](./docs/zarishlog-technical-blueprint.md)** — Complete supply chain system design
- 📋 **[HIS Requirements Checklist v1.0](./docs/his-requirements-checklist.md)** — 390-item requirements for ZarishHIS
- 🏥 **[CPI Bangladesh Mission Profile](./docs/cpi-bangladesh-profile.md)** — Organizational context & governance
- 🔄 **[FHIR Implementation Guide](./docs/fhir-implementation-guide.md)** — Standard-based data modeling

---

## 📊 GitHub Activity

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=cpintl&show_icons=true&theme=github_dark&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=cpintl&layout=compact&theme=github_dark&hide_border=true)

---

## 🤝 CPI Bangladesh Partners & Stakeholders

| Entity | Role | Contact |
|--------|------|----------|
| **Young Power in Social Action (YPSA)** | Prime implementing partner | https://ypsa.org |
| **Community Partners International (CPI)** | Lead organization | https://cpintl.org |
| **WHO / Health Sector (Cox's Bazar)** | Coordination & oversight | WHO Health Sector Coordinator |
| **UNHCR Bangladesh** | Refugee registration, FCN issuance | UNHCR Cox's Bazar |
| **Ministry of Health (Bangladesh)** | Government liaison | DGHS, Cox's Bazar Civil Surgeon |
| **District Sadar Hospital (DSH)** | Clinical partner | HSS program (Emergency Department) |
| **Friendship (NGO)** | Health program partner | Camp 5 sentinel screening |
| **icddr,b** | Research partner | CVD-HCV cluster randomized trial |

---

## 💡 Philosophy

My approach to humanitarian technology:

1. **User-Centered** — Design from field realities, not assumptions
2. **Open-Source** — Transparency, reproducibility, community ownership
3. **Offline-First** — Assuming connectivity is rare, not default
4. **Standards-Based** — FHIR/HL7 for interoperability and future portability
5. **Scalable** — From single health post to national health system
6. **Sustainable** — Zero-cost, maintainable by local teams without external dependency

---

## 🎯 What I'm Looking For

- 🤝 **Collaborators** — FHIR/HL7 specialists, humanitarian tech developers, Go engineers
- 💡 **Feedback** — On ZarishLog & ZarishHIS architecture, system design decisions
- 🌐 **Community** — Humanitarian tech practitioners, crisis informatics professionals, NGO tech leads
- 📚 **Learning** — Advanced Go, distributed systems, blockchain for supply chain transparency
- 🏥 **Partners** — NGOs, health systems, academic institutions working in crisis zones

---

## 🔗 Connect With Me

| Platform | Link | Purpose |
|----------|------|----------|
| **Email (Work)** | [ariful@cpi-ypsa.org](mailto:ariful@cpi-ypsa.org) | CPI Bangladesh program matters |
| **Email (Alt)** | [bgd.cpms@cpintl.org](mailto:bgd.cpms@cpintl.org) | Project management system |
| **LinkedIn** | [arifulislambgd](https://www.linkedin.com/in/arifulislambgd) | Professional profile |
| **GitHub** | [@cpintl](https://github.com/cpintl) | Code & documentation |
| **Phone** | +880 1723 889843 | Field coordination |
| **CPI Bangladesh** | [cpintl.org](https://cpintl.org) | Organization website |

---

## 📞 Support & Questions

- 🐛 **Report a bug:** [Open an issue](https://github.com/cpintl/cpintl.github.io/issues/new)
- 💬 **Ask a question:** [GitHub Discussions](https://github.com/cpintl/cpintl.github.io/discussions/new)
- 📧 **Email:** [ariful@cpi-ypsa.org](mailto:ariful@cpi-ypsa.org)
- 🔗 **LinkedIn:** [Connect here](https://linkedin.com/in/arifulislambgd)

---

## 🙏 Acknowledgments

- **Community Partners International (CPI)** — For humanitarian mission and technical freedom
- **Young Power in Social Action (YPSA)** — For field partnership and implementation expertise
- **WHO, UNHCR, Health Sector partners** — For coordination and guidance
- **Open-source community** — For enabling tools, standards, and collaborative ethos
- **Rohingya refugee community** — For trust and feedback that drives system design

---

**Built with ❤️ for humanitarian impact**  
*Open-source · Vendor-free · Standards-first · Offline-ready*

**Last Updated:** 2026-07-15  
**License:** [MIT License](./LICENSE)