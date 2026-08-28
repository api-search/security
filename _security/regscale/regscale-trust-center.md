---
certifications:
- FedRAMP High
- SOC 2 Type 2
- ISO 27001:2022
- TX-RAMP Level 2
- CSA STAR Level 1
- CSA STAR Valid-AI-ted
- DoD IL5 (in process)
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Regscale Trust Center
name_suffix: Trust Center
overview: RegScale maintains a public trust center documenting FedRAMP High, SOC 2 Type 2, ISO 27001:2022, TX-RAMP Level 2, CSA STAR Level 1, CSA STAR Valid-AI-ted, DoD IL5 (in process), HIPAA, and GDPR compliance.
provider_name: RegScale
provider_slug: regscale
slug: regscale-trust-center
source_filename: regscale-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nprobe: true\nurl: https://trust.regscale.com/\nsource: https://regscale.com/security/\nnote: >-\n  RegScale runs a dedicated trust center at trust.regscale.com (HTTP 200, title \"Trust Center -\n  Compliance Management Platform\"). It is a single-page application that renders its content\n  client-side, so the automated keyword probe found nothing in the served HTML - the\n  certifications recorded below were read from RegScale's own public security page, which\n  states each one with a date and an issuing context. That SPA behaviour is also why every\n  /.well-known/* path on that host answers 200 with the same shell (see\n  well-known/regscale-well-known.yml).\ncertifications:\n- FedRAMP High\n- SOC 2 Type 2\n- ISO 27001:2022\n- TX-RAMP Level 2\n- CSA STAR Level 1\n- CSA STAR Valid-AI-ted\n- 'DoD IL5 (in process)'\n- HIPAA\n- GDPR\ndetail:\n  fedramp_high:\n    authorized: '2025-06'\n    sponsor: DHS\n    marketplace: true\n  soc2_type2:\n\
  \    achieved: '2024-01'\n    availability: upon request\n  iso_27001:\n    version: '2022'\n    controls: 123\n    nonconformities: 0\n    auditor: A-LIGN\n  tx_ramp:\n    level: 2\n    baseline: NIST SP 800-53 Moderate\n  csa_star:\n    level_1: '2024-08'\n    valid_ai_ted: '2025-09'\n    caiq_score: '97.7%'\n  dod_il5:\n    status: in-process\nsbom:\n  published: on-request\n  scope:\n  - Core RegScale Application\n  - RegScale CLI Automation Platform\n  format: not stated\nevidence:\n- source: https://trust.regscale.com/\n  http_status: 200\n  content_type: text/html\n  note: SPA shell; certifications not present in server-rendered HTML\n- source: https://regscale.com/security/\n  http_status: 200\n  keywords: [soc 2 type 2, fedramp high, iso 27001, tx-ramp, csa star, dod il5, sbom]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regscale/refs/heads/main/security/regscale-trust-center.yml
summary_line: FedRAMP High, SOC 2 Type 2, ISO 27001:2022, TX-RAMP Level 2, CSA STAR Level 1, CSA STAR Valid-AI-ted, DoD IL5 (in process), HIPAA, GDPR
tags:
- Company
- Compliance
- Governance Risk and Compliance
- Continuous Controls Monitoring
- Security
- FedRAMP
- OSCAL
- Risk Management
- Audit
- Compliance as Code
- Vulnerability Management
- Government
trust_url: https://trust.regscale.com/
---
