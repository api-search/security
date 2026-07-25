---
api_specs:
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Sonic Text-to-Speech API
  slug: tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-asyncapi.yml
  format: yaml
  label: Cartesia Ink Speech-to-Text API
  slug: stt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/asyncapi/cartesia-asyncapi.yml
- filename: cartesia-auth-api-openapi.yml
  format: yaml
  label: Cartesia Auth API
  slug: cartesia-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-auth-api-openapi.yml
- filename: cartesia-stt-api-openapi.yml
  format: yaml
  label: Cartesia STT API
  slug: cartesia-stt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-stt-api-openapi.yml
- filename: cartesia-tts-api-openapi.yml
  format: yaml
  label: Cartesia TTS API
  slug: cartesia-tts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-tts-api-openapi.yml
- filename: cartesia-voices-api-openapi.yml
  format: yaml
  label: Cartesia Voices API
  slug: cartesia-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/openapi/cartesia-voices-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cartesia.ai
  spf: true
hosts:
- cert_expires: Sep 18 22:07:57 2026 GMT
  host: cartesia.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 22:07:57 2026 GMT
  host: docs.cartesia.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.cartesia.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cartesia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartesia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cartesia
provider_slug: cartesia
slug: cartesia-domain-security
source_filename: cartesia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cartesia.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesia/refs/heads/main/security/cartesia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- TTS
- Text to Speech
- STT
- Speech to Text
- Streaming
- WebSocket
- Voice Agents
- Voice Clone
- Sonic
- Ink
- Real-Time
---
