---
api_specs:
- filename: flux-image-generation-openapi.yml
  format: yaml
  label: Flux Image Generation API
  slug: flux-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/openapi/flux-image-generation-openapi.yml
- filename: flux-image-editing-openapi.yml
  format: yaml
  label: Flux Image Editing API
  slug: flux-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/openapi/flux-image-editing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bfl.ai
  spf: false
hosts:
- cert_expires: Sep 13 10:54:55 2026 GMT
  host: bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.bfl.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flux, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Flux
provider_slug: flux
slug: flux-domain-security
source_filename: flux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.bfl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bfl.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/security/flux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Image Generation
- Machine Learning
- Open Source
- Text to Image
---
