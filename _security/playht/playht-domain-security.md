---
api_specs:
- filename: playht-asyncapi.yml
  format: yaml
  label: PlayAI Text-to-Speech API
  slug: tts-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/asyncapi/playht-asyncapi.yml
- filename: playht-asyncapi.yml
  format: yaml
  label: PlayAI Voice Agents API
  slug: agents-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/asyncapi/playht-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: play.ht
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: play.ai
  spf: true
hosts:
- host: play.ht
  https: false
- cert_expires: Jul 27 09:44:06 2026 GMT
  host: docs.play.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.play.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Playht Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlayHT, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PlayHT
provider_slug: playht
slug: playht-domain-security
source_filename: playht-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: play.ht\n  https: false\n- host: docs.play.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 09:44:06 2026 GMT\n  hsts: null\n- host: api.play.ai\n  https: false\ndomains:\n- domain: play.ht\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: play.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playht/refs/heads/main/security/playht-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Voice
- TTS
- Text to Speech
- Voice Cloning
- Voice Agents
- Streaming
- PlayDialog
- Play 3.0
- PlayNote
- Multilingual
- Real-Time
---
