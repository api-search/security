---
api_specs:
- filename: tadeus-api-integration-openapi.json
  format: json
  label: Tadeus Integration API
  slug: tadeus-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/openapi/tadeus-api-integration-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tadeus.net
  spf: true
hosts:
- cert_expires: Oct  9 03:57:00 2026 GMT
  host: app.tadeus.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tadeus Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tadeus API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tadeus API
provider_slug: tadeus-api
slug: tadeus-api-domain-security
source_filename: tadeus-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.tadeus.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:57:00 2026 GMT\n  hsts: false\ndomains:\n- domain: tadeus.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tadeus-api/refs/heads/main/security/tadeus-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Voice AI
- Research
- Interviews
- Workforce
- HR Tech
- Conversational AI
- Employee Experience
- AI Agents
- MCP
- EU AI Act
- Compliance
- Employee Engagement
---
