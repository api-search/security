---
api_specs:
- filename: reson8-openapi.yml
  format: yaml
  label: Reson8 Speech-to-Text API
  slug: reson8-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reson8/refs/heads/main/openapi/reson8-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reson8.dev
  spf: true
hosts:
- cert_expires: Sep 19 17:14:35 2026 GMT
  host: www.reson8.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:16:06 2026 GMT
  host: docs.reson8.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:16:06 2026 GMT
  host: api.reson8.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reson8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reson8, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reson8
provider_slug: reson8
slug: reson8-domain-security
source_filename: reson8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reson8.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:14:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.reson8.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:16:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reson8.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:16:06 2026 GMT\n  hsts: null\ndomains:\n- domain: reson8.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reson8/refs/heads/main/security/reson8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Speech Recognition
- Speech-to-Text
- ASR
- Voice AI
- Transcription
- Diarization
- Machine Learning
- Developers
---
