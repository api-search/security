---
api_specs:
- filename: hume-ai-voices-openapi.yml
  format: yaml
  label: Hume Voices API
  slug: voices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-voices-openapi.yml
- filename: hume-ai-tts-openapi.yml
  format: yaml
  label: Hume Octave Text-to-Speech API
  slug: tts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-tts-openapi.yml
- filename: hume-ai-evi-openapi.yml
  format: yaml
  label: Hume Empathic Voice Interface (EVI) API
  slug: evi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-evi-openapi.yml
- filename: hume-ai-expression-openapi.yml
  format: yaml
  label: Hume Expression Measurement API
  slug: expression
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/openapi/hume-ai-expression-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hume.ai
  spf: true
hosts:
- cert_expires: Aug  9 15:41:55 2026 GMT
  host: www.hume.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:36:52 2026 GMT
  host: dev.hume.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 18:43:43 2026 GMT
  host: api.hume.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hume Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hume AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hume AI
provider_slug: hume-ai
slug: hume-ai-domain-security
source_filename: hume-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 15:41:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hume.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:43:43 2026 GMT\n  hsts: null\ndomains:\n- domain: hume.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hume-ai/refs/heads/main/security/hume-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- Empathic
- Emotion
- Multimodal
---
