---
api_specs:
- filename: anam-openapi-original.json
  format: json
  label: Anam AI API
  slug: anam-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/openapi/anam-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anam.ai
  spf: true
hosts:
- cert_expires: Sep 15 19:51:51 2026 GMT
  host: www.anam.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anam
provider_slug: anam
slug: anam-domain-security
source_filename: anam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anam/refs/heads/main/security/anam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Avatars
- Conversational AI
- Video
- Real-Time
- Voice
- Agents
---
