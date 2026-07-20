---
api_specs:
- filename: c1-openapi-original.yml
  format: yaml
  label: ConductorOne API
  slug: conductorone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c1/refs/heads/main/openapi/c1-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: c1.ai
  spf: true
hosts:
- cert_expires: Aug 24 12:35:15 2026 GMT
  host: c1.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: C1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: C1
provider_slug: c1
slug: c1-domain-security
source_filename: c1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: c1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:35:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: c1.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c1/refs/heads/main/security/c1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Access Management
- IAM
- Identity Governance
- Access Control
- Authorization
- AI Agents
- MCP
- Security
---
