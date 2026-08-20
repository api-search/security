---
api_specs:
- filename: sideko-api-projects-api-openapi.yml
  format: yaml
  label: Sideko API Projects API
  slug: sideko-api-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-api-projects-api-openapi.yml
- filename: sideko-api-versions-api-openapi.yml
  format: yaml
  label: Sideko API Versions API
  slug: sideko-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-api-versions-api-openapi.yml
- filename: sideko-authentication-api-openapi.yml
  format: yaml
  label: Sideko Authentication API
  slug: sideko-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-authentication-api-openapi.yml
- filename: sideko-documentation-api-openapi.yml
  format: yaml
  label: Sideko Documentation API
  slug: sideko-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-documentation-api-openapi.yml
- filename: sideko-linting-api-openapi.yml
  format: yaml
  label: Sideko Linting API
  slug: sideko-linting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-linting-api-openapi.yml
- filename: sideko-mcp-generation-api-openapi.yml
  format: yaml
  label: Sideko MCP Generation API
  slug: sideko-mcp-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-mcp-generation-api-openapi.yml
- filename: sideko-mock-servers-api-openapi.yml
  format: yaml
  label: Sideko Mock Servers API
  slug: sideko-mock-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-mock-servers-api-openapi.yml
- filename: sideko-sdk-generation-api-openapi.yml
  format: yaml
  label: Sideko SDK Generation API
  slug: sideko-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-sdk-generation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sideko.dev
  spf: true
hosts:
- cert_expires: Aug 30 06:51:19 2026 GMT
  host: www.sideko.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:10:51 2026 GMT
  host: docs.sideko.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:55:29 2026 GMT
  host: api.sideko.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sideko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sideko, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sideko
provider_slug: sideko
slug: sideko-domain-security
source_filename: sideko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:51:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:10:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sideko.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:55:29 2026 GMT\n  hsts: null\ndomains:\n- domain: sideko.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/security/sideko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CLI
- Documentation
- Mock Servers
- Platform
- SDK
- API Tooling
- SDK Generation
- MCP Generation
- Artificial Intelligence
- Hybrid Codegen
- OpenAPI Linting
---
