---
api_specs:
- filename: kotoba-transcription-openapi-original.yml
  format: yaml
  label: Kotoba Transcription API (Batch REST)
  slug: kotoba-transcription-api-batch-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-transcription-openapi-original.yml
- filename: kotoba-asr-realtime-openapi-original.yml
  format: yaml
  label: Kotoba ASR Realtime API (WebSocket)
  slug: kotoba-asr-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-asr-realtime-openapi-original.yml
- filename: kotoba-sts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba Speech-to-Speech Translation API (WebSocket)
  slug: kotoba-speech-to-speech-translation-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-sts-realtime-openapi-original.yml
- filename: kotoba-tts-realtime-openapi-original.yml
  format: yaml
  label: Kotoba TTS Realtime API (WebSocket)
  slug: kotoba-tts-realtime-api-websocket
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/openapi/kotoba-tts-realtime-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kotoba.tech
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kotobatech.ai
  spf: false
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: kotoba.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.kotobatech.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kotoba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kotoba, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kotoba
provider_slug: kotoba
slug: kotoba-domain-security
source_filename: kotoba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kotoba.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kotobatech.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kotoba.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: kotobatech.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotoba/refs/heads/main/security/kotoba-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Voice
- Speech Recognition
- Speech to Text
- Text to Speech
- Translation
- Real Time
- WebSockets
- Audio
- Transcription
---
