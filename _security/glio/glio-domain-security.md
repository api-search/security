---
api_specs:
- filename: glio-openapi-original.json
  format: json
  label: Glio API
  slug: glio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glio/refs/heads/main/openapi/glio-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glio.io
  spf: true
hosts:
- cert_expires: Oct  8 14:14:06 2026 GMT
  host: glio.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  8 14:14:06 2026 GMT
  host: api.glio.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Glio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Glio
provider_slug: glio
slug: glio-domain-security
source_filename: glio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glio.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 14:14:06 2026 GMT\n  hsts: false\n- host: api.glio.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 14:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glio/refs/heads/main/security/glio-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- AI
- Machine Learning
- Media Generation
- Video Generation
- Image Generation
- Audio Generation
- Text to Speech
- Large Language Models
- Generative AI
- API Aggregator
- Developer Tools
---
