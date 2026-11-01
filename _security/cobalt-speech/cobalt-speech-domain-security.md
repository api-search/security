---
api_specs:
- filename: cobalt-speech-openapi-generated.yml
  format: yaml
  label: Cobalt Speech API
  slug: cobalt-speech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cobalt-speech/openapi/_ae-authored/cobalt-speech-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cobaltspeech.com
  spf: false
hosts:
- cert_expires: Jan 13 19:22:31 2027 GMT
  host: cobaltspeech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobalt Speech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobalt Speech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cobalt Speech
provider_slug: cobalt-speech
slug: cobalt-speech-domain-security
source_filename: cobalt-speech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cobaltspeech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:22:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cobaltspeech.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cobalt-speech/security/cobalt-speech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Speech
- AI
- Transcription
- Voice
---
