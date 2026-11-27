---
api_specs:
- filename: chimpanseo-app-audit-api-openapi.yml
  format: yaml
  label: ChimpanSEO Audit API
  slug: chimpanseo-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimpanseo-app/openapi/chimpanseo-app-audit-api-openapi.yml
- filename: chimpanseo-app-mcp-api-openapi.yml
  format: yaml
  label: ChimpanSEO MCP API
  slug: chimpanseo-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chimpanseo-app/openapi/chimpanseo-app-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chimpanseo.app
  spf: true
hosts:
- cert_expires: Jan 11 04:37:06 2027 GMT
  host: chimpanseo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ChimpanSEO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChimpanSEO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ChimpanSEO
provider_slug: chimpanseo-app
slug: chimpanseo-app-domain-security
source_filename: chimpanseo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chimpanseo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:37:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chimpanseo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chimpanseo-app/security/chimpanseo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SEO
- Generative Engine Optimization
- AI Content
- Content Marketing
- WordPress
- MCP
---
