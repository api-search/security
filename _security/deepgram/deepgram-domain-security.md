---
api_specs:
- filename: deepgram-voice-agent-asyncapi.yml
  format: yaml
  label: Deepgram Voice Agent API
  slug: voice-agent-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/asyncapi/deepgram-voice-agent-asyncapi.yml
- filename: deepgram-balances-api-openapi.yml
  format: yaml
  label: Deepgram Balances API
  slug: deepgram-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-balances-api-openapi.yml
- filename: deepgram-invitations-api-openapi.yml
  format: yaml
  label: Deepgram Invitations API
  slug: deepgram-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-invitations-api-openapi.yml
- filename: deepgram-keys-api-openapi.yml
  format: yaml
  label: Deepgram Keys API
  slug: deepgram-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-keys-api-openapi.yml
- filename: deepgram-members-api-openapi.yml
  format: yaml
  label: Deepgram Members API
  slug: deepgram-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-members-api-openapi.yml
- filename: deepgram-models-api-openapi.yml
  format: yaml
  label: Deepgram Models API
  slug: deepgram-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-models-api-openapi.yml
- filename: deepgram-pre-recorded-api-openapi.yml
  format: yaml
  label: Deepgram Pre-Recorded API
  slug: deepgram-pre-recorded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-pre-recorded-api-openapi.yml
- filename: deepgram-projects-api-openapi.yml
  format: yaml
  label: Deepgram Projects API
  slug: deepgram-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-projects-api-openapi.yml
- filename: deepgram-scopes-api-openapi.yml
  format: yaml
  label: Deepgram Scopes API
  slug: deepgram-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-scopes-api-openapi.yml
- filename: deepgram-text-intelligence-api-openapi.yml
  format: yaml
  label: Deepgram Text Intelligence API
  slug: deepgram-text-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-intelligence-api-openapi.yml
- filename: deepgram-text-to-speech-api-openapi.yml
  format: yaml
  label: Deepgram Text-To-Speech API
  slug: deepgram-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-text-to-speech-api-openapi.yml
- filename: deepgram-usage-api-openapi.yml
  format: yaml
  label: Deepgram Usage API
  slug: deepgram-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/openapi/deepgram-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepgram.com
  spf: true
hosts:
- cert_expires: Sep  5 06:43:52 2026 GMT
  host: deepgram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 20:02:28 2026 GMT
  host: developers.deepgram.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:52:49 2026 GMT
  host: api.deepgram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepgram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepgram, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deepgram
provider_slug: deepgram
slug: deepgram-domain-security
source_filename: deepgram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.deepgram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:52:49 2026 GMT\n  hsts: null\ndomains:\n- domain: deepgram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepgram/refs/heads/main/security/deepgram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Speech-To-Text
- Text-To-Speech
- Transcription
- Voice AI
---
