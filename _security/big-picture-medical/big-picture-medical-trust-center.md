---
certifications:
- ISO/IEC 27001:2022
- Cyber Essentials
- HIPAA
- GDPR
- WCAG 2.1 AA
description: ''
kind: trust-center
layout: security
name: Big Picture Medical Trust Center
name_suffix: Trust Center
overview: Big Picture Medical maintains a public trust center documenting ISO/IEC 27001:2022, Cyber Essentials, HIPAA, GDPR, and WCAG 2.1 AA compliance.
provider_name: Big Picture Medical
provider_slug: big-picture-medical
slug: big-picture-medical-trust-center
source_filename: big-picture-medical-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nprobe: true\nsource: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\nurl: https://trust.bigpicturemedical.com/\nplatform: SafeBase (CNAME bigpicturemedical.portals.safebase.io)\nurl_status: 403\nurl_status_note: >-\n  The trust centre is real and linked from the footer of every page on\n  bigpicturemedical.com, but it sits behind a Cloudflare bot interstitial that answered\n  HTTP 403 \"Just a moment...\" to our fetch, including at the portal's own SafeBase\n  hostname. That is an ordinary edge policy turning away a crawler, not a dead page — the\n  DNS record, the CNAME to SafeBase's portal service and the site-wide footer link all\n  establish that the page exists. Its CONTENTS were therefore not read by us. Every\n  certification listed below is taken instead from two documents we did fetch at 200: the\n  company's own homepage badge row and its G-Cloud 14 Digital Marketplace listing.\n\
  certifications:\n- ISO/IEC 27001:2022\n- Cyber Essentials\n- HIPAA\n- GDPR\n- WCAG 2.1 AA\ncertification_detail:\n- name: ISO/IEC 27001\n  status: certified\n  accreditor: UKAS\n  accreditation_date: '2022-07-05'\n  scope: >-\n    \"Provision of a SaaS-based intelligent pathway technology to support collaborative\n    healthcare delivery and clinical research within the healthcare eco-system\"\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\n- name: Cyber Essentials\n  status: certified\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\n- name: Cyber Essentials Plus\n  status: claimed-on-website-but-answered-No-on-G-Cloud-14\n  note: >-\n    bigpicturemedical.com's homepage badge row advertises \"Cyber Essentials Plus —\n    Independently audited\". The company's G-Cloud 14 submission (May 2024) answers \"Cyber\n    essentials plus: No\". Recorded as a discrepancy, not resolved\
  \ in either direction.\n  sources:\n  - https://www.bigpicturemedical.com/\n  - https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\n- name: HIPAA Seal of Compliance\n  status: claimed\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\n- name: PCI DSS\n  status: not certified\n  source: 'G-Cloud 14: \"PCI certification: No\"'\n- name: CSA STAR\n  status: not certified\n  source: 'G-Cloud 14: \"CSA STAR certification: No\"'\n- name: SOC 2\n  status: not claimed anywhere we could read\nsecurity_program:\n  penetration_testing: at least once a year, \"IT Health Check\" performed by a CHECK service provider\n  access_restriction_testing: at least every 6 months\n  data_at_rest: encrypted at rest using cloud-provider managed functionality with application-specific keys\n  data_in_transit: TLS 1.2 or above, buyer-to-supplier and within the supplier network\n  data_location: United Kingdom\n  authentication:\
  \ 2-factor authentication for users; RBAC plus MFA and VPN-limited environment access for management interfaces\n  governance: >-\n    Named board-level person responsible for service security; ISMS Management Review Board\n    and an InfoSec & Privacy Working Group reporting to it; regular internal audits; staff\n    attestation to key policies on commencement.\n  vulnerability_management: >-\n    Automated continuous monitoring of project dependencies for known vulnerabilities, with\n    automatic pull requests to update affected dependencies and integrated security\n    advisories. Conforms to a recognised standard per the G-Cloud answer.\n  secure_development: independent review of processes (ISO/IEC 27034 / ISO/IEC 27001 / CSA CCM v3.0 class)\n  log_retention: at least 12 months for user, supplier and system audit data\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No coordinated vulnerability disclosure surface was found. /.well-known/security.txt\n    404s, /security\
  \ 404s, and no HackerOne, Bugcrowd or Intigriti program could be located.\n    A published security.txt with a Contact and Policy line is the cheapest single fix\n    available here. No Security or VulnerabilityDisclosure pointer is emitted.\nevidence:\n- source: https://www.bigpicturemedical.com/\n  status: 200\n  keywords: [Cyber Essentials, Cyber Essentials Plus, G-Cloud, GDPR, HIPAA, 'ISO/IEC 27001:2022', Trust Centre]\n- source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\n  status: 200\n  keywords: ['ISO/IEC 27001', UKAS, Cyber essentials, HIPAA Seal of Compliance, CHECK]\n- source: https://trust.bigpicturemedical.com/\n  status: 403\n  keywords: []\n  note: Cloudflare bot challenge; contents not read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-picture-medical/refs/heads/main/security/big-picture-medical-trust-center.yml
summary_line: ISO/IEC 27001:2022, Cyber Essentials, HIPAA, GDPR, WCAG 2.1 AA
tags:
- Company
- Healthcare
- Health Care
- Electronic Health Records
- openEHR
- FHIR
- HL7
- Interoperability
- Clinical Data
- Care Pathways
- Workflow
- Orchestration
- No Code
- NHS
- United Kingdom
trust_url: https://trust.bigpicturemedical.com/
---
