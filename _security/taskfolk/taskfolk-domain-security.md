---
api_specs:
- filename: taskfolk-product-api-openapi.yml
  format: yaml
  label: Taskfolk API
  slug: taskfolk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-product-api-openapi.yml
- filename: taskfolk-agent-commerce-openapi.yml
  format: yaml
  label: Taskfolk Agent Commerce API
  slug: taskfolk-agent-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/openapi/taskfolk-agent-commerce-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: taskfolk.ai
  spf: true
hosts:
- cert_expires: Nov  6 13:37:44 2026 GMT
  host: taskfolk.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taskfolk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taskfolk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Taskfolk
provider_slug: taskfolk
slug: taskfolk-domain-security
source_filename: taskfolk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taskfolk.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 13:37:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taskfolk.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taskfolk/refs/heads/main/security/taskfolk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Project Management
- Issue Tracking
- Task Management
- Productivity
- Collaboration
- MCP
- AI Agents
- agent-native
- Agentic Commerce
- A2A
- REST API
- OpenAPI
- Webhook
- Authentication
- Agile
- Sprints
- OKR
- Developer Tools
---
