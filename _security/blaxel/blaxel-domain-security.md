---
api_specs:
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Agents API
  slug: blaxel-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Functions / MCP Servers API
  slug: blaxel-functions-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Models Gateway API
  slug: blaxel-models-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Sandboxes API
  slug: blaxel-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Jobs API
  slug: blaxel-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Policies API
  slug: blaxel-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Integrations API
  slug: blaxel-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
- filename: blaxel-openapi.yml
  format: yaml
  label: Blaxel Workspaces API
  slug: blaxel-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/openapi/blaxel-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blaxel.ai
  spf: true
hosts:
- cert_expires: Sep 24 14:26:22 2026 GMT
  host: blaxel.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 02:26:43 2026 GMT
  host: docs.blaxel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.blaxel.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blaxel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blaxel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blaxel
provider_slug: blaxel
slug: blaxel-domain-security
source_filename: blaxel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blaxel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:26:22 2026 GMT\n  hsts: false\n- host: docs.blaxel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:26:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.blaxel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: blaxel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blaxel/refs/heads/main/security/blaxel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- Infrastructure
- Sandboxes
- MCP
- Compute
- Serverless
---
