---
api_specs:
- filename: feedly-streams-openapi.yml
  format: yaml
  label: Feedly API
  slug: feedly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/openapi/feedly-streams-openapi.yml
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
description: Feedly, Inc. runs a public trust portal (Simple Trust Portal). The landing page is public and names its document set; the reports themselves are access-gated behind a "Request Access to All Documents" form. The certifications are therefore publicly ASSERTED even though the evidence is gated.
kind: trust-center
layout: security
name: Feedly Trust Center
name_suffix: Trust Center
overview: Feedly maintains a public trust center documenting SOC 2 Type 1 and SOC 2 Type 2 compliance.
provider_name: Feedly
provider_slug: feedly
slug: feedly-trust-center
source_filename: feedly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://trust.feedly.com/ — fetched 2026-08-12, HTTP 200\nurl: https://trust.feedly.com/\ndescription: >-\n  Feedly, Inc. runs a public trust portal (Simple Trust Portal). The landing page is public and names\n  its document set; the reports themselves are access-gated behind a \"Request Access to All Documents\"\n  form. The certifications are therefore publicly ASSERTED even though the evidence is gated.\n\nplatform: Simple Trust Portal\npublic_landing_page: true\ndocuments_gated: true\n\ncertifications:\n- name: SOC 2 Type 1\n  document_title: Feedly 2026 SOC 2 Type 1 Report\n  year: 2026\n  access: request required\n  evidence: >-\n    Listed in the trust portal document manifest with description \"Feedly Inc. SOC 2 Type 1 Report\n    2026\" and storage filename Feedly-2026-SOC-2-Type-1-Report.pdf.\n- name: SOC 2 Type 2\n  document_title: Feedly 2026 SOC 2 Type 2 Report\n  year: 2026\n  access: request required\n\
  \  evidence: >-\n    Listed in the trust portal document manifest; storage filename\n    Feedly-2026-SOC_2_Type_2_Report.pdf.\n\ndocument_sections:\n- name: Public Documents\n  note: >-\n    \"All documents in this section are public and don't need requests\" — the portal renders a public\n    section, but the two SOC 2 reports sit under the confidential grouping.\n- name: Confidential Documents\n  note: Requires an access request.\n\nnot_listed:\n  note: >-\n    Absence recorded as data. No document in the portal manifest names any of the following.\n  frameworks:\n  - ISO 27001\n  - ISO 27017\n  - ISO 27018\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - CSA STAR\n  - FIPS 140\n  - TISAX\n\nrelated_pages:\n  privacy_policy: https://feedly.com/legal/privacy\n  terms_of_service: https://feedly.com/legal/terms\n  api_terms: https://developers.feedly.com/reference/feedly-api-terms-of-service\n  status_page: https://status.feedly.com/\n\nx-evidence:\n- source: https://trust.feedly.com/\n  http_status:\
  \ 200\n  fetched: '2026-08-12'\n  keywords: [trust portal, SOC 2 Type 1, SOC 2 Type 2, confidential documents, request access]\n\nnote_on_automated_probe: >-\n  0-working/probe-security-programs.py reported trust=none for this provider. That is a\n  false negative: the portal is a JavaScript-rendered single-page app whose document manifest is\n  embedded in a JSON blob rather than in visible HTML text, so the probe's ≥2-keyword body check does\n  not fire. The certifications above were read out of that embedded manifest in the page source. This\n  artifact is therefore method: searched, not probed-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feedly/refs/heads/main/security/feedly-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2
tags:
- threat-intelligence
- cybersecurity
- cyber-threat-intelligence
- content-aggregation
- rss
- news
- vulnerability-management
- indicators-of-compromise
- malware
- threat-actors
- mitre-attack
- security-automation
- artificial-intelligence
- mcp
- agent-native
- webhooks
trust_url: https://trust.feedly.com/
---
