---
api_specs:
- filename: roosteragents-ai-agent-readiness-api-openapi.yml
  format: yaml
  label: roosteragents-ai Agent Readiness API
  slug: roosteragents-ai-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-agent-readiness-api-openapi.yml
- filename: roosteragents-ai-gateway-api-openapi.yml
  format: yaml
  label: roosteragents-ai Gateway API
  slug: roosteragents-ai-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-gateway-api-openapi.yml
- filename: roosteragents-ai-mcp-api-openapi.yml
  format: yaml
  label: roosteragents-ai MCP API
  slug: roosteragents-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-mcp-api-openapi.yml
- filename: roosteragents-ai-scan-api-openapi.yml
  format: yaml
  label: roosteragents-ai Scan API
  slug: roosteragents-ai-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-scan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roosteragents.ai
  spf: true
hosts:
- cert_expires: Dec 30 18:30:19 2026 GMT
  host: roosteragents.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Roosteragents Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for roosteragents-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: roosteragents-ai
provider_slug: roosteragents-ai
slug: roosteragents-ai-domain-security
source_filename: roosteragents-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roosteragents.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 18:30:19 2026 GMT\n  hsts: false\ndomains:\n- domain: roosteragents.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/roosteragents-ai/security/roosteragents-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Marketing
- Automation
- SaaS
- Data
---
