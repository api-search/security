---
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2022
- ISO/IEC 27001:2013
- PCI DSS 4.0.1
- HIPAA
- GDPR
- CCPA
- PIPEDA
- DORA (EU Digital Operational Resilience Act)
- CIS Controls v8.1
- Shared Assessments SIG
description: eSentire runs a published UpGuard trust page at trust.esentire.com. The page itself renders client-side and returns an HTML shell to any non-browser fetch, but the data behind it is served as public JSON at https://trust.esentire.com/api/trustpage/public/v1/ with no credentials, and that document is the source for everything recorded below. It is the richest machine-readable artifact eSentire publishes — considerably richer than anything on its own developer surface.
kind: trust-center
layout: security
name: Esentire Trust Center
name_suffix: Trust Center
overview: eSentire maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2022, ISO/IEC 27001:2013, PCI DSS 4.0.1, HIPAA, GDPR, CCPA, PIPEDA, DORA (EU Digital Operational Resilience Act), CIS Controls v8.1, and Shared Assessments SIG compliance.
provider_name: eSentire
provider_slug: esentire
slug: esentire-trust-center
source_filename: esentire-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://trust.esentire.com/api/trustpage/public/v1/\nname: eSentire Trust Center\nurl: https://trust.esentire.com/\nplatform: UpGuard Trust Page\ndescription: >-\n  eSentire runs a published UpGuard trust page at trust.esentire.com. The page\n  itself renders client-side and returns an HTML shell to any non-browser fetch,\n  but the data behind it is served as public JSON at\n  https://trust.esentire.com/api/trustpage/public/v1/ with no credentials, and\n  that document is the source for everything recorded below. It is the richest\n  machine-readable artifact eSentire publishes — considerably richer than anything\n  on its own developer surface.\ncontact:\n  name: Office of the CISO\n  role: Governance Risk and Compliance Team\n  email: security@esentire.com\ncertifications:\n- id: SOC_2_Type_II\n  name: SOC 2 Type II\n  scope: Managed Detection and Response Services; Digital Forensics & Incident Response Services (separate\
  \ reports)\n  period: '2024-12-01 to 2025-11-30'\n  evidence: System and Organization Controls Report SOC 2 Type 2 — MDR Services; and — Digital Forensics Incident Response Services\n  bridge_letter: SOC2 Bridge Letter - February 2026\n  updated: '2026-02-27'\n- id: ISO_27001\n  name: ISO/IEC 27001:2022\n  certificate: IS735163\n  expires: '2027-04-07'\n  evidence: ISO 27001:2022 Certificate of Registration; ISO Statement of Applicability\n  updated: '2026-03-06'\n- id: ISO_27001_2013\n  name: ISO/IEC 27001:2013\n  note: Superseded badge retained alongside the 2022 certification.\n- id: PCI_DSS\n  name: PCI DSS 4.0.1\n  evidence: PCI DSS 4.0 Attestation of Compliance; eSentire PCI DSS Shared Responsibility Matrix\n  scope: eSentire XDR Services\n  updated: '2025-12-05'\n- id: HIPAA\n  name: HIPAA\n- id: GDPR\n  name: GDPR\n- id: CCPA\n  name: CCPA\n- id: PIPEDA\n  name: PIPEDA\n  note: Canadian federal privacy law; eSentire is headquartered in Waterloo, Ontario.\n- id: DORA\n  name: DORA\
  \ (EU Digital Operational Resilience Act)\n  evidence: eSentire Services Locations and Subcontracting (DORA) — also published at https://www.esentire.com/legal/compliance\n- id: CIS_8_1\n  name: CIS Controls v8.1\n- id: SIG\n  name: Shared Assessments SIG\n  evidence: 2025 SigLite questionnaire, updated 2025-04-09\nother_attestations:\n- name: Penetration Test - Attestation 2025\n  note: Independent internal/external penetration test attestation.\n  updated: '2025-12-17'\n- name: Cyber Insurance Attestation\n  updated: '2025-10-17'\n- name: eSentire & Regulation S-P\n  note: Position statement on the U.S. SEC Regulation S-P amendments.\n  updated: '2025-11-25'\n- name: eSentire Statement on Criminal Justice Information Systems (CJIS) Compliance\n  updated: '2025-04-21'\n- name: Data Residency Matrix\n  note: Data elements stored/processed/transmitted and the third-party SaaS/PaaS/CSP subprocessors involved.\n  updated: '2025-05-02'\n- name: eSentire Description of Security Controls\n \
  \ updated: '2025-04-08'\n- name: Modern Slavery Statement\n  updated: '2025-04-25'\n- name: Klue Security Incident\n  note: Published statement on a third-party incident affecting an integration partner.\n  updated: '2026-06-26'\ndocument_access:\n  gated: true\n  note: >-\n    The trust page indexes the documents publicly, but downloading a SOC 2 report or\n    the ISO Statement of Applicability requires requesting access through UpGuard.\n    The index is public; the evidence itself is not.\nscores:\n  upguard_public_score: 867\n  upguard_industry_average: 726\n  note: UpGuard's own security rating of eSentire, published on the trust page. Not an API Evangelist measure.\nevidence_pages:\n- category: privacy\n  url: https://esentire.com/privacy-policy\n- category: tos\n  url: https://esentire.com/terms-and-conditions\nsubprocessors_published: false\ngaps:\n- The trust page is client-side rendered; a human or agent fetching trust.esentire.com without JavaScript receives a 1KB HTML shell\
  \ with no content.\n- The underlying public JSON is undocumented and unversioned — it is UpGuard's internal endpoint, not a contract eSentire offers.\n- Certification documents are request-gated rather than downloadable.\nx-evidence:\n  fetched: '2026-08-12'\n  urls:\n  - url: https://trust.esentire.com/\n    status: 200\n    note: HTML shell, 1083 bytes, no content without JS.\n  - url: https://trust.esentire.com/api/trustpage/public/v1/\n    status: 200\n    content_type: application/json\n    size: 8543\n  - url: https://www.esentire.com/legal/compliance\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esentire/refs/heads/main/security/esentire-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2022, ISO/IEC 27001:2013, PCI DSS 4.0.1, HIPAA, GDPR, CCPA, PIPEDA, DORA (EU Digital Operational Resilience Act), CIS Controls v8.1, Shared Assessments SIG
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Incident Response
- MCP
- Agents
- Authentication
- Software-as-a-Service
trust_url: https://trust.esentire.com/
---
