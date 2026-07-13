---
api_specs:
- filename: d-id-videos-openapi.yml
  format: yaml
  label: D-ID Videos API
  slug: d-id-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/openapi/d-id-videos-openapi.yml
- filename: d-id-agents-openapi.yml
  format: yaml
  label: D-ID Agents API
  slug: d-id-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/openapi/d-id-agents-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: d-id.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.d-id.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:46:30 2026 GMT
  host: docs.d-id.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.d-id.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D-ID, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: D-ID
provider_slug: d-id
slug: d-id-domain-security
source_filename: d-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d-id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.d-id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:46:30 2026 GMT\n  hsts: null\n- host: api.d-id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: d-id.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-id/refs/heads/main/security/d-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Video
- Digital Humans
- Talking Head
- Avatar
- Generative AI
- Video Generation
- Real-Time Streaming
- Text to Video
- Video Translation
- Voice Cloning
---
