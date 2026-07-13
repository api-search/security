---
api_specs:
- filename: salad-transcription-api-openapi.yml
  format: yaml
  label: Salad Transcription API
  slug: salad-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salad-transcription-api/refs/heads/main/openapi/salad-transcription-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salad.com
  spf: true
hosts:
- cert_expires: Oct  5 16:34:15 2026 GMT
  host: salad.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salad Transcription Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salad Transcription API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salad Transcription API
provider_slug: salad-transcription-api
slug: salad-transcription-api-domain-security
source_filename: salad-transcription-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:34:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: salad.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salad-transcription-api/refs/heads/main/security/salad-transcription-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Audio Transcription
- Captions
- Diarization
- GPU
- Speech Recognition
- Transcription
- Video Processing
---
