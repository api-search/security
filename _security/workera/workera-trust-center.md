---
api_specs:
- filename: workera-api-openapi.json
  format: json
  label: Workera API
  slug: workera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/openapi/workera-api-openapi.json
certification_count: 4
certifications:
- ISO/IEC 27001
- ISO/IEC 42001
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Workera Trust Center
name_suffix: Trust Center
overview: Workera maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 42001, SOC 2 Type II, and GDPR compliance.
provider_name: Workera
provider_slug: workera
slug: workera-trust-center
source_filename: workera-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.workera.ai/legal/security\nname: Workera Trust Center\nurl: https://trust.workera.ai/\nurl_status: 200\nurl_note: >-\n  trust.workera.ai is a Vanta-hosted trust center (CNAME 60900f408041cfc5165baeab.cname.vantatrust.com).\n  The landing page returns HTTP 200 but the certification list is rendered client-side and is not\n  machine-readable to an anonymous crawler; the certifications below were read from Workera's own\n  first-party security page at https://www.workera.ai/legal/security.\ncertifications:\n- name: ISO/IEC 27001\n  scope: Information Security Management System (ISMS)\n  evidence: https://www.workera.ai/legal/security\n- name: ISO/IEC 42001\n  scope: Artificial Intelligence Management System (AIMS)\n  evidence: https://www.workera.ai/legal/security\n- name: SOC 2 Type II\n  scope: Service organization controls, Type II report\n  evidence: https://www.workera.ai/legal/security\n- name: GDPR\n  scope:\
  \ EU General Data Protection Regulation compliance program\n  evidence: https://www.workera.ai/legal/security\ndocument_access:\n  self_serve: false\n  note: >-\n    SOC 2 Type II reports, ISO certificates, penetration-test summaries and security policies are\n    released to authorized customers and prospective customers on request, not published openly.\npractices:\n- independent third-party penetration testing\n- continuous security monitoring\naudit_surface:\n  api: GET /api/v1/audit_events\n  note: >-\n    Workera exposes a SIEM-compatible enterprise audit-event feed over the public REST API, gated by\n    an `audit_events` API-key scope. See conformance/workera-conformance.yml.\nevidence:\n- url: https://www.workera.ai/legal/security\n  status: 200\n- url: https://trust.workera.ai/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workera/refs/heads/main/security/workera-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 42001, SOC 2 Type II, GDPR
tags:
- Skills Intelligence
- Skills Assessment
- Human Resources
- Learning and Development
- Talent Management
- Workforce Analytics
- Artificial Intelligence
- Benchmarking
- Enterprise Software
- MCP
- Company
trust_url: https://trust.workera.ai/
---
