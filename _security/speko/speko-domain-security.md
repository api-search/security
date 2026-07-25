---
api_specs:
- filename: speko-agents-api-openapi.yml
  format: yaml
  label: Speko Agents API
  slug: speko-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-agents-api-openapi.yml
- filename: speko-providers-api-openapi.yml
  format: yaml
  label: Speko Providers API
  slug: speko-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-providers-api-openapi.yml
- filename: speko-telephony-api-openapi.yml
  format: yaml
  label: Speko Telephony API
  slug: speko-telephony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-telephony-api-openapi.yml
- filename: speko-voice-api-openapi.yml
  format: yaml
  label: Speko Voice API
  slug: speko-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/openapi/speko-voice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: speko.dev
  spf: false
hosts:
- cert_expires: Oct 19 07:55:16 2026 GMT
  host: api.speko.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Speko
provider_slug: speko
slug: speko-domain-security
source_filename: speko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.speko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 07:55:16 2026 GMT\n  hsts: null\ndomains:\n- domain: speko.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speko/refs/heads/main/security/speko-domain-security.yml
summary_line: TLSv1.3
tags:
- Voice
- Voice AI
- Speech to Text
- Text to Speech
- LLM
- Telephony
- API Gateway
- Conversational AI
- Developer Tools
- AI Infrastructure
---
