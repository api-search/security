---
api_specs:
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow API
  slug: langflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Flows API
  slug: langflow-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Run API
  slug: langflow-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Build API
  slug: langflow-build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Projects API
  slug: langflow-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Files API
  slug: langflow-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Monitor API
  slug: langflow-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Traces API
  slug: langflow-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Users API
  slug: langflow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow MCP API
  slug: langflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow Workflow API
  slug: langflow-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow OpenAI Responses API
  slug: langflow-openai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
- filename: langflow-openapi.yml
  format: yaml
  label: Langflow API Keys API
  slug: langflow-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/openapi/langflow-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: langflow.org
  spf: true
hosts:
- cert_expires: Aug 20 18:14:06 2026 GMT
  host: www.langflow.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:34:48 2026 GMT
  host: docs.langflow.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Langflow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Langflow
provider_slug: langflow
slug: langflow-domain-security
source_filename: langflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.langflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.langflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:34:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: langflow.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langflow/refs/heads/main/security/langflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Agents
- Workflows
- Low-Code
- Visual Builder
- LangChain
- RAG
- MCP
- Open Source
- FastAPI
---
