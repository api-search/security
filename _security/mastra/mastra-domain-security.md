---
api_specs:
- filename: mastra-agents-api-openapi.yml
  format: yaml
  label: Mastra Agents API
  slug: mastra-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-agents-api-openapi.yml
- filename: mastra-conversations-api-openapi.yml
  format: yaml
  label: Mastra Conversations API
  slug: mastra-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-conversations-api-openapi.yml
- filename: mastra-logs-api-openapi.yml
  format: yaml
  label: Mastra Logs API
  slug: mastra-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-logs-api-openapi.yml
- filename: mastra-mcp-api-openapi.yml
  format: yaml
  label: Mastra Mcp API
  slug: mastra-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-mcp-api-openapi.yml
- filename: mastra-memory-api-openapi.yml
  format: yaml
  label: Mastra Memory API
  slug: mastra-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-memory-api-openapi.yml
- filename: mastra-responses-api-openapi.yml
  format: yaml
  label: Mastra Responses API
  slug: mastra-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-responses-api-openapi.yml
- filename: mastra-telemetry-api-openapi.yml
  format: yaml
  label: Mastra Telemetry API
  slug: mastra-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-telemetry-api-openapi.yml
- filename: mastra-tools-api-openapi.yml
  format: yaml
  label: Mastra Tools API
  slug: mastra-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-tools-api-openapi.yml
- filename: mastra-vectors-api-openapi.yml
  format: yaml
  label: Mastra Vectors API
  slug: mastra-vectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-vectors-api-openapi.yml
- filename: mastra-workflows-api-openapi.yml
  format: yaml
  label: Mastra Workflows API
  slug: mastra-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/openapi/mastra-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mastra.ai
  spf: true
hosts:
- cert_expires: Sep 20 21:27:30 2026 GMT
  host: mastra.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mastra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mastra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mastra
provider_slug: mastra
slug: mastra-domain-security
source_filename: mastra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mastra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mastra.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastra/refs/heads/main/security/mastra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Artificial Intelligence
- JavaScript
- RAG
- TypeScript
- Workflows
---
