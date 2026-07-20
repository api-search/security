---
api_specs:
- filename: bluejay-openapi-original.json
  format: json
  label: Bluejay API
  slug: bluejay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay/refs/heads/main/openapi/bluejay-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbluejay.ai
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: getbluejay.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:25:36 2026 GMT
  host: api.getbluejay.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluejay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluejay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bluejay
provider_slug: bluejay
slug: bluejay-domain-security
source_filename: bluejay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbluejay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getbluejay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:25:36 2026 GMT\n  hsts: null\ndomains:\n- domain: getbluejay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluejay/refs/heads/main/security/bluejay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Agents
- Voice AI
- Conversational AI
- Agent Testing
- Quality Assurance
- Observability
- Simulation
- Evaluation
- Monitoring
---
