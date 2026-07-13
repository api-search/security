---
api_specs:
- filename: uberduck-openapi.yml
  format: yaml
  label: Uberduck Text-to-Speech API
  slug: uberduck-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-openapi.yml
- filename: uberduck-openapi.yml
  format: yaml
  label: Uberduck Voices API
  slug: uberduck-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-openapi.yml
- filename: uberduck-openapi.yml
  format: yaml
  label: Uberduck Models API
  slug: uberduck-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-openapi.yml
- filename: uberduck-openapi.yml
  format: yaml
  label: Uberduck Conversational Voice API
  slug: uberduck-conversational-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/openapi/uberduck-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uberduck.ai
  spf: true
hosts:
- cert_expires: Sep 30 19:24:57 2026 GMT
  host: uberduck.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 12:17:30 2026 GMT
  host: docs.uberduck.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 19:24:57 2026 GMT
  host: api.uberduck.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uberduck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uberduck, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Uberduck
provider_slug: uberduck
slug: uberduck-domain-security
source_filename: uberduck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uberduck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.uberduck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 12:17:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.uberduck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:24:57 2026 GMT\n  hsts: null\ndomains:\n- domain: uberduck.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uberduck/refs/heads/main/security/uberduck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- TTS
- Voice
- Voice Cloning
- Speech Synthesis
- Conversational AI
---
