---
api_specs:
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream Connect
  slug: connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-mcp-openapi.yml
  format: yaml
  label: Pipedream MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-mcp-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pipedream.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pipedream.net
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: pipedream.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.pipedream.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: remote.mcp.pipedream.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pipedream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pipedream, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pipedream
provider_slug: pipedream
slug: pipedream-domain-security
source_filename: pipedream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pipedream.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pipedream.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: remote.mcp.pipedream.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pipedream.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pipedream.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/security/pipedream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ProCode_API_Composition
- Workflows
- Connect
- MCP
- Embedded Integrations
- Managed Auth
- AI Agents
---
