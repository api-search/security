---
api_specs:
- filename: 2s-io-openapi.json
  format: json
  label: 2s API
  slug: 2s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2s-io/refs/heads/main/openapi/2s-io-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 2s.io
  spf: false
hosts:
- cert_expires: Nov 21 17:16:33 2026 GMT
  host: 2s.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 2S Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2s, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: 2s
provider_slug: 2s-io
slug: 2s-io-domain-security
source_filename: 2s-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2s.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 17:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 2s.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2s-io/refs/heads/main/security/2s-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agentic Commerce
- x402
- MCP
- A2A
- Public Records
- Government Data
- Finance
- Crypto
- Security
- Legal
- Weather
- Geocoding
- EDI
- AI Gateway
- Agent Infrastructure
- Webhook
- Agent-Native
---
