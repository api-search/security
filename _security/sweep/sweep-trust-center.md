---
api_specs:
- filename: sweep-api-openapi.yml
  format: yaml
  label: Sweep API
  slug: sweep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/openapi/sweep-api-openapi.yml
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Sweep Trust Center
name_suffix: Trust Center
overview: Sweep maintains a public trust center documenting SOC 2 compliance.
provider_name: Sweep
provider_slug: sweep
slug: sweep-trust-center
source_filename: sweep-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nprobe: true\nurl: https://security.sweep.io/\nplatform: Scytale (the trust-centre bundle loads https://api.scytale.ai)\ncertifications:\n- SOC 2\ncertifications_source: https://www.sweep.io/security-compliance-governance — the provider states \"SOC2\n  compliant\". The trust centre itself is client-side rendered, so its certification list is not machine-readable.\nevidence:\n- source: https://security.sweep.io/\n  http_status: 200\n  content_type: text/html\n  signal: <title>Trust Center</title>; SPA shell served from Sweep's own subdomain\n- source: https://security.sweep.io/main.8f323eb1d028c9a65ab0.js\n  http_status: 200\n  signal: references https://api.scytale.ai — Scytale-operated trust centre\n- source: https://www.sweep.io/security-compliance-governance\n  http_status: 200\n  signal: '\"SOC2 compliant\"'\nmachine_readable: false\nnotes: 'The trust centre is real but JS-rendered: every path under security.sweep.io returns the\
  \ same\n  200 HTML shell, so the certification list, sub-processors and documents cannot be read without executing\n  JavaScript. Recorded as a verified presence with an unreadable payload.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/security/sweep-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Cloud
- Salesforce
- Revenue Operations
- Metadata
- Governance
- AI Agents
- MCP
- Automation
- Documentation
- REST API
- OpenAPI
- Enterprise Systems
- Snowflake
- ServiceNow
- Data Governance
trust_url: https://security.sweep.io/
---
