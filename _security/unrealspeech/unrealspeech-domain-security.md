---
api_specs:
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Speech API
  slug: unrealspeech-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Stream API
  slug: unrealspeech-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
- filename: unrealspeech-openapi.yml
  format: yaml
  label: Unreal Speech Synthesis Tasks API
  slug: unrealspeech-synthesis-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/openapi/unrealspeech-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unrealspeech.com
  spf: true
hosts:
- cert_expires: Oct  6 08:52:53 2026 GMT
  host: unrealspeech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 08:56:49 2026 GMT
  host: docs.unrealspeech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 10:40:03 2026 GMT
  host: api.v7.unrealspeech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unrealspeech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unreal Speech, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unreal Speech
provider_slug: unrealspeech
slug: unrealspeech-domain-security
source_filename: unrealspeech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unrealspeech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:52:53 2026 GMT\n  hsts: false\n- host: docs.unrealspeech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:56:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.v7.unrealspeech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 10:40:03 2026 GMT\n  hsts: null\ndomains:\n- domain: unrealspeech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrealspeech/refs/heads/main/security/unrealspeech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text to Speech
- TTS
- Speech Synthesis
- Audio
- Voice
- AI
---
