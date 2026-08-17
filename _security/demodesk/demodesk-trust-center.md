---
api_specs:
- filename: demodesk-externally-recorded-demos-api-openapi.yml
  format: yaml
  label: Demodesk Externally recorded demos API
  slug: demodesk-externally-recorded-demos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-externally-recorded-demos-api-openapi.yml
- filename: demodesk-recordings-api-openapi.yml
  format: yaml
  label: Demodesk Recordings API
  slug: demodesk-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-recordings-api-openapi.yml
- filename: demodesk-users-api-openapi.yml
  format: yaml
  label: Demodesk Users API
  slug: demodesk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-users-api-openapi.yml
certifications:
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Demodesk Trust Center
name_suffix: Trust Center
overview: Demodesk maintains a public trust center documenting ISO 27001 and GDPR compliance.
provider_name: Demodesk
provider_slug: demodesk
slug: demodesk-trust-center
source_filename: demodesk-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://security.demodesk.com\nurl: https://security.demodesk.com\nplatform: Vanta Trust Center\nplatform_evidence: >-\n  https://security.demodesk.com returns 200 and its HTML shell is Vanta's\n  (assets.vanta.com signature manifest, static.vanta.com API version endpoint) —\n  a hosted trust center on a dedicated subdomain, not a marketing page.\ncertifications:\n- ISO 27001\n- GDPR\nevidence:\n- source: https://security.demodesk.com\n  http_status: 200\n  note: >-\n    Vanta-hosted trust center on a Demodesk-controlled subdomain. Contents are\n    JS-rendered, so the certification list below is corroborated from the\n    provider's own text rather than scraped from the SPA.\n- source: https://demodesk.com/legal/privacy-policy\n  keywords:\n  - iso 27001\n  - gdpr\n- source: https://demodesk.com/llms.txt\n  keywords:\n  - ISO 27001:2022 certified\n  - GDPR-native\n  - EU-only data (Azure Frankfurt)\n- source:\
  \ https://mcp.demodesk.ai/llms.txt\n  keywords:\n  - 'Trust: ISO 27001:2022, GDPR-native, EU-only data (Azure Frankfurt)'\nvulnerability_disclosure:\n  published: false\n  checked: '2026-08-14'\n  evidence:\n  - url: https://demodesk.com/.well-known/security.txt\n    status: 404\n  - url: https://demodesk.com/security.txt\n    status: 404\n  - url: https://security.demodesk.com/.well-known/security.txt\n    status: 200\n    document: false\n    note: SPA catch-all returning HTML for every path — a soft 200, not an RFC 9116 document.\n  note: >-\n    No security.txt, no bug-bounty program (HackerOne / Bugcrowd / Intigriti) and\n    no disclosure page found. security/demodesk-vulnerability-disclosure.yml was\n    deliberately NOT written and no `type: Security` pointer is wired — the\n    absence is the finding. This is the single clearest remediation available to\n    Demodesk: an ISO 27001:2022-certified company with a Vanta trust center that\n    does not serve a two-line security.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/security/demodesk-trust-center.yml
summary_line: ISO 27001, GDPR
tags:
- Company
- Sales
- AI
- Conversation Intelligence
- Video Conferencing
- CRM
- Transcription
- Webhooks
- MCP
trust_url: https://security.demodesk.com
---
