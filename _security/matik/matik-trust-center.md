---
api_specs:
- filename: matik-oauth-postman-collection.json
  format: json
  label: Matik External API
  slug: matik-external-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/matik/refs/heads/main/postman/matik-oauth-postman-collection.json
certifications:
- SOC 2 Type I
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Matik Trust Center
name_suffix: Trust Center
overview: Matik maintains a public trust center documenting SOC 2 Type I, SOC 2 Type II, and GDPR compliance.
provider_name: Matik
provider_slug: matik
slug: matik-trust-center
source_filename: matik-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nprobe: true\nsource: https://www.matik.io/security\nurl: https://www.matik.io/security\ncertifications:\n- SOC 2 Type I\n- SOC 2 Type II\n- GDPR\npractices:\n- AES-256 encryption at rest\n- AWS infrastructure with CloudTrail logging and WAF\n- Role-based access control (RBAC)\n- Enforced two-factor authentication\n- 72-hour breach notification\n- Daily database backups retained 30 days\ncontact: hello@matik.io\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Re-probed 2026-08-14: https://www.matik.io/security returns 200 (~20k chars) and\n    contains no \"disclosure\", \"vulnerability\", \"bug bounty\", \"security@\", \"penetration\"\n    or \"report a\". No /.well-known/security.txt on any Matik-controlled host, and no\n    HackerOne/Bugcrowd/Intigriti program. There is no published route to report a\n    vulnerability — only hello@matik.io as a general contact.\nevidence:\n- source: https://www.matik.io/security\n\
  \  keywords:\n  - soc 2\n  - soc2\n  - gdpr\nx-recheck: '2026-08-14'\nx-recheck-note: >-\n  Content re-verified 2026-08-14; certifications and practices unchanged. The mechanical\n  probe would have flattened \"SOC 2 Type I\"/\"SOC 2 Type II\" to \"SOC 2\" and dropped the\n  practices list and contact, so its weaker output was discarded per the pipeline's\n  never-downgrade rule.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matik/refs/heads/main/security/matik-trust-center.yml
summary_line: SOC 2 Type I, SOC 2 Type II, GDPR
tags:
- Company
- Content Automation
- Presentations
- Documents
- Data-Driven Content
- Sales Enablement
- Customer Success
- Revenue Operations
- AI
- MCP
trust_url: https://www.matik.io/security
---
