---
api_specs:
- filename: fish-audio-model-api-openapi.yml
  format: yaml
  label: Fish Audio Model API
  slug: fish-audio-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-model-api-openapi.yml
- filename: fish-audio-wallet-api-openapi.yml
  format: yaml
  label: Fish Audio Wallet API
  slug: fish-audio-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-wallet-api-openapi.yml
- filename: fish-audio-agent-sessions-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Sessions API
  slug: fish-audio-agent-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-sessions-api-openapi.yml
- filename: fish-audio-agent-tests-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Tests API
  slug: fish-audio-agent-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-tests-api-openapi.yml
- filename: fish-audio-agent-tools-api-openapi.yml
  format: yaml
  label: Fish Audio Agent Tools API
  slug: fish-audio-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agent-tools-api-openapi.yml
- filename: fish-audio-agents-api-openapi.yml
  format: yaml
  label: Fish Audio Agents API
  slug: fish-audio-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-agents-api-openapi.yml
- filename: fish-audio-knowledge-sources-api-openapi.yml
  format: yaml
  label: Fish Audio Knowledge Sources API
  slug: fish-audio-knowledge-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-knowledge-sources-api-openapi.yml
- filename: fish-audio-openapi-v1-api-openapi.yml
  format: yaml
  label: Fish Audio OpenAPI v1 API
  slug: fish-audio-openapi-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-openapi-v1-api-openapi.yml
- filename: fish-audio-phone-calls-api-openapi.yml
  format: yaml
  label: Fish Audio Phone Calls API
  slug: fish-audio-phone-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-phone-calls-api-openapi.yml
- filename: fish-audio-phone-numbers-api-openapi.yml
  format: yaml
  label: Fish Audio Phone Numbers API
  slug: fish-audio-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fish-audio/openapi/fish-audio-phone-numbers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fish.audio
  spf: true
hosts:
- cert_expires: Oct  3 11:43:07 2026 GMT
  host: fish.audio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:35:32 2026 GMT
  host: docs.fish.audio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:46:37 2026 GMT
  host: api.fish.audio
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fish Audio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fish Audio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fish Audio
provider_slug: fish-audio
slug: fish-audio-domain-security
source_filename: fish-audio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:35:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fish.audio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:46:37 2026 GMT\n  hsts: null\ndomains:\n- domain: fish.audio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fish-audio/security/fish-audio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice
- Text-to-Speech
- Speech-to-Text
- Voice Cloning
- Audio
- Generative AI
- Multilingual
- Streaming
- SDK
- Open Source
---
