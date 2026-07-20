---
api_specs:
- filename: clawvisor-gateway-openapi.yml
  format: yaml
  label: Clawvisor Gateway API
  slug: clawvisor-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawvisor/refs/heads/main/openapi/clawvisor-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clawvisor.com
  spf: true
hosts:
- cert_expires: Oct 10 06:36:50 2026 GMT
  host: app.clawvisor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clawvisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clawvisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clawvisor
provider_slug: clawvisor
slug: clawvisor-domain-security
source_filename: clawvisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.clawvisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clawvisor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawvisor/refs/heads/main/security/clawvisor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Authorization
- Security
- Identity
- Access Control
- MCP
- Credential Management
- Governance
- Developer Tools
---
