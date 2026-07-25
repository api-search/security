---
api_specs:
- filename: letta-ai-agent-templates-api-openapi.yml
  format: yaml
  label: Letta Agent Templates API
  slug: letta-ai-agent-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-agent-templates-api-openapi.yml
- filename: letta-ai-agents-api-openapi.yml
  format: yaml
  label: Letta Agents API
  slug: letta-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-agents-api-openapi.yml
- filename: letta-ai-archival-memory-api-openapi.yml
  format: yaml
  label: Letta Archival Memory API
  slug: letta-ai-archival-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-archival-memory-api-openapi.yml
- filename: letta-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Letta Chat Completions API
  slug: letta-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-chat-completions-api-openapi.yml
- filename: letta-ai-identities-api-openapi.yml
  format: yaml
  label: Letta Identities API
  slug: letta-ai-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-identities-api-openapi.yml
- filename: letta-ai-mcp-servers-api-openapi.yml
  format: yaml
  label: Letta MCP Servers API
  slug: letta-ai-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-mcp-servers-api-openapi.yml
- filename: letta-ai-memory-blocks-api-openapi.yml
  format: yaml
  label: Letta Memory Blocks API
  slug: letta-ai-memory-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-memory-blocks-api-openapi.yml
- filename: letta-ai-models-and-providers-api-openapi.yml
  format: yaml
  label: Letta Models and Providers API
  slug: letta-ai-models-and-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-models-and-providers-api-openapi.yml
- filename: letta-ai-multi-agent-groups-api-openapi.yml
  format: yaml
  label: Letta Multi-Agent Groups API
  slug: letta-ai-multi-agent-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-multi-agent-groups-api-openapi.yml
- filename: letta-ai-runs-jobs-and-steps-api-openapi.yml
  format: yaml
  label: Letta Runs, Jobs and Steps API
  slug: letta-ai-runs-jobs-and-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-runs-jobs-and-steps-api-openapi.yml
- filename: letta-ai-sources-and-files-api-openapi.yml
  format: yaml
  label: Letta Sources and Files API
  slug: letta-ai-sources-and-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-sources-and-files-api-openapi.yml
- filename: letta-ai-tag-api-openapi.yml
  format: yaml
  label: Letta Tag API
  slug: letta-ai-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-tag-api-openapi.yml
- filename: letta-ai-tools-api-openapi.yml
  format: yaml
  label: Letta Tools API
  slug: letta-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-tools-api-openapi.yml
- filename: letta-ai-voice-api-openapi.yml
  format: yaml
  label: Letta Voice API
  slug: letta-ai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/openapi/letta-ai-voice-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: letta.com
  spf: true
hosts:
- cert_expires: Sep  9 21:50:59 2026 GMT
  host: www.letta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 20:28:09 2026 GMT
  host: docs.letta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 01:41:01 2026 GMT
  host: api.letta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Letta Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Letta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Letta
provider_slug: letta-ai
slug: letta-ai-domain-security
source_filename: letta-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:50:59 2026 GMT\n  hsts: false\n- host: docs.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:28:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.letta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:41:01 2026 GMT\n  hsts: false\ndomains:\n- domain: letta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/security/letta-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- LLM
- Memory
- Stateful Agents
- MemGPT
---
