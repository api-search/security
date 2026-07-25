---
api_specs:
- filename: nexosai-agent-management-api-openapi.yml
  format: yaml
  label: nexos.ai Agent Management API
  slug: nexosai-agent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-agent-management-api-openapi.yml
- filename: nexosai-assistant-management-api-openapi.yml
  format: yaml
  label: nexos.ai Assistant Management API
  slug: nexosai-assistant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-assistant-management-api-openapi.yml
- filename: nexosai-audio-api-openapi.yml
  format: yaml
  label: nexos.ai Audio API
  slug: nexosai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-audio-api-openapi.yml
- filename: nexosai-batches-api-openapi.yml
  format: yaml
  label: nexos.ai Batches API
  slug: nexosai-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-batches-api-openapi.yml
- filename: nexosai-budget-limit-management-api-openapi.yml
  format: yaml
  label: nexos.ai Budget Limit Management API
  slug: nexosai-budget-limit-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-budget-limit-management-api-openapi.yml
- filename: nexosai-chat-api-openapi.yml
  format: yaml
  label: nexos.ai Chat API
  slug: nexosai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-chat-api-openapi.yml
- filename: nexosai-company-management-api-openapi.yml
  format: yaml
  label: nexos.ai Company Management API
  slug: nexosai-company-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-company-management-api-openapi.yml
- filename: nexosai-embeddings-api-openapi.yml
  format: yaml
  label: nexos.ai Embeddings API
  slug: nexosai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-embeddings-api-openapi.yml
- filename: nexosai-files-api-openapi.yml
  format: yaml
  label: nexos.ai Files API
  slug: nexosai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-files-api-openapi.yml
- filename: nexosai-images-api-openapi.yml
  format: yaml
  label: nexos.ai Images API
  slug: nexosai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-images-api-openapi.yml
- filename: nexosai-messages-api-openapi.yml
  format: yaml
  label: nexos.ai Messages API
  slug: nexosai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-messages-api-openapi.yml
- filename: nexosai-models-api-openapi.yml
  format: yaml
  label: nexos.ai Models API
  slug: nexosai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-models-api-openapi.yml
- filename: nexosai-responses-api-openapi.yml
  format: yaml
  label: nexos.ai Responses API
  slug: nexosai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-responses-api-openapi.yml
- filename: nexosai-storage-api-openapi.yml
  format: yaml
  label: nexos.ai Storage API
  slug: nexosai-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-storage-api-openapi.yml
- filename: nexosai-team-management-api-openapi.yml
  format: yaml
  label: nexos.ai Team Management API
  slug: nexosai-team-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-team-management-api-openapi.yml
- filename: nexosai-user-management-api-openapi.yml
  format: yaml
  label: nexos.ai User Management API
  slug: nexosai-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/openapi/nexosai-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nexos.ai
  spf: true
hosts:
- cert_expires: Sep 20 10:43:20 2026 GMT
  host: nexos.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexosai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nexos.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: nexos.ai
provider_slug: nexosai
slug: nexosai-domain-security
source_filename: nexosai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 10:43:20 2026 GMT\n  hsts: null\ndomains:\n- domain: nexos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexosai/refs/heads/main/security/nexosai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Machine Learning
- Embeddings
- Agents
- Developer Tools
- OpenAI Compatible
---
