---
api_specs:
- filename: retell-agent-api-openapi.yml
  format: yaml
  label: Retell AI Agent API
  slug: retell-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-agent-api-openapi.yml
- filename: retell-batch-call-api-openapi.yml
  format: yaml
  label: Retell AI Batch Call API
  slug: retell-batch-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-batch-call-api-openapi.yml
- filename: retell-call-api-openapi.yml
  format: yaml
  label: Retell AI Call API
  slug: retell-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-call-api-openapi.yml
- filename: retell-concurrency-api-openapi.yml
  format: yaml
  label: Retell AI Concurrency API
  slug: retell-concurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-concurrency-api-openapi.yml
- filename: retell-conversation-flow-api-openapi.yml
  format: yaml
  label: Retell AI Conversation Flow API
  slug: retell-conversation-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-conversation-flow-api-openapi.yml
- filename: retell-knowledge-base-api-openapi.yml
  format: yaml
  label: Retell AI Knowledge Base API
  slug: retell-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-knowledge-base-api-openapi.yml
- filename: retell-phone-call-api-openapi.yml
  format: yaml
  label: Retell AI Phone Call API
  slug: retell-phone-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-phone-call-api-openapi.yml
- filename: retell-phone-number-api-openapi.yml
  format: yaml
  label: Retell AI Phone Number API
  slug: retell-phone-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-phone-number-api-openapi.yml
- filename: retell-retell-llm-api-openapi.yml
  format: yaml
  label: Retell AI Retell LLM API
  slug: retell-retell-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-retell-llm-api-openapi.yml
- filename: retell-voice-api-openapi.yml
  format: yaml
  label: Retell AI Voice API
  slug: retell-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-voice-api-openapi.yml
- filename: retell-web-call-api-openapi.yml
  format: yaml
  label: Retell AI Web Call API
  slug: retell-web-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/openapi/retell-web-call-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: retellai.com
  spf: true
hosts:
- cert_expires: Sep 28 05:15:21 2026 GMT
  host: www.retellai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:59:11 2026 GMT
  host: docs.retellai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.retellai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retell AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Retell AI
provider_slug: retell
slug: retell-domain-security
source_filename: retell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.retellai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:15:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.retellai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:59:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.retellai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: retellai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retell/refs/heads/main/security/retell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- Voice Agents
- Conversational AI
- Telephony
---
