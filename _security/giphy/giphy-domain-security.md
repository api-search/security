---
api_specs:
- filename: giphy-openapi.yml
  format: yaml
  label: GIPHY API
  slug: giphy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/openapi/giphy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: giphy.com
  spf: true
hosts:
- cert_expires: Nov 10 22:03:15 2026 GMT
  host: giphy.com
  hsts: true
  hsts_max_age: 15465600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 22:03:15 2026 GMT
  host: developers.giphy.com
  hsts: true
  hsts_max_age: 15465600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 22:03:15 2026 GMT
  host: api.giphy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Giphy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giphy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Giphy
provider_slug: giphy
slug: giphy-domain-security
source_filename: giphy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: giphy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 22:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15465600\n- host: developers.giphy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 22:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15465600\n- host: api.giphy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 22:03:15 2026 GMT\n  hsts: null\ndomains:\n- domain: giphy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giphy/refs/heads/main/security/giphy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Photography
- Media
- GIFs
- Stickers
- Emoji
- Video
- Messaging
- Social
- Meta
---
