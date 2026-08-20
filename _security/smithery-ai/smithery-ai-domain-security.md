---
api_specs:
- filename: smithery-ai-connect-api-openapi.yml
  format: yaml
  label: Smithery connect API
  slug: smithery-ai-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-connect-api-openapi.yml
- filename: smithery-ai-connect-mcp-api-openapi.yml
  format: yaml
  label: Smithery connect.mcp API
  slug: smithery-ai-connect-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-connect-mcp-api-openapi.yml
- filename: smithery-ai-domains-api-openapi.yml
  format: yaml
  label: Smithery domains API
  slug: smithery-ai-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-domains-api-openapi.yml
- filename: smithery-ai-health-api-openapi.yml
  format: yaml
  label: Smithery Health API
  slug: smithery-ai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-health-api-openapi.yml
- filename: smithery-ai-namespaces-api-openapi.yml
  format: yaml
  label: Smithery namespaces API
  slug: smithery-ai-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-namespaces-api-openapi.yml
- filename: smithery-ai-organizations-api-openapi.yml
  format: yaml
  label: Smithery organizations API
  slug: smithery-ai-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-organizations-api-openapi.yml
- filename: smithery-ai-servers-api-openapi.yml
  format: yaml
  label: Smithery servers API
  slug: smithery-ai-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-servers-api-openapi.yml
- filename: smithery-ai-skills-api-openapi.yml
  format: yaml
  label: Smithery skills API
  slug: smithery-ai-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-skills-api-openapi.yml
- filename: smithery-ai-tokens-api-openapi.yml
  format: yaml
  label: Smithery tokens API
  slug: smithery-ai-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/openapi/smithery-ai-tokens-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smithery.ai
  spf: true
hosts:
- cert_expires: Sep 23 15:19:05 2026 GMT
  host: smithery.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:31:52 2026 GMT
  host: api.smithery.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smithery Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smithery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smithery
provider_slug: smithery-ai
slug: smithery-ai-domain-security
source_filename: smithery-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:31:52 2026 GMT\n  hsts: null\ndomains:\n- domain: smithery.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery-ai/refs/heads/main/security/smithery-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Agents
- MCP
- Registry
- Hosting
- Tools
- Skills
- Marketplace
- Developer Platform
---
