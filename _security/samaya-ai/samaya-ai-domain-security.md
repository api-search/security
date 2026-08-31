---
api_specs:
- filename: samaya-ai-organizations-api-openapi.yml
  format: yaml
  label: Samaya AI Organizations API
  slug: samaya-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-organizations-api-openapi.yml
- filename: samaya-ai-teams-api-openapi.yml
  format: yaml
  label: Samaya AI Teams API
  slug: samaya-ai-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-teams-api-openapi.yml
- filename: samaya-ai-users-api-openapi.yml
  format: yaml
  label: Samaya AI Users API
  slug: samaya-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/openapi/samaya-ai-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: samaya.ai
  spf: true
hosts:
- cert_expires: Oct 31 08:14:14 2026 GMT
  host: samaya.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 21:31:00 2026 GMT
  host: api.samaya.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 21:31:00 2026 GMT
  host: mcp.samaya.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Samaya Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Samaya AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Samaya AI
provider_slug: samaya-ai
slug: samaya-ai-domain-security
source_filename: samaya-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: samaya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 08:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.samaya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 21:31:00 2026 GMT\n  hsts: null\n- host: mcp.samaya.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 21:31:00 2026 GMT\n  hsts: null\ndomains:\n- domain: samaya.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samaya-ai/refs/heads/main/security/samaya-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- artificial-intelligence
- Financial-Services
- investment-research
- AI Agents
- MCP
- agent-native
- capital-markets
- enterprise-search
- retrieval
- graphql
---
