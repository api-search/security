---
api_specs:
- filename: nabla-openapi.yml
  format: yaml
  label: Nabla Core API
  slug: nabla-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nabla/refs/heads/main/openapi/nabla-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nabla.com
  spf: true
hosts:
- cert_expires: Sep  2 20:50:07 2026 GMT
  host: www.nabla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 04:21:56 2026 GMT
  host: docs.nabla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:30:54 2026 GMT
  host: api.nabla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nabla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nabla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nabla
provider_slug: nabla
slug: nabla-domain-security
source_filename: nabla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nabla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:50:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nabla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:21:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nabla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:30:54 2026 GMT\n  hsts: null\ndomains:\n- domain: nabla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nabla/refs/heads/main/security/nabla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Ambient AI
- Clinical Documentation
- Medical Transcription
- Speech Recognition
- FHIR
- SOAP Notes
- Voice
- EHR Integration
---
