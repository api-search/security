---
api_specs:
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Text-to-Speech API
  slug: camb-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Dubbing API
  slug: camb-ai-dubbing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Translation API
  slug: camb-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Voices API
  slug: camb-ai-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
- filename: camb-ai-openapi.yml
  format: yaml
  label: Camb.AI Transcription API
  slug: camb-ai-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/openapi/camb-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: camb.ai
  spf: true
hosts:
- cert_expires: Aug 13 00:01:46 2026 GMT
  host: www.camb.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 01:49:34 2026 GMT
  host: docs.camb.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 14:51:49 2026 GMT
  host: client.camb.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camb Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camb.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Camb.AI
provider_slug: camb-ai
slug: camb-ai-domain-security
source_filename: camb-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.camb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:01:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.camb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 01:49:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: client.camb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:51:49 2026 GMT\n  hsts: null\ndomains:\n- domain: camb.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camb-ai/refs/heads/main/security/camb-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Text to Speech
- Dubbing
- Translation
- Transcription
- Voice Cloning
- Speech
---
