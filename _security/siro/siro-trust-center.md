---
api_specs:
- filename: siro-audit-api-openapi.yml
  format: yaml
  label: Siro Audit API
  slug: siro-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-audit-api-openapi.yml
- filename: siro-core-api-openapi.yml
  format: yaml
  label: Siro Core API
  slug: siro-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-core-api-openapi.yml
- filename: siro-folders-api-openapi.yml
  format: yaml
  label: Siro Folders API
  slug: siro-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-folders-api-openapi.yml
- filename: siro-integrations-api-openapi.yml
  format: yaml
  label: Siro Integrations API
  slug: siro-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/siro-integrations-api-openapi.yml
- filename: siro-platform-api-openapi.json
  format: json
  label: Siro Platform API
  slug: siro-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/openapi/_original/siro-platform-api-openapi.json
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Siro Trust Center
name_suffix: Trust Center
overview: Siro maintains a public trust center documenting SOC 2 Type 1 and SOC 2 Type 2 compliance.
provider_name: Siro
provider_slug: siro
slug: siro-trust-center
source_filename: siro-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.siro.ai/\nplatform: Vanta\nsummary: >-\n  Siro operates a Vanta-hosted trust center at trust.siro.ai and has published its security and\n  compliance posture in a dated post on its own site. SOC 2 Type 1 is achieved; SOC 2 Type 2 was\n  stated as in progress as of 2025-04-29.\ncertifications:\n- name: SOC 2 Type 1\n  status: achieved\n  evidence: >-\n    \"Siro has achieved SOC 2 Type 1 compliance\" —\n    https://www.siro.ai/insights/siros-security-posture-and-soc-2-journey (published 2025-04-29)\n- name: SOC 2 Type 2\n  status: in-progress\n  evidence: >-\n    \"we're already hard at work on the SOC 2 Type 2 audit process\" — same post, no target date given.\nsecurity_posture:\n  encryption_at_rest: true\n  encryption_in_transit: true\n  transit_protocol: TLS/SSL\n  hosting: Google Cloud Platform\n  region: US central\n  data_deletion: >-\n    Deletion on request, with backups purged in accordance\
  \ with stated retention policies\n    (\"delete means delete\").\n  penetration_testing: not-published\n  iso_27001: >-\n    Referenced only as a Google Cloud certification, NOT claimed by Siro. Not recorded as a Siro\n    certification.\n  hipaa_gdpr_ccpa: not-published\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt on any Siro host (all /.well-known/security.txt probes 404), no bug bounty on\n    HackerOne/Bugcrowd/Intigriti, and no /security or /responsible-disclosure page — www.siro.ai/security\n    returns 404. probe-security-programs.py returned \"vdp=none\". No Security pointer is emitted;\n    see security/siro-domain-security.yml for the probed transport posture.\nevidence:\n- {source: 'https://trust.siro.ai/', http_status: 200, keywords: [trust center, vanta], note: 'Vanta-hosted SPA; the certification list is rendered client-side from app.vanta.com and is not present in the served HTML, so certifications were taken from Siro''s own dated post\
  \ rather than scraped from the widget.'}\n- {source: 'https://www.siro.ai/insights/siros-security-posture-and-soc-2-journey', http_status: 200, published: '2025-04-29'}\n- {source: 'https://www.siro.ai/security', http_status: 404}\n- {source: 'https://www.siro.ai/.well-known/security.txt', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siro/refs/heads/main/security/siro-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2
tags:
- Company
- Sales
- Sales Coaching
- Conversation Intelligence
- Field Sales
- CRM
- Artificial Intelligence
- Speech-to-Text
- Webhook
- Integration
trust_url: https://trust.siro.ai/
---
