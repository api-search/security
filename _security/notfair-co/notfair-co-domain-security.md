---
api_specs:
- filename: notfair-co-health-api-openapi.yml
  format: yaml
  label: notfair-co Health API
  slug: notfair-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-health-api-openapi.yml
- filename: notfair-co-mcp-api-openapi.yml
  format: yaml
  label: notfair-co MCP API
  slug: notfair-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-mcp-api-openapi.yml
- filename: notfair-co-well-known-api-openapi.yml
  format: yaml
  label: notfair-co .well Known API
  slug: notfair-co-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notfair.co
  spf: false
hosts:
- cert_expires: Nov 28 23:51:39 2026 GMT
  host: notfair.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Notfair Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for notfair-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: notfair-co
provider_slug: notfair-co
slug: notfair-co-domain-security
source_filename: notfair-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notfair.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:51:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: notfair.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/notfair-co/security/notfair-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AI
- Marketing
- Automation
---
