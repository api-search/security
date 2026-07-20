---
api_specs:
- filename: hedra-web-api-openapi-original.json
  format: json
  label: Hedra Web API
  slug: hedra-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hedra/refs/heads/main/openapi/hedra-web-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hedra.com
  spf: true
hosts:
- cert_expires: Aug 20 07:31:05 2026 GMT
  host: www.hedra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.hedra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hedra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hedra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hedra
provider_slug: hedra
slug: hedra-domain-security
source_filename: hedra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hedra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hedra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hedra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedra/refs/heads/main/security/hedra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Image Generation
- Audio Generation
- Text to Speech
- Avatars
- Media
- Machine Learning
---
