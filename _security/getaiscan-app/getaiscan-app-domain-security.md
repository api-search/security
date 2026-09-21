---
api_specs:
- filename: getaiscan-app-openapi.json
  format: json
  label: AIScan Agent API
  slug: aiscan-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaiscan-app/refs/heads/main/openapi/getaiscan-app-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getaiscan.app
  spf: false
hosts:
- cert_expires: Oct 29 17:18:57 2026 GMT
  host: getaiscan.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 19:20:56 2026 GMT
  host: api.getaiscan.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Getaiscan App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIScan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AIScan
provider_slug: getaiscan-app
slug: getaiscan-app-domain-security
source_filename: getaiscan-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getaiscan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 17:18:57 2026 GMT\n  hsts: false\n- host: api.getaiscan.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 19:20:56 2026 GMT\n  hsts: false\ndomains:\n- domain: getaiscan.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaiscan-app/refs/heads/main/security/getaiscan-app-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Visibility
- Website Auditing
- SEO
- Answer Engine Optimization
- Generative Engine Optimization
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- agent-native
---
