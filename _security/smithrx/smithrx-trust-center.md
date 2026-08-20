---
certifications:
- SOC 2
- HIPAA
description: 'Verbatim page description: "As a radically transparent PBM, our mission is to reduce cost and complexity for employers and their members. We take the security of your data seriously—applying rigorous compliance standards and best-in-class safeguards to protect sensitive information at every step. Learn more about our commitment to privacy, compliance, and operational integrity."'
kind: trust-center
layout: security
name: Smithrx Trust Center
name_suffix: Trust Center
overview: SmithRx maintains a public trust center documenting SOC 2 and HIPAA compliance.
provider_name: SmithRx
provider_slug: smithrx
slug: smithrx-trust-center
source_filename: smithrx-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nurl: https://trust.smithrx.com/\nname: SmithRx Trust Center\nplatform: Vanta\nplatform_evidence: trust.smithrx.com is a CNAME to 63375548372ed4d85b680637.cname.vantatrust.com;\n  the page is served by Vanta's trust-report application (assets.vanta.com/static/index-trust-report.*)\ndescription: 'Verbatim page description: \"As a radically transparent PBM, our mission\n  is to reduce cost and complexity for employers and their members. We take the security\n  of your data seriously—applying rigorous compliance standards and best-in-class safeguards\n  to protect sensitive information at every step. Learn more about our commitment to\n  privacy, compliance, and operational integrity.\"'\ncontent_machine_readable: false\ncontent_note: The trust center is a client-side rendered single-page app backed by\n  an authenticated Vanta API (api.vanta.com returns 401 Unauthorized anonymously).\n  The certification list, audit reports\
  \ and subprocessors are therefore NOT harvestable\n  without JavaScript execution or a document request. Presence is verified; the\n  specific framework list served by this page is not recorded here rather than guessed.\nsecondary_page:\n  url: https://smithrx.com/security\n  name: SmithRx Security Protocols\ncertifications:\n- name: SOC 2\n  claim: 'SOC2 Hosting — \"Ensures compliance with industry standards\"'\n  scope: hosting\n  evidence: https://smithrx.com/security\n  attestation_available: request-via-trust-center\n  note: Stated on the public security page as a property of hosting, not as a named\n    SmithRx Type I/II report; no auditor is named on the public surface.\n- name: HIPAA\n  claim: 'Privacy policy states collection and use of personal information \"will be\n    subject to the requirements of the Health Insurance Portability and Accountability\n    Act (\\\"HIPAA\\\")\" and that identifiable member health data is protected health\n    information (PHI).'\n  evidence:\
  \ https://smithrx.com/privacy-policy\n  evidence_date: '2026-07-10'\naccreditations:\n- name: URAC Pharmacy Benefit Management\n  body: URAC\n  accreditation_id: PBM010015\n  url: https://accreditnet.urac.org/directory/#/accreditation/PBM010015/info\n  expires: '2029-02-01'\n  evidence: https://smithrx.com/security\ncontrols_published:\n- control: AES-256 encryption for data at rest and in transit\n- control: Role-Based Access Control (RBAC), least privilege\n- control: Multi-Factor Authentication (MFA)\n- control: Single Sign-On (SSO)\n- control: Endpoint security with central management\n- control: Full disk encryption with remote wipe\n- control: Audit logging and anomaly detection\n- control: Security Awareness Training required before access is granted\nnot_evidenced_on_public_surface:\n- ISO 27001\n- ISO 27017\n- ISO 27018\n- HITRUST\n- PCI DSS\n- FedRAMP\n- CSA STAR\n- penetration test summary\n- subprocessor list\nevidence:\n- source: https://trust.smithrx.com/\n  http_status:\
  \ 200\n  fetched: '2026-08-02'\n  matched:\n  - SmithRx Trust Center\n  - rigorous compliance standards\n  - commitment to privacy, compliance, and operational integrity\n- source: https://smithrx.com/security\n  http_status: 200\n  fetched: '2026-08-02'\n  keywords:\n  - soc2\n  - encryption\n  - rbac\n  - mfa\n  - audit logging\n  - security vulnerability\n- source: https://smithrx.com/privacy-policy\n  http_status: 200\n  fetched: '2026-08-02'\n  keywords:\n  - HIPAA\n  - protected health information\n  last_updated: '2026-07-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithrx/refs/heads/main/security/smithrx-trust-center.yml
summary_line: SOC 2, HIPAA
tags:
- Company
- Healthcare
- Pharmacy
- Pharmacy Benefit Management
- Prescription Drugs
- Employee Benefits
- Claims
- Insurance
- Health Technology
trust_url: https://trust.smithrx.com/
---
