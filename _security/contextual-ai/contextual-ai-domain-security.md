---
api_specs:
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agents API
  slug: contextual-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Agent Query API
  slug: contextual-ai-agent-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Datastores & Documents API
  slug: contextual-ai-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Generate API
  slug: contextual-ai-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Rerank API
  slug: contextual-ai-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI Parse API
  slug: contextual-ai-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
- filename: contextual-ai-openapi.yml
  format: yaml
  label: Contextual AI LMUnit Evaluation API
  slug: contextual-ai-lmunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/openapi/contextual-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contextual.ai
  spf: true
hosts:
- cert_expires: Sep  2 09:40:40 2026 GMT
  host: contextual.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 22:34:50 2026 GMT
  host: docs.contextual.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 16:52:20 2026 GMT
  host: api.contextual.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Contextual Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contextual AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contextual AI
provider_slug: contextual-ai
slug: contextual-ai-domain-security
source_filename: contextual-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contextual.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:40:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.contextual.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 22:34:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.contextual.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:52:20 2026 GMT\n  hsts: null\ndomains:\n- domain: contextual.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextual-ai/refs/heads/main/security/contextual-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- RAG
- LLM
- Grounded Language Model
- Enterprise
---
