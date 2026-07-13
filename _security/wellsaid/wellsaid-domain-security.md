---
api_specs:
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Text-to-Speech API
  slug: wellsaid-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Streaming TTS API
  slug: wellsaid-streaming-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
- filename: wellsaid-openapi.yml
  format: yaml
  label: WellSaid Voices and Speakers API
  slug: wellsaid-voices-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/openapi/wellsaid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellsaidlabs.com
  spf: true
hosts:
- cert_expires: Aug 27 04:26:58 2026 GMT
  host: wellsaidlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:40:47 2026 GMT
  host: docs.wellsaidlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:22:14 2026 GMT
  host: api.wellsaidlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellsaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WellSaid Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WellSaid Labs
provider_slug: wellsaid
slug: wellsaid-domain-security
source_filename: wellsaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wellsaidlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 04:26:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wellsaidlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:40:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wellsaidlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:22:14 2026 GMT\n  hsts: null\ndomains:\n- domain: wellsaidlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellsaid/refs/heads/main/security/wellsaid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- Voice
- Audio
- TTS
---
