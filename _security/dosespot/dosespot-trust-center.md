---
api_specs:
- filename: dosespot-rest-api-jumpstart-epcs-v2-swagger.json
  format: json
  label: DoseSpot REST API - JumpStart + EPCS - V2
  slug: dosespot-rest-api-jumpstart-epcs-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/_original/dosespot-rest-api-jumpstart-epcs-v2-swagger.json
- filename: dosespot-rest-api-full-epcs-v2-swagger.json
  format: json
  label: DoseSpot REST API - Full + EPCS - V2
  slug: dosespot-rest-api-full-epcs-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/_original/dosespot-rest-api-full-epcs-v2-swagger.json
- filename: dosespot-medications-api-openapi.yml
  format: yaml
  label: DoseSpot Medications API
  slug: dosespot-medications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-medications-api-openapi.yml
- filename: dosespot-notifications-api-openapi.yml
  format: yaml
  label: DoseSpot Notifications API
  slug: dosespot-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-notifications-api-openapi.yml
- filename: dosespot-patients-api-openapi.yml
  format: yaml
  label: DoseSpot Patients API
  slug: dosespot-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-patients-api-openapi.yml
- filename: dosespot-pharmacies-api-openapi.yml
  format: yaml
  label: DoseSpot Pharmacies API
  slug: dosespot-pharmacies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-pharmacies-api-openapi.yml
- filename: dosespot-prescribers-api-openapi.yml
  format: yaml
  label: DoseSpot Prescribers API
  slug: dosespot-prescribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-prescribers-api-openapi.yml
- filename: dosespot-prescriptions-api-openapi.yml
  format: yaml
  label: DoseSpot Prescriptions API
  slug: dosespot-prescriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/openapi/dosespot-prescriptions-api-openapi.yml
certifications:
- SOC 2 Type 2
- HIPAA
- PCI DSS
- NIST
description: ''
kind: trust-center
layout: security
name: Dosespot Trust Center
name_suffix: Trust Center
overview: DoseSpot maintains a public trust center documenting SOC 2 Type 2, HIPAA, PCI DSS, and NIST compliance.
provider_name: DoseSpot
provider_slug: dosespot
slug: dosespot-trust-center
source_filename: dosespot-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nprobe: true\nurl: https://trust.dosespot.com/\nname: Interra Health Trust Center\nplatform: Vanta\noperator: >-\n  Interra Health - the parent brand covering DoseSpot and its subsidiary pVerify. The trust center is served\n  from DoseSpot's own domain (trust.dosespot.com, canonical https://trust.dosespot.com) and is linked from the\n  dosespot.com footer and from https://dosespot.com/security/, so it is DoseSpot's published trust surface even\n  though the page title carries the parent brand.\ncertifications: [SOC 2 Type 2, HIPAA, PCI DSS, NIST]\nin_progress: [HITRUST Tier 2]\ncertification_source: https://dosespot.com/security/\nnote: >-\n  The trust center itself renders client-side (Vanta SPA; a raw fetch returns only the document head with the\n  company description and no control or certification list), so the certification list above is taken from\n  DoseSpot's own /security/ page rather than scraped from the trust center body.\
  \ DoseSpot's /security/ page\n  states of SOC 2: \"Currently, we have the type 2 designation with zero exceptions.\" Requesting reports through\n  the trust center requires an NDA workflow. The automated probe (probe-security-programs.py) recorded\n  trust=none because it requires two or more trust keywords in the fetched body and the body is JS-rendered -\n  this file is the manual, evidenced upgrade of that miss.\nevidence:\n  - {source: 'https://trust.dosespot.com/', http_status: 200, content_type: text/html, signal: 'Vanta trust-center shell, canonical trust.dosespot.com, title \"Interra Health Trust Center\"'}\n  - {source: 'https://dosespot.com/security/', http_status: 200, keywords: [SOC 2 Type 2, HITRUST, HIPAA, NIST, PCI DSS, ONC Certification, Real World Testing]}\n  - {source: 'https://dosespot.com/', http_status: 200, signal: 'footer links to https://trust.dosespot.com/'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dosespot/refs/heads/main/security/dosespot-trust-center.yml
summary_line: SOC 2 Type 2, HIPAA, PCI DSS, NIST
tags:
- e-Prescribing
- eRx
- Healthcare
- EHR
- Pharmacy
- EPCS
- Prescriptions
- Clinical
- Medications
- Prior Authorization
- Surescripts
- Medi-Span
- Telehealth
- PDMP
- Digital Health
trust_url: https://trust.dosespot.com/
---
