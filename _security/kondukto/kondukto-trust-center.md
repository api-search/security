---
api_specs:
- filename: kondukto-authorization-managers-api-openapi.yml
  format: yaml
  label: Kondukto Authorization Managers API
  slug: kondukto-authorization-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-authorization-managers-api-openapi.yml
- filename: kondukto-events-api-openapi.yml
  format: yaml
  label: Kondukto Events API
  slug: kondukto-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-events-api-openapi.yml
- filename: kondukto-health-api-openapi.yml
  format: yaml
  label: Kondukto Health API
  slug: kondukto-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-health-api-openapi.yml
- filename: kondukto-labels-api-openapi.yml
  format: yaml
  label: Kondukto Labels API
  slug: kondukto-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-labels-api-openapi.yml
- filename: kondukto-products-api-openapi.yml
  format: yaml
  label: Kondukto Products API
  slug: kondukto-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-products-api-openapi.yml
- filename: kondukto-projects-api-openapi.yml
  format: yaml
  label: Kondukto Projects API
  slug: kondukto-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-projects-api-openapi.yml
- filename: kondukto-scanners-api-openapi.yml
  format: yaml
  label: Kondukto Scanners API
  slug: kondukto-scanners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-scanners-api-openapi.yml
- filename: kondukto-scans-api-openapi.yml
  format: yaml
  label: Kondukto Scans API
  slug: kondukto-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-scans-api-openapi.yml
- filename: kondukto-teams-api-openapi.yml
  format: yaml
  label: Kondukto Teams API
  slug: kondukto-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-teams-api-openapi.yml
- filename: kondukto-users-api-openapi.yml
  format: yaml
  label: Kondukto Users API
  slug: kondukto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-users-api-openapi.yml
- filename: kondukto-vulnerabilities-api-openapi.yml
  format: yaml
  label: Kondukto Vulnerabilities API
  slug: kondukto-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-vulnerabilities-api-openapi.yml
certifications:
- SOC 2 Type 2
- ISO 27001:2025
description: ''
kind: trust-center
layout: security
name: Kondukto Trust Center
name_suffix: Trust Center
overview: Kondukto maintains a public trust center documenting SOC 2 Type 2 and ISO 27001:2025 compliance.
provider_name: Kondukto
provider_slug: kondukto
slug: kondukto-trust-center
source_filename: kondukto-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.invicti.com\ncompliance_page: https://www.invicti.com/compliance/\nnotes: >-\n  Kondukto has no standalone trust centre; post-acquisition the compliance posture for the ASPM\n  product is published on Invicti's properties. trust.invicti.com resolves and returns 200 but is a\n  JavaScript-rendered trust-portal application whose certification list could not be read from the\n  raw HTML. The certifications recorded below were verified in the server-rendered text of\n  https://www.invicti.com/compliance/ and are quoted as that page names them.\ncertifications:\n- name: SOC 2 Type 2\n  evidence: >-\n    \"Our SOC 2 Type 2 report validates internal controls and systems related to security\n    availability, processing integrity, confidentiality, and data privacy.\" (invicti.com/compliance)\n  artifact: report available on request via the compliance page\n- name: ISO 27001:2025\n  evidence: >-\n    \"Our Information\
  \ Security Management Systems meet international security standards in data\n    protection.\" (invicti.com/compliance)\n  artifact: certificate linked from the compliance page\npolicies:\n- name: Information Security Policy\n  url: https://www.invicti.com/compliance/\n  note: Invicti's published commitment to maintaining information security controls.\nnot_found:\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- FIPS 140\nnot_found_note: >-\n  These frameworks were probed for and are not named on the compliance page; absence here is\n  recorded data, not a claim that they do not exist elsewhere.\nevidence:\n- source: https://trust.invicti.com\n  status: 200\n  keywords: []\n  note: JS-rendered trust portal; body contains only a loading shim.\n- source: https://www.invicti.com/compliance/\n  status: 200\n  keywords: [soc 2 type 2, 'iso 27001:2025', enterprise compliance, information security policy]\n- source: https://www.invicti.com/trust-center/\n  status: 404\nrelated:\n  conformance: conformance/kondukto-conformance.yml\n\
  \  vulnerability_disclosure: security/kondukto-vulnerability-disclosure.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/security/kondukto-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001:2025
tags:
- Company
- Application Security
- ASPM
- Vulnerability Management
- DevSecOps
- Security Orchestration
- SAST
- DAST
- SCA
- Software Composition Analysis
- Container Security
- SBOM
- Security Testing
- CI/CD
- Security
trust_url: https://trust.invicti.com
---
