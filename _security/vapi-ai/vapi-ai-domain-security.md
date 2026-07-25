---
api_specs:
- filename: vapi-ai-analytics-api-openapi.yml
  format: yaml
  label: Vapi Analytics API
  slug: vapi-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-analytics-api-openapi.yml
- filename: vapi-ai-assistants-api-openapi.yml
  format: yaml
  label: Vapi Assistants API
  slug: vapi-ai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-assistants-api-openapi.yml
- filename: vapi-ai-calls-api-openapi.yml
  format: yaml
  label: Vapi Calls API
  slug: vapi-ai-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-calls-api-openapi.yml
- filename: vapi-ai-campaigns-api-openapi.yml
  format: yaml
  label: Vapi Campaigns API
  slug: vapi-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-campaigns-api-openapi.yml
- filename: vapi-ai-chats-api-openapi.yml
  format: yaml
  label: Vapi Chats API
  slug: vapi-ai-chats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-chats-api-openapi.yml
- filename: vapi-ai-eval-api-openapi.yml
  format: yaml
  label: Vapi Eval API
  slug: vapi-ai-eval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-eval-api-openapi.yml
- filename: vapi-ai-files-api-openapi.yml
  format: yaml
  label: Vapi Files API
  slug: vapi-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-files-api-openapi.yml
- filename: vapi-ai-insight-api-openapi.yml
  format: yaml
  label: Vapi Insight API
  slug: vapi-ai-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-insight-api-openapi.yml
- filename: vapi-ai-observability-scorecard-api-openapi.yml
  format: yaml
  label: Vapi Observability/Scorecard API
  slug: vapi-ai-observability-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-observability-scorecard-api-openapi.yml
- filename: vapi-ai-phone-numbers-api-openapi.yml
  format: yaml
  label: Vapi Phone Numbers API
  slug: vapi-ai-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-phone-numbers-api-openapi.yml
- filename: vapi-ai-provider-resources-api-openapi.yml
  format: yaml
  label: Vapi Provider Resources API
  slug: vapi-ai-provider-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-provider-resources-api-openapi.yml
- filename: vapi-ai-sessions-api-openapi.yml
  format: yaml
  label: Vapi Sessions API
  slug: vapi-ai-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-sessions-api-openapi.yml
- filename: vapi-ai-squads-api-openapi.yml
  format: yaml
  label: Vapi Squads API
  slug: vapi-ai-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-squads-api-openapi.yml
- filename: vapi-ai-structured-outputs-api-openapi.yml
  format: yaml
  label: Vapi Structured Outputs API
  slug: vapi-ai-structured-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-structured-outputs-api-openapi.yml
- filename: vapi-ai-tools-api-openapi.yml
  format: yaml
  label: Vapi Tools API
  slug: vapi-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vapi-ai/refs/heads/main/openapi/vapi-ai-tools-api-openapi.yml
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
