---
api_specs:
- filename: galileo-ai-annotations-api-openapi.yml
  format: yaml
  label: Galileo Annotations API
  slug: galileo-ai-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-annotations-api-openapi.yml
- filename: galileo-ai-apikeys-api-openapi.yml
  format: yaml
  label: Galileo ApiKeys API
  slug: galileo-ai-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-apikeys-api-openapi.yml
- filename: galileo-ai-auth-api-openapi.yml
  format: yaml
  label: Galileo Auth API
  slug: galileo-ai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-auth-api-openapi.yml
- filename: galileo-ai-datasets-api-openapi.yml
  format: yaml
  label: Galileo Datasets API
  slug: galileo-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-datasets-api-openapi.yml
- filename: galileo-ai-experiments-api-openapi.yml
  format: yaml
  label: Galileo Experiments API
  slug: galileo-ai-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-experiments-api-openapi.yml
- filename: galileo-ai-groups-api-openapi.yml
  format: yaml
  label: Galileo Groups API
  slug: galileo-ai-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-groups-api-openapi.yml
- filename: galileo-ai-health-api-openapi.yml
  format: yaml
  label: Galileo Health API
  slug: galileo-ai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-health-api-openapi.yml
- filename: galileo-ai-integrations-api-openapi.yml
  format: yaml
  label: Galileo Integrations API
  slug: galileo-ai-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/openapi/galileo-ai-integrations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: galileo.ai
  spf: true
hosts:
- cert_expires: Sep 25 15:02:15 2026 GMT
  host: galileo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:52:22 2026 GMT
  host: docs.galileo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:42:58 2026 GMT
  host: api.galileo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Galileo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Galileo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Galileo
provider_slug: galileo-ai
slug: galileo-ai-domain-security
source_filename: galileo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:52:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.galileo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:42:58 2026 GMT\n  hsts: null\ndomains:\n- domain: galileo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/galileo-ai/refs/heads/main/security/galileo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Evaluation
- AI Observability
- GenAI
- Guardrails
- Agentic AI
- LLM
- Tracing
- Experiments
- Prompts
- Datasets
---
