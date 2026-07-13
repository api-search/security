---
api_specs:
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Text-to-Speech API
  slug: text-to-speech
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Streaming TTS API
  slug: streaming-tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
- filename: speechify-openapi.yml
  format: yaml
  label: Speechify Voice Cloning API
  slug: voice-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/openapi/speechify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: speechify.com
  spf: true
hosts:
- cert_expires: Sep 28 08:05:07 2026 GMT
  host: speechify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 13:58:20 2026 GMT
  host: docs.sws.speechify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 01:07:07 2026 GMT
  host: api.sws.speechify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speechify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speechify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Speechify
provider_slug: speechify
slug: speechify-domain-security
source_filename: speechify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speechify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:05:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sws.speechify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.sws.speechify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 01:07:07 2026 GMT\n  hsts: null\ndomains:\n- domain: speechify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speechify/refs/heads/main/security/speechify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- Voice
- Speech Synthesis
- Voice Cloning
---
