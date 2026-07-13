---
api_specs:
- filename: heygen-openapi.yml
  format: yaml
  label: HeyGen API
  slug: heygen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/openapi/heygen-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heygen.com
  spf: true
hosts:
- cert_expires: Sep 12 15:00:09 2026 GMT
  host: www.heygen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:34:54 2026 GMT
  host: developers.heygen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.heygen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heygen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyGen, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HeyGen
provider_slug: heygen
slug: heygen-domain-security
source_filename: heygen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heygen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.heygen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:34:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.heygen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: heygen.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heygen/refs/heads/main/security/heygen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Generative AI
- Video
- Avatars
- Voice Cloning
- Text To Speech
- Lipsync
- Translation
- Streaming
- MCP
---
