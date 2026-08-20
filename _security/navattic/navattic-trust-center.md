---
api_specs:
- filename: navattic-website-openapi.json
  format: json
  label: Navattic API
  slug: navattic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/openapi/navattic-website-openapi.json
certifications:
- SOC 2 Type II
- GDPR
description: 'Navattic runs a trust center at https://trust.navattic.com/ and links to it from its documentation as the place to get certifications, security documentation and vendor-questionnaire support. The certifications recorded here are named in Navattic''s own documentation; they were NOT read off the trust center itself, because that page renders client-side and returns no certification text to a non-JS fetch.

  '
kind: trust-center
layout: security
name: Navattic Trust Center
name_suffix: Trust Center
overview: Navattic maintains a public trust center documenting SOC 2 Type II and GDPR compliance.
provider_name: Navattic
provider_slug: navattic
slug: navattic-trust-center
source_filename: navattic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://docs.navattic.com/workspace/security\nurl: https://trust.navattic.com/\ncertifications:\n  - SOC 2 Type II\n  - GDPR\ndescription: >\n  Navattic runs a trust center at https://trust.navattic.com/ and links to it\n  from its documentation as the place to get certifications, security\n  documentation and vendor-questionnaire support. The certifications recorded\n  here are named in Navattic's own documentation; they were NOT read off the\n  trust center itself, because that page renders client-side and returns no\n  certification text to a non-JS fetch.\nevidence:\n  - source: https://docs.navattic.com/workspace/security\n    kind: docs security page\n    http_status: 200\n    quote: >\n      \"Current certifications — including SOC 2 Type II and GDPR compliance —\n      are listed on the Navattic Trust Center.\"\n  - source: https://trust.navattic.com/\n    kind: trust center\n    http_status: 200\n    keywords:\
  \ []\n    note: >\n      Reachable but JS-rendered — a plain fetch returns only the \"Navattic Trust\n      Center\" heading, which is why the automated probe\n      (probe-security-programs.py) recorded trust=none. Certifications above are\n      sourced from the docs instead.\ncontact:\n  - success@navattic.com\ndocuments:\n  available_on_request: true\n  note: >\n    The docs direct infosec teams to the trust center to download security\n    reports and policies, or to email success@navattic.com for custom security\n    materials and vendor questionnaires. Whether an NDA gate applies could not\n    be determined without JS.\nsecurity_posture_documented:\n  data_capture: >\n    Demos are static HTML/media snapshots of the customer's application —\n    Navattic holds no live connection to the customer's product or its\n    underlying data, so demo visitors never touch the real application.\n  content_redaction: [blur tool, text edit/replace, per-capture deletion]\n  demo_access_controls:\
  \ [link expiration, password protection, email domain restriction, form gating, revoke access]\n  workspace_controls: [SSO, SCIM directory sync, audit logs (Enterprise), custom domains]\n  roles: [Admin, Builder, Rep]\n  ai_data_use: >\n    \"Navattic does not use your demo content to train AI models\" — consistent\n    with the Content-Signal ai-train=no published in robots.txt.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navattic/refs/heads/main/security/navattic-trust-center.yml
summary_line: SOC 2 Type II, GDPR
tags:
- Interactive Demos
- Product Demo
- Sales Enablement
- Marketing
- No-Code
- Webhook
- CRM Integration
- Sales Automation
- MCP
- Agents
- Product Analytics
trust_url: https://trust.navattic.com/
---
