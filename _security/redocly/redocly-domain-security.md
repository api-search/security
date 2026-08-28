---
api_specs:
- filename: redocly-search-api-openapi.yaml
  format: yaml
  label: Redocly Realm Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yaml
- filename: redocly-docs-mcp-openapi.yaml
  format: yaml
  label: Redocly Docs MCP Server
  slug: redocly-docs-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-docs-mcp-openapi.yaml
- filename: redocly-scout-openapi.yaml
  format: yaml
  label: Redocly Scout API
  slug: redocly-scout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-openapi.yaml
- filename: redocly-scout-agent-openapi.yaml
  format: yaml
  label: Redocly Scout Agent API
  slug: redocly-scout-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-agent-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: redocly.com
  spf: true
hosts:
- cert_expires: Oct  8 16:47:51 2026 GMT
  host: redocly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redocly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redocly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Redocly
provider_slug: redocly
slug: redocly-domain-security
source_filename: redocly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redocly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:47:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redocly.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/security/redocly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
---
