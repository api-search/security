---
api_specs:
- filename: vapi-assistants-api-openapi.yml
  format: yaml
  label: Vapi Assistants API
  slug: vapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-assistants-api-openapi.yml
- filename: vapi-calls-api-openapi.yml
  format: yaml
  label: Vapi Calls API
  slug: vapi-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-calls-api-openapi.yml
- filename: vapi-phone-numbers-api-openapi.yml
  format: yaml
  label: Vapi Phone Numbers API
  slug: vapi-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-phone-numbers-api-openapi.yml
- filename: vapi-squads-api-openapi.yml
  format: yaml
  label: Vapi Squads API
  slug: vapi-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-squads-api-openapi.yml
- filename: vapi-tools-api-openapi.yml
  format: yaml
  label: Vapi Tools API
  slug: vapi-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-tools-api-openapi.yml
- filename: vapi-files-api-openapi.yml
  format: yaml
  label: Vapi Files API
  slug: vapi-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-files-api-openapi.yml
- filename: vapi-chats-api-openapi.yml
  format: yaml
  label: Vapi Chats API
  slug: vapi-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-chats-api-openapi.yml
- filename: vapi-sessions-api-openapi.yml
  format: yaml
  label: Vapi Sessions API
  slug: vapi-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-sessions-api-openapi.yml
- filename: vapi-campaigns-api-openapi.yml
  format: yaml
  label: Vapi Campaigns API
  slug: vapi-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-campaigns-api-openapi.yml
- filename: vapi-analytics-api-openapi.yml
  format: yaml
  label: Vapi Analytics API
  slug: vapi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-analytics-api-openapi.yml
- filename: vapi-insight-api-openapi.yml
  format: yaml
  label: Vapi Insight API
  slug: vapi-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-insight-api-openapi.yml
- filename: vapi-observability-api-openapi.yml
  format: yaml
  label: Vapi Observability Scorecard API
  slug: vapi-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-observability-api-openapi.yml
- filename: vapi-eval-api-openapi.yml
  format: yaml
  label: Vapi Eval API
  slug: vapi-eval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-eval-api-openapi.yml
- filename: vapi-structured-outputs-api-openapi.yml
  format: yaml
  label: Vapi Structured Outputs API
  slug: vapi-structured-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-structured-outputs-api-openapi.yml
- filename: vapi-provider-resources-api-openapi.yml
  format: yaml
  label: Vapi Provider Resources API
  slug: vapi-provider-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-provider-resources-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vapi.ai
  spf: true
hosts:
- cert_expires: Sep 30 05:31:31 2026 GMT
  host: vapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:20:51 2026 GMT
  host: docs.vapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:52:46 2026 GMT
  host: api.vapi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vapi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vapi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vapi
provider_slug: vapi-ai
slug: vapi-ai-domain-security
source_filename: vapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:52:46 2026 GMT\n  hsts: false\ndomains:\n- domain: vapi.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/security/vapi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Voice AI
- Voice Agents
- Conversational AI
- Telephony
- Real-Time
- Transcription
- Text-to-Speech
- LLM
- Agents
- MCP
---
