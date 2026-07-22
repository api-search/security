---
api_specs:
- filename: slng-stt-slng-openapi.yml
  format: yaml
  label: SLNG Gateway API
  slug: slng-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-stt-slng-openapi.yml
- filename: slng-agents-openapi.yml
  format: yaml
  label: SLNG Voice Agents API
  slug: slng-voice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-agents-openapi.yml
- filename: slng-batch-openapi.json
  format: json
  label: SLNG Batch API
  slug: slng-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/openapi/slng-batch-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: slng.ai
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: api.agents.slng.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: api.batch.slng.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: stageapi.batch.slng.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SLNG, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SLNG
provider_slug: slng
slug: slng-domain-security
source_filename: slng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.agents.slng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\n- host: api.batch.slng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\n- host: stageapi.batch.slng.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: slng.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slng/refs/heads/main/security/slng-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Speech
- Voice
- Speech to Text
- Text to Speech
- Voice AI
- Voice Agents
- Transcription
- Speech Recognition
- Artificial Intelligence
- API Gateway
---
