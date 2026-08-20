---
api_specs:
- filename: sambanova-systems-audio-api-openapi.yml
  format: yaml
  label: SambaNova Systems Audio API
  slug: sambanova-systems-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-audio-api-openapi.yml
- filename: sambanova-systems-chat-completions-api-openapi.yml
  format: yaml
  label: SambaNova Systems Chat completions API
  slug: sambanova-systems-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-chat-completions-api-openapi.yml
- filename: sambanova-systems-completions-api-openapi.yml
  format: yaml
  label: SambaNova Systems Completions API
  slug: sambanova-systems-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-completions-api-openapi.yml
- filename: sambanova-systems-embeddings-api-openapi.yml
  format: yaml
  label: SambaNova Systems Embeddings API
  slug: sambanova-systems-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-embeddings-api-openapi.yml
- filename: sambanova-systems-file-management-api-openapi.yml
  format: yaml
  label: SambaNova Systems File Management API
  slug: sambanova-systems-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-file-management-api-openapi.yml
- filename: sambanova-systems-main-agent-api-openapi.yml
  format: yaml
  label: SambaNova Systems Main Agent API
  slug: sambanova-systems-main-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-main-agent-api-openapi.yml
- filename: sambanova-systems-main-agent-interactive-api-openapi.yml
  format: yaml
  label: SambaNova Systems Main Agent Interactive API
  slug: sambanova-systems-main-agent-interactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-main-agent-interactive-api-openapi.yml
- filename: sambanova-systems-messages-api-openapi.yml
  format: yaml
  label: SambaNova Systems Messages API
  slug: sambanova-systems-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-messages-api-openapi.yml
- filename: sambanova-systems-models-api-openapi.yml
  format: yaml
  label: SambaNova Systems Models API
  slug: sambanova-systems-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-models-api-openapi.yml
- filename: sambanova-systems-responses-api-openapi.yml
  format: yaml
  label: SambaNova Systems Responses API
  slug: sambanova-systems-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-responses-api-openapi.yml
- filename: sambanova-systems-subagents-api-openapi.yml
  format: yaml
  label: SambaNova Systems Subagents API
  slug: sambanova-systems-subagents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-subagents-api-openapi.yml
- filename: sambanova-systems-subagents-interactive-api-openapi.yml
  format: yaml
  label: SambaNova Systems Subagents Interactive API
  slug: sambanova-systems-subagents-interactive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/openapi/sambanova-systems-subagents-interactive-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sambanovasystems.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sambanova.ai
  spf: true
hosts:
- cert_expires: Oct 17 21:40:44 2026 GMT
  host: sambanovasystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 22:47:18 2026 GMT
  host: chat.sambanova.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:04:00 2027 GMT
  host: api.sambanova.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sambanova Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SambaNova Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SambaNova Systems
provider_slug: sambanova-systems
slug: sambanova-systems-domain-security
source_filename: sambanova-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sambanovasystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:40:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chat.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 22:47:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sambanova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:04:00 2027 GMT\n  hsts: null\ndomains:\n- domain: sambanovasystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sambanova.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sambanova-systems/refs/heads/main/security/sambanova-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- LLM
- Inference
- Generative AI
- Agents
- Embeddings
---
