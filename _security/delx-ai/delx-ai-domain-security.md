---
api_specs:
- filename: delx-ai-a2a-api-openapi.yml
  format: yaml
  label: Delx A2a API
  slug: delx-ai-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-a2a-api-openapi.yml
- filename: delx-ai-agents-api-openapi.yml
  format: yaml
  label: Delx Agents API
  slug: delx-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-agents-api-openapi.yml
- filename: delx-ai-discovery-api-openapi.yml
  format: yaml
  label: Delx Discovery API
  slug: delx-ai-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-discovery-api-openapi.yml
- filename: delx-ai-mcp-api-openapi.yml
  format: yaml
  label: Delx MCP API
  slug: delx-ai-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-mcp-api-openapi.yml
- filename: delx-ai-protocol-api-openapi.yml
  format: yaml
  label: Delx Protocol API
  slug: delx-ai-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-protocol-api-openapi.yml
- filename: delx-ai-reliability-api-openapi.yml
  format: yaml
  label: Delx Reliability API
  slug: delx-ai-reliability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-reliability-api-openapi.yml
- filename: delx-ai-tools-api-openapi.yml
  format: yaml
  label: Delx Tools API
  slug: delx-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-tools-api-openapi.yml
- filename: delx-ai-x402-api-openapi.yml
  format: yaml
  label: Delx X402 API
  slug: delx-ai-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delx.ai
  spf: true
hosts:
- cert_expires: Nov 12 21:05:40 2026 GMT
  host: delx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 22:37:38 2026 GMT
  host: ontology.delx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 21:19:57 2026 GMT
  host: api.delx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Delx Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delx
provider_slug: delx-ai
slug: delx-ai-domain-security
source_filename: delx-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 21:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ontology.delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 22:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 21:19:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: delx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/security/delx-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI Agents
- MCP
- A2A
- x402
- Agentic Commerce
- Agent Continuity
- Agent Recovery
- Media Generation
- Web Intelligence
- Data Quality
- Agent-Native
---
