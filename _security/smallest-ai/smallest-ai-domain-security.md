---
api_specs:
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Text-to-Speech (Waves)
  slug: text-to-speech-waves
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Streaming / Realtime TTS
  slug: streaming-realtime-tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
- filename: smallest-ai-openapi.yml
  format: yaml
  label: Smallest AI Voices / Cloning
  slug: voices-cloning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/openapi/smallest-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smallest.ai
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: smallest.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:53:39 2026 GMT
  host: docs.smallest.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: waves-api.smallest.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Smallest Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smallest AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smallest AI
provider_slug: smallest-ai
slug: smallest-ai-domain-security
source_filename: smallest-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smallest.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.smallest.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:53:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: waves-api.smallest.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: smallest.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/security/smallest-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- Voice
- Realtime
- Voice Agents
---
