---
api_specs:
- filename: barndoor-openapi.yml
  format: yaml
  label: Barndoor Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barndoor/refs/heads/main/openapi/barndoor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: barndoor.ai
  spf: true
hosts:
- cert_expires: Sep 17 21:28:49 2026 GMT
  host: barndoor.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:21:36 2026 GMT
  host: app.barndoor.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:21:36 2026 GMT
  host: docs.barndoor.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barndoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barndoor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Barndoor
provider_slug: barndoor
slug: barndoor-domain-security
source_filename: barndoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barndoor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:28:49 2026 GMT\n  hsts: false\n- host: app.barndoor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.barndoor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: barndoor.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barndoor/refs/heads/main/security/barndoor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- AI Governance
- Agentic AI
- MCP
- Model Context Protocol
- Policy Enforcement
- OAuth
- Identity
- Security
- Audit
- Control Plane
---
