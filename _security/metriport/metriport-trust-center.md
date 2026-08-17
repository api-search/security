---
api_specs:
- filename: metriport-consolidated-api-openapi.yml
  format: yaml
  label: Metriport Consolidated API
  slug: metriport-consolidated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-consolidated-api-openapi.yml
- filename: metriport-devices-data-api-openapi.yml
  format: yaml
  label: Metriport Devices Data API
  slug: metriport-devices-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-devices-data-api-openapi.yml
- filename: metriport-document-api-openapi.yml
  format: yaml
  label: Metriport Document API
  slug: metriport-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-document-api-openapi.yml
- filename: metriport-facility-api-openapi.yml
  format: yaml
  label: Metriport Facility API
  slug: metriport-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-facility-api-openapi.yml
- filename: metriport-patient-api-openapi.yml
  format: yaml
  label: Metriport Patient API
  slug: metriport-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-patient-api-openapi.yml
- filename: metriport-settings-api-openapi.yml
  format: yaml
  label: Metriport Settings API
  slug: metriport-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-settings-api-openapi.yml
- filename: metriport-user-api-openapi.yml
  format: yaml
  label: Metriport User API
  slug: metriport-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/openapi/metriport-user-api-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA
description: 'Metriport runs a trust center at security.metriport.com and links to it from the homepage. The certifications themselves are stated on the marketing site, not in the trust center — the trust center is a client-rendered React application that ships a 604-byte HTML shell with an empty #root div, so an unauthenticated non-JavaScript client (including every agent and crawler) reads zero certifications from it. Nothing was extractable from the JS bundle either: no SOC, HIPAA, ISO or subprocessor strings appear in it, so the content is fetched at runtime from an endpoint not discoverable anonymously.'
kind: trust-center
layout: security
name: Metriport Trust Center
name_suffix: Trust Center
overview: Metriport maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: Metriport
provider_slug: metriport
slug: metriport-trust-center
source_filename: metriport-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://security.metriport.com (probed 2026-08-14, HTTP 200) and\n  https://www.metriport.com (the security section of the marketing homepage,\n  which is where the named certifications actually are).\ndescription: >-\n  Metriport runs a trust center at security.metriport.com and links to it from\n  the homepage. The certifications themselves are stated on the marketing site,\n  not in the trust center — the trust center is a client-rendered React\n  application that ships a 604-byte HTML shell with an empty #root div, so an\n  unauthenticated non-JavaScript client (including every agent and crawler)\n  reads zero certifications from it. Nothing was extractable from the JS bundle\n  either: no SOC, HIPAA, ISO or subprocessor strings appear in it, so the\n  content is fetched at runtime from an endpoint not discoverable anonymously.\ntrust_center:\n  url: https://security.metriport.com\n  http_status: 200\n  content_type:\
  \ text/html\n  machine_readable: false\n  rendering: client-side (React/Vite SPA, empty #root, no server-rendered content)\n  shell_bytes: 604\n  linked_from: https://www.metriport.com\ncertifications:\n  - name: SOC 2 Type II\n    status: claimed\n    evidence_url: https://www.metriport.com\n    evidence_quote: >-\n      \"We are a certified HIPAA and SOC 2 Type 2 compliant organization, and\n      follow best industry-best practices such as MFA.\"\n    report_available: not publicly — no attestation letter, report or NDA-gated request flow is reachable anonymously\n  - name: HIPAA\n    status: claimed\n    evidence_url: https://www.metriport.com\n    evidence_quote: '\"HIPAA Compliant\" / \"a certified HIPAA and SOC 2 Type 2 compliant organization\"'\n    note: >-\n      HIPAA has no certification body, so \"certified HIPAA compliant\" is a\n      marketing formulation rather than a third-party attestation. BAA terms are\n      a commercial-agreement item (plans/metriport-plans-pricing.yml).\n\
  controls_claimed:\n  - Externally audited\n  - Fully encrypted\n  - MFA\n  - VPN\ncompliance_automation:\n  vendor: Vanta\n  evidence: https://www.vanta.com/ is linked from the security section of https://www.metriport.com (\"uses Third Party Standards for automated compliance monitoring\").\nnot_found:\n  - ISO 27001\n  - HITRUST\n  - PCI DSS\n  - FedRAMP\n  - GDPR statement\n  - Published subprocessor list\n  - Downloadable or NDA-gated report request\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metriport/refs/heads/main/security/metriport-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Healthcare
- Medical Records
- FHIR
- Health Data
- Wearables
- Open Source
trust_url: ''
---
