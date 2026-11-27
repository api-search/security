---
api_specs:
- filename: linkdr-admin-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP Admin MCP API
  slug: linkdr-admin-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-admin-mcp-api-openapi.yml
- filename: linkdr-agent-resources-api-openapi.yml
  format: yaml
  label: LinkDR MCP Agent resources API
  slug: linkdr-agent-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-agent-resources-api-openapi.yml
- filename: linkdr-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP MCP API
  slug: linkdr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-mcp-api-openapi.yml
- filename: linkdr-public-data-api-openapi.yml
  format: yaml
  label: LinkDR MCP Public data API
  slug: linkdr-public-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-public-data-api-openapi.yml
- filename: linkdr-system-api-openapi.yml
  format: yaml
  label: LinkDR MCP System API
  slug: linkdr-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linkdr.com
  spf: true
hosts:
- cert_expires: Dec 17 22:18:30 2026 GMT
  host: linkdr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LinkDR MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkDR MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LinkDR MCP
provider_slug: linkdr
slug: linkdr-domain-security
source_filename: linkdr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkdr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 22:18:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: linkdr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/linkdr/security/linkdr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SEO
- Backlink
- Artificial Intelligence
- Software-as-a-Service
---
