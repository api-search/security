---
api_specs:
- filename: voiceitt-rest-api-openapi-original.json
  format: json
  label: Voiceitt HTTP API
  slug: voiceitt-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/openapi/voiceitt-rest-api-openapi-original.json
- filename: voiceitt-websockets-asyncapi.yml
  format: yaml
  label: Voiceitt WebSockets API
  slug: voiceitt-websockets-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/asyncapi/voiceitt-websockets-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voiceitt.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 10 04:43:57 2026 GMT
  host: voiceitt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: voiceitt-si-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api2.voiceitt.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voiceitt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voiceitt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voiceitt
provider_slug: voiceitt
slug: voiceitt-domain-security
source_filename: voiceitt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voiceitt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: voiceitt-si-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api2.voiceitt.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: voiceitt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceitt/refs/heads/main/security/voiceitt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Speech Recognition
- Speech-to-Text
- Voice
- Accessibility
- Assistive Technology
- Artificial Intelligence
- Transcription
- Captioning
- Company
---
