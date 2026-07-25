---
api_specs:
- filename: shotstack-create-api-openapi.yml
  format: yaml
  label: Shotstack Create API
  slug: shotstack-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-create-api-openapi.yml
- filename: shotstack-edit-api-openapi.yml
  format: yaml
  label: Shotstack Edit API
  slug: shotstack-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-edit-api-openapi.yml
- filename: shotstack-ingest-api-openapi.yml
  format: yaml
  label: Shotstack Ingest API
  slug: shotstack-ingest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-ingest-api-openapi.yml
- filename: shotstack-serve-api-openapi.yml
  format: yaml
  label: Shotstack Serve API
  slug: shotstack-serve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-serve-api-openapi.yml
- filename: shotstack-templates-api-openapi.yml
  format: yaml
  label: Shotstack Templates API
  slug: shotstack-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/openapi/shotstack-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shotstack.io
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: shotstack.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: api.shotstack.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shotstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shotstack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shotstack
provider_slug: shotstack
slug: shotstack-domain-security
source_filename: shotstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shotstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: api.shotstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shotstack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/security/shotstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Video Editing
- Media
- Rendering
- Generative AI
---
