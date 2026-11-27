---
api_specs:
- filename: kurdishtts-com-stt-api-openapi.yml
  format: yaml
  label: Kurdish TTS STT API
  slug: kurdishtts-com-stt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-stt-api-openapi.yml
- filename: kurdishtts-com-tts-api-openapi.yml
  format: yaml
  label: Kurdish TTS TTS API
  slug: kurdishtts-com-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-tts-api-openapi.yml
- filename: kurdishtts-com-voices-api-openapi.yml
  format: yaml
  label: Kurdish TTS Voices API
  slug: kurdishtts-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kurdishtts-com/openapi/kurdishtts-com-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kurdishtts.com
  spf: true
hosts:
- cert_expires: Feb 10 02:54:36 2027 GMT
  host: kurdishtts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kurdish TTS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kurdish TTS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kurdish TTS
provider_slug: kurdishtts-com
slug: kurdishtts-com-domain-security
source_filename: kurdishtts-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kurdishtts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 02:54:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kurdishtts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kurdishtts-com/security/kurdishtts-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kurdish
- Text-to-Speech
- Speech-to-Text
- Voice Chat
- Artificial Intelligence
---
