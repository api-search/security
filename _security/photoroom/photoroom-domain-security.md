---
api_specs:
- filename: photoroom-openapi.yml
  format: yaml
  label: Photoroom API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/openapi/photoroom-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: photoroom.com
  spf: true
hosts:
- cert_expires: Oct  9 06:24:40 2026 GMT
  host: www.photoroom.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:24:41 2026 GMT
  host: docs.photoroom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 06:24:40 2026 GMT
  host: image-api.photoroom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Photoroom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photoroom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Photoroom
provider_slug: photoroom
slug: photoroom-domain-security
source_filename: photoroom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.photoroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:24:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.photoroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:24:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: image-api.photoroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 06:24:40 2026 GMT\n  hsts: null\ndomains:\n- domain: photoroom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photoroom/refs/heads/main/security/photoroom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Image Editing
- Background Removal
- E-commerce
- Visual
---
