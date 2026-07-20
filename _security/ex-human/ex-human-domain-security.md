---
api_specs:
- filename: ex-human-openapi.yml
  format: yaml
  label: Ex-Human API
  slug: ex-human-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/openapi/ex-human-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exh.ai
  spf: true
hosts:
- cert_expires: Oct  3 18:59:07 2026 GMT
  host: docs.exh.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:54 2026 GMT
  host: api.exh.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ex Human Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ex-Human, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ex-Human
provider_slug: ex-human
slug: ex-human-domain-security
source_filename: ex-human-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.exh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:59:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.exh.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 23:59:54 2026 GMT\n  hsts: false\ndomains:\n- domain: exh.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ex-human/refs/heads/main/security/ex-human-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- AI Companions
- Generative AI
- Text to Speech
- Image Generation
- Video Generation
- Avatars
- Multimodal
---
