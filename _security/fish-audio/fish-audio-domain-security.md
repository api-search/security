---
api_specs:
- filename: fish-audio-openapi.yml
  format: yaml
  label: Fish Audio API
  slug: fish-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/openapi/fish-audio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fish.audio
  spf: true
hosts:
- cert_expires: Oct  3 11:43:07 2026 GMT
  host: fish.audio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:35:32 2026 GMT
  host: docs.fish.audio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:46:37 2026 GMT
  host: api.fish.audio
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fish Audio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fish Audio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fish Audio
provider_slug: fish-audio
slug: fish-audio-domain-security
source_filename: fish-audio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:46:37 2026 GMT\n  hsts: null\ndomains:\n- domain: fish.audio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fish-audio/refs/heads/main/security/fish-audio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- Text to Speech
- Speech to Text
- Voice Cloning
- Audio
- Generative AI
- Multilingual
- Streaming
- SDK
- Open Source
---
