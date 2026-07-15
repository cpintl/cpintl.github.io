# ZarishHIS Requirements Overview

For the complete 390-item requirements checklist, see [HIS Requirements Checklist v1.0](../his-requirements-checklist.md).

## What is ZarishHIS?

**ZarishHIS** is a national-grade **Health Information System (HIS)** designed for CPI Bangladesh's health programs, serving 970,000+ Rohingya refugees in Cox's Bazar.

## Core Components

### 1. Patient Registry
- **Patient ID:** UNHCR Family Card Number (FCN) as universal identifier
- **Demographics:** Name (Rohingya), age/DOB, sex, location (camp/block/sub-block)
- **Vulnerability Flags:** Pregnant, elderly (60+), disability, unaccompanied minor
- **Population Integration:** Linked to UNHCR March 2026 block-level population data

### 2. Electronic Medical Record (EMR)
- **OPD Encounters:** Chief complaint, vital signs (BP, pulse, temp, weight, height, SpO2)
- **Clinical Notes:** Diagnosis (ICD-11 coded), examination findings, clinical assessment
- **Prescriptions:** Treatment/medication linked to facility drug formulary
- **Lab Orders & Results:** Sample tracking, result recording, lab integration
- **Referrals:** Referral generation, follow-up tracking, outcome recording
- **Visit History:** Longitudinal patient record with past encounter visibility

### 3. HCV Treatment Cascade (WHO 90-90-90)
- **Screening Encounter:** HCV RDT testing, results recording
- **Diagnosis:** HCV RNA PCR confirmation, genotyping (if available)
- **Treatment Initiation:** DAA regimen selection, baseline labs (fibrosis assessment)
- **Monthly Follow-up:** Visits 1–12, adverse event tracking, medication adherence
- **SVR Assessment:** Cure confirmation (SVR12 or SVR24)
- **Lost-to-Follow-Up Alerts:** Automated flagging of missed visits

### 4. CVD/NCD Management
- **Screening Form:** WHO PEN risk assessment, BP/glucose measurement
- **Enrollment:** Risk stratification, treatment initiation, medication selection
- **Quarterly Follow-Up:** BP/glucose rechecks, medication refills, complication assessment
- **Patient Tracking:** Self-management adherence (diet, exercise, smoking status)
- **Outcome Recording:** Stroke, MI, amputation, blindness, death

### 5. Community Health Worker (CHW) Tools
- **Mobile App (offline-first):** Household visit logs, RDT screening, referral initiation
- **FCN Lookup:** Patient search by UNHCR family card number
- **GPS Geotagging:** Location-based visit tracking
- **Photo Capture:** Wound photos, MUAC documentation
- **Supervisor Review:** Approval workflow before data finalization
- **Performance Metrics:** Visit completion, referral rates, adherence rates

### 6. Laboratory & Diagnostics
- **Point-of-Care Tests:** RDT (HCV, malaria), blood glucose, urine dipstick
- **External Lab Integration:** Sample dispatch tracking, result receipt, critical value alerts
- **Barcode/RFID Labeling:** Sample identification and tracking
- **Result Turnaround:** Automated notifications when results available

### 7. Pharmacy & Supply Chain
- **Dispensing Linked to EMR:** Each dispensing event recorded against patient encounter
- **Stock Management:** Current inventory levels, minimum thresholds, reorder points
- **Expiry Tracking:** Automated alerts for near-expiry medicines
- **Consumption Reporting:** Monthly drug consumption trends
- **HCV DAA Tracking:** Antiretroviral inventory management
- **Stock-Out Alerts:** Triggered when stock falls below threshold

### 8. Disease Surveillance (EWARS)
- **Auto-Generated EWARS Report:** System compiles weekly disease surveillance from OPD data
- **Outbreak Alerts:** Triggered when case count exceeds threshold
- **Contact Tracing:** For communicable diseases requiring follow-up
- **WHO EWARS Portal Integration:** Direct data push to WHO surveillance system

### 9. Reporting & M&E
- **HCV Cascade Dashboard:** 90-90-90 visualization, cascade bottleneck identification
- **NCD Control Metrics:** % BP controlled, % diabetes controlled, treatment adherence
- **CHW Performance:** Household visits, referrals, screening completion
- **Donor Reports:** UNHCR, ECHO, USAID indicator dashboards
- **DHIS2 Auto-Push:** Monthly aggregate data submission to national health system
- **HeRAMS Facility Assessment:** Resource & capacity tracking
- **4W Activity Reporting:** Sector coordination (ISCG platform)

### 10. Data Integration & Interoperability
- **Inbound:** UNHCR population data, lab results, CHW forms
- **Outbound:** DHIS2, HeRAMS, EWARS, ActivityInfo, donor portals
- **FHIR Compliance:** All data models follow FHIR R5 standard
- **API Layer:** Third-party system integration capability

---

## Offline-First Architecture

**Key Challenge:** Intermittent internet in Cox's Bazar; 60% of district inaccessible during monsoon  
**Solution:**
- Local encounter store on tablets/phones
- Automatic sync when connectivity available
- Conflict resolution for offline edits
- Optional mini-server (local deployment) at health post

---

## User Roles & Access Control

| Role | System Access | Primary Tasks |
|------|---|---|
| **System Administrator** | Full system access | Backups, security, user management |
| **Medical Officer** | Own patient caseload + all clinical records | Patient visits, prescriptions, referrals |
| **Nurse / Paramedic** | Patient registration, vital signs, dispensing | Triage, vital capture, medication dispensing |
| **CHW / Field Worker** | Mobile app only (limited fields) | Household visits, screening, referrals |
| **M&E Officer** | Read-only dashboard access | Indicator tracking, donor reports |
| **Pharmacy** | Pharmacy module only | Stock management, dispensing logs |
| **Lab Assistant** | Lab module only | Sample receipt, result entry |

---

## Data Governance & Compliance

### Security
- **Informed Consent:** Written, translated to Rohingya
- **Data Ownership:** Clear policy (CPI? YPSA? UNHCR? GoB?)
- **Access Logging:** Audit trail of who viewed/edited each record
- **Encryption:** Data in transit (HTTPS) and at rest
- **Anonymization:** De-identified data for research

### Legal
- **Bangladesh Digital Security Act 2018** compliance
- **UNHCR Data Protection Standards** for refugee data
- **GoB / RRRC Access Requirements:** Clarify government access needs
- **Data Destruction Policy:** Retention period and permanent deletion procedures

---

## Implementation Status

✅ **Requirements gathering:** 77/390 items confirmed (20% complete)  
⚠️ **Partial clarity:** 9/390 items (2% — pending stakeholder input)  
⬜ **Still needed:** 304/390 items (78% — awaiting decisions)  

**Next Steps:**
1. Complete stakeholder consultation (Sections 2, 4, 6–8, 15, 18–25)
2. Finalize system vision & phasing strategy
3. Confirm budget & development timeline
4. Begin Tier 1 prototype (CHW mobile app)

---

## For More Information

See the full [HIS Requirements Checklist v1.0](../his-requirements-checklist.md) document for:
- Complete 390-item requirements matrix
- Stakeholder input needed per section
- System design decisions pending
- Phasing strategy options

**Contact:** Mohammad Ariful Islam | ariful@cpi-ypsa.org