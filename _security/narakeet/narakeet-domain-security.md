---
api_specs:
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Text to Speech API
  slug: narakeet-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Markdown to Video API
  slug: narakeet-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Voice Listing API
  slug: narakeet-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
- filename: narakeet-openapi.yml
  format: yaml
  label: Narakeet Account Credits API
  slug: narakeet-account-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/openapi/narakeet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: narakeet.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.narakeet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: api.narakeet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Narakeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Narakeet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Narakeet
provider_slug: narakeet
slug: narakeet-domain-security
source_filename: narakeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.narakeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.narakeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: narakeet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narakeet/refs/heads/main/security/narakeet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text to Speech
- TTS
- Voice
- Audio
- Video
- AI
- Media Generation
---
