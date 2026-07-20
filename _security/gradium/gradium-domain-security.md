---
api_specs:
- filename: gradium-openapi-original.json
  format: json
  label: Gradium API
  slug: gradium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradium/refs/heads/main/openapi/gradium-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gradium.ai
  spf: true
hosts:
- cert_expires: Aug 24 13:22:38 2026 GMT
  host: gradium.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 13:48:29 2026 GMT
  host: api.gradium.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gradium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gradium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gradium
provider_slug: gradium
slug: gradium-domain-security
source_filename: gradium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gradium.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:22:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gradium.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:48:29 2026 GMT\n  hsts: null\ndomains:\n- domain: gradium.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradium/refs/heads/main/security/gradium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Voice AI
- Text-to-Speech
- Speech-to-Text
- Speech-to-Speech
- Voice Cloning
- Audio
- Real-Time Streaming
- WebSocket
- Developer API
- Voice Agents
---
