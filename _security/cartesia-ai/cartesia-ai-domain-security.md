---
api_specs:
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Text-to-Speech API
  slug: cartesia-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-asyncapi.yml
  format: yaml
  label: Cartesia TTS WebSocket API
  slug: cartesia-ai-tts-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/asyncapi/cartesia-ai-asyncapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Speech-to-Text API
  slug: cartesia-ai-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-asyncapi.yml
  format: yaml
  label: Cartesia STT WebSocket API
  slug: cartesia-ai-stt-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/asyncapi/cartesia-ai-asyncapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voices API
  slug: cartesia-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voice Changer API
  slug: cartesia-ai-voice-changer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Infill API
  slug: cartesia-ai-infill-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Datasets API
  slug: cartesia-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Pronunciation Dictionaries API
  slug: cartesia-ai-pronunciation-dictionaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia API Keys and Auth API
  slug: cartesia-ai-api-keys-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Voice Agents API
  slug: cartesia-ai-voice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
- filename: cartesia-ai-openapi.yml
  format: yaml
  label: Cartesia Usage API
  slug: cartesia-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/openapi/cartesia-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
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
name: Cartesia Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cartesia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cartesia
provider_slug: cartesia-ai
slug: cartesia-ai-domain-security
source_filename: cartesia-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:07:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cartesia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cartesia.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartesia-ai/refs/heads/main/security/cartesia-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice AI
- Text to Speech
- Speech to Text
- Realtime
- WebSocket
- Voice Cloning
- Voice Agents
---
