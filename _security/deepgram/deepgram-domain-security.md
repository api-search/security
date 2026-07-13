---
api_specs:
- filename: deepgram-speech-to-text-openapi.yml
  format: yaml
  label: Deepgram Speech-To-Text API
  slug: speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-speech-to-text-openapi.yml
- filename: deepgram-text-to-speech-openapi.yml
  format: yaml
  label: Deepgram Text-To-Speech API
  slug: text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-to-speech-openapi.yml
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-speech-to-text-openapi.yml
  format: yaml
  label: Deepgram Audio Intelligence API
  slug: audio-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-speech-to-text-openapi.yml
- filename: deepgram-management-openapi.yml
  format: yaml
  label: Deepgram Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepgram.com
  spf: true
hosts:
- cert_expires: Sep  5 06:43:52 2026 GMT
  host: deepgram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:02:28 2026 GMT
  host: developers.deepgram.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:52:49 2026 GMT
  host: api.deepgram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepgram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepgram, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deepgram
provider_slug: deepgram
slug: deepgram-domain-security
source_filename: deepgram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:52:49 2026 GMT\n  hsts: null\ndomains:\n- domain: deepgram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/security/deepgram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Speech-To-Text
- Text-To-Speech
- Transcription
- Voice AI
---
