---
api_specs:
- filename: pyannoteai-api-openapi.yml
  format: yaml
  label: pyannoteAI API
  slug: pyannoteai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyannoteai/refs/heads/main/openapi/pyannoteai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pyannote.ai
  spf: true
hosts:
- cert_expires: Nov 13 17:03:03 2026 GMT
  host: pyannote.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 01:51:38 2026 GMT
  host: docs.pyannote.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:03:38 2026 GMT
  host: api.pyannote.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pyannoteai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PyannoteAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PyannoteAI
provider_slug: pyannoteai
slug: pyannoteai-domain-security
source_filename: pyannoteai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pyannote.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 17:03:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pyannote.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 01:51:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pyannote.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:03:38 2026 GMT\n  hsts: null\ndomains:\n- domain: pyannote.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyannoteai/refs/heads/main/security/pyannoteai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Speech Recognition
- Speaker Diarization
- Audio
- Voice AI
- Machine-Learning
- Transcription
- Streaming
- Webhook
---
