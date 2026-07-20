---
api_specs:
- filename: anamai-openapi-original.json
  format: json
  label: Anam AI API
  slug: anam-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/openapi/anamai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anam.ai
  spf: true
hosts:
- cert_expires: Sep 16 11:59:26 2026 GMT
  host: anam.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 12:55:42 2026 GMT
  host: api.anam.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anamai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anam.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anam.ai
provider_slug: anamai
slug: anamai-domain-security
source_filename: anamai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.anam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:55:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anamai/refs/heads/main/security/anamai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Avatars
- Conversational AI
- Real-Time Video
- WebRTC
- Digital Humans
- Generative AI
---
