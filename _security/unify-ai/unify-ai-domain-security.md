---
api_specs:
- filename: unify-ai-agent-api-openapi.yml
  format: yaml
  label: Unify Agent API
  slug: unify-ai-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-agent-api-openapi.yml
- filename: unify-ai-assistants-api-openapi.yml
  format: yaml
  label: Unify Assistants API
  slug: unify-ai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-assistants-api-openapi.yml
- filename: unify-ai-contexts-api-openapi.yml
  format: yaml
  label: Unify Contexts API
  slug: unify-ai-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-contexts-api-openapi.yml
- filename: unify-ai-logs-api-openapi.yml
  format: yaml
  label: Unify Logs API
  slug: unify-ai-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-logs-api-openapi.yml
- filename: unify-ai-organizations-api-openapi.yml
  format: yaml
  label: Unify Organizations API
  slug: unify-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-organizations-api-openapi.yml
- filename: unify-ai-platform-api-openapi.yml
  format: yaml
  label: Unify Platform API
  slug: unify-ai-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-platform-api-openapi.yml
- filename: unify-ai-projects-api-openapi.yml
  format: yaml
  label: Unify Projects API
  slug: unify-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-projects-api-openapi.yml
- filename: unify-ai-spaces-api-openapi.yml
  format: yaml
  label: Unify Spaces API
  slug: unify-ai-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/openapi/unify-ai-spaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unify.ai
  spf: true
hosts:
- cert_expires: Sep 14 16:01:50 2026 GMT
  host: unify.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 21:26:26 2026 GMT
  host: api.unify.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unify Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unify
provider_slug: unify-ai
slug: unify-ai-domain-security
source_filename: unify-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:26:26 2026 GMT\n  hsts: null\ndomains:\n- domain: unify.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify-ai/refs/heads/main/security/unify-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM
- AI
- Large Language Models
- LLM Routing
- Model Gateway
- AI Gateway
- OpenAI
- Anthropic
- Mistral
- Benchmarking
- Model Comparison
- AI Infrastructure
- Machine Learning
---
