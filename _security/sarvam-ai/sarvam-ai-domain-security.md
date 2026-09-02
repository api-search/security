---
api_specs:
- filename: sarvam-ai-chat-api-openapi.yml
  format: yaml
  label: Sarvam AI Chat API
  slug: sarvam-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-chat-api-openapi.yml
- filename: sarvam-ai-language-identification-api-openapi.yml
  format: yaml
  label: Sarvam AI Language Identification API
  slug: sarvam-ai-language-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-language-identification-api-openapi.yml
- filename: sarvam-ai-speech-to-text-api-openapi.yml
  format: yaml
  label: Sarvam AI Speech to Text API
  slug: sarvam-ai-speech-to-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-speech-to-text-api-openapi.yml
- filename: sarvam-ai-text-to-speech-api-openapi.yml
  format: yaml
  label: Sarvam AI Text to Speech API
  slug: sarvam-ai-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-text-to-speech-api-openapi.yml
- filename: sarvam-ai-translate-api-openapi.yml
  format: yaml
  label: Sarvam AI Translate API
  slug: sarvam-ai-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-translate-api-openapi.yml
- filename: sarvam-ai-transliterate-api-openapi.yml
  format: yaml
  label: Sarvam AI Transliterate API
  slug: sarvam-ai-transliterate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/openapi/sarvam-ai-transliterate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sarvam.ai
  spf: true
hosts:
- cert_expires: Oct  9 17:25:51 2026 GMT
  host: www.sarvam.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:41:47 2026 GMT
  host: docs.sarvam.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 12:46:21 2026 GMT
  host: api.sarvam.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sarvam Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sarvam AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sarvam AI
provider_slug: sarvam-ai
slug: sarvam-ai-domain-security
source_filename: sarvam-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sarvam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:25:51 2026 GMT\n  hsts: false\n- host: docs.sarvam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:41:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sarvam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:46:21 2026 GMT\n  hsts: null\ndomains:\n- domain: sarvam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarvam-ai/refs/heads/main/security/sarvam-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Speech-to-Text
- Text-to-Speech
- Translation
- Indian Languages
---
