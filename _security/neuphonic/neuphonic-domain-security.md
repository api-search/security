---
api_specs:
- filename: sse
  format: yaml
  label: Neuphonic TTS SSE API
  slug: neuphonic-tts-sse-api
  spec_type: OpenAPI
  url: https://docs.neuphonic.com/api-reference/tts/sse
- filename: websocket
  format: yaml
  label: Neuphonic TTS WebSocket API
  slug: neuphonic-tts-websocket-api
  spec_type: AsyncAPI
  url: https://docs.neuphonic.com/api-reference/tts/websocket
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neuphonic.com
  spf: false
hosts:
- cert_expires: Sep 11 12:53:30 2026 GMT
  host: www.neuphonic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 22:01:20 2026 GMT
  host: docs.neuphonic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:32:27 2026 GMT
  host: api.neuphonic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuphonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neuphonic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Neuphonic
provider_slug: neuphonic
slug: neuphonic-domain-security
source_filename: neuphonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neuphonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.neuphonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:01:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.neuphonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:32:27 2026 GMT\n  hsts: null\ndomains:\n- domain: neuphonic.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuphonic/refs/heads/main/security/neuphonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Text-to-Speech
- Voice AI
- Audio
- Streaming
- WebSocket
- Voice Cloning
- Conversational AI
- Real-Time
- Multilingual
- On-Device AI
---
