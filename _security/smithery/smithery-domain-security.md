---
api_specs:
- filename: smithery-connect-api-openapi.yml
  format: yaml
  label: Smithery connect API
  slug: smithery-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-connect-api-openapi.yml
- filename: smithery-connect-mcp-api-openapi.yml
  format: yaml
  label: Smithery connect.mcp API
  slug: smithery-connect-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-connect-mcp-api-openapi.yml
- filename: smithery-domains-api-openapi.yml
  format: yaml
  label: Smithery domains API
  slug: smithery-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-domains-api-openapi.yml
- filename: smithery-health-api-openapi.yml
  format: yaml
  label: Smithery Health API
  slug: smithery-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-health-api-openapi.yml
- filename: smithery-namespaces-api-openapi.yml
  format: yaml
  label: Smithery namespaces API
  slug: smithery-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-namespaces-api-openapi.yml
- filename: smithery-organizations-api-openapi.yml
  format: yaml
  label: Smithery organizations API
  slug: smithery-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-organizations-api-openapi.yml
- filename: smithery-servers-api-openapi.yml
  format: yaml
  label: Smithery servers API
  slug: smithery-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-servers-api-openapi.yml
- filename: smithery-skills-api-openapi.yml
  format: yaml
  label: Smithery skills API
  slug: smithery-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-skills-api-openapi.yml
- filename: smithery-tokens-api-openapi.yml
  format: yaml
  label: Smithery tokens API
  slug: smithery-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/openapi/smithery-tokens-api-openapi.yml
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
name: Smithery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smithery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smithery
provider_slug: smithery
slug: smithery-domain-security
source_filename: smithery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:19:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smithery.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:31:52 2026 GMT\n  hsts: null\ndomains:\n- domain: smithery.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithery/refs/heads/main/security/smithery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Large Language Models
- MCP
- Model Context Protocol
- AI Agents
- Developer Tools
- Registry
- Skills
- Tool Discovery
---
