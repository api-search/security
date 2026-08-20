---
api_specs:
- filename: flume-health-console-api-openapi.yml
  format: yaml
  label: Flume Console API
  slug: flume-console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-console-api-openapi.yml
certifications:
- SOC 2 Type II
- HITRUST CSF
- HIPAA
description: ''
kind: trust-center
layout: security
name: Flume Health Trust Center
name_suffix: Trust Center
overview: Flume Health maintains a public trust center documenting SOC 2 Type II, HITRUST CSF, and HIPAA compliance.
provider_name: Flume Health
provider_slug: flume-health
slug: flume-health-trust-center
source_filename: flume-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nprobe: true\nsource: https://www.flumehealth.com/security\nurl: https://www.flumehealth.com/security\nnote: >-\n  Flume Health names its compliance posture on a marketing security page. There is no trust portal, no evidence\n  room, no auditor named, no attestation date, no report request flow, and no downloadable artifact behind any of\n  the three claims — the page states them and stops. That is recorded faithfully below: `claimed`, not `verified`.\ntrust_portal: false\ntrust_portal_url: null\nreport_request_flow: false\ncertifications:\n- name: SOC 2 Type II\n  id: soc2-type-ii\n  claimed: true\n  verified: false\n  evidence_url: https://www.flumehealth.com/security\n  detail: Named on the public security page. No auditor, no report period, no attestation date, no report access flow.\n- name: HITRUST CSF\n  id: hitrust-csf\n  claimed: true\n  verified: false\n  evidence_url: https://www.flumehealth.com/security\n  detail: Named\
  \ on the public security page. Certification level (e1/i1/r2) and validity dates not published.\n- name: HIPAA\n  id: hipaa\n  claimed: partial\n  verified: false\n  evidence_url: https://www.flumehealth.com/security\n  detail: >-\n    The page says \"HIPAA-aligned controls\" — it does not claim certification (no such certification exists) and\n    publishes no BAA, covered-entity/business-associate posture, or breach-notification commitment.\ndata_residency:\n  claim: >-\n    The platform is described on www.flumehealth.com as running on portable, customer-owned infrastructure —\n    \"your data never leaves your environment.\"\n  evidence_url: https://www.flumehealth.com/\ngaps:\n- No trust center or evidence portal.\n- No named auditor or attestation dates for SOC 2 or HITRUST.\n- No subprocessor list published.\n- No penetration-test summary published.\nevidence:\n- url: https://www.flumehealth.com/security\n  http_status: 200\n  keywords: [soc 2 type ii, hitrust csf, hipaa-aligned\
  \ controls]\n- url: https://www.flumehealth.com/trust\n  http_status: 404\nchecked: '2026-08-16'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/security/flume-health-trust-center.yml
summary_line: SOC 2 Type II, HITRUST CSF, HIPAA
tags:
- Healthcare
- Health Plans
- Payers
- Healthcare Data
- Data Integration
- iPaaS
- Eligibility
- Claims
- Knowledge Graph
- MCP
- agent-native
- Authentication
- Data Engineering
- Interoperability
trust_url: https://www.flumehealth.com/security
---
