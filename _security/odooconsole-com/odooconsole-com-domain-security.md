---
api_specs:
- filename: odooconsole-com-discovery-api-openapi.yml
  format: yaml
  label: OConsole Discovery API
  slug: odooconsole-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-discovery-api-openapi.yml
- filename: odooconsole-com-mcp-api-openapi.yml
  format: yaml
  label: OConsole MCP API
  slug: odooconsole-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: odooconsole.com
  spf: true
hosts:
- cert_expires: Jan  3 08:46:20 2027 GMT
  host: odooconsole.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OConsole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OConsole, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OConsole
provider_slug: odooconsole-com
slug: odooconsole-com-domain-security
source_filename: odooconsole-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: odooconsole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 08:46:20 2027 GMT\n  hsts: null\ndomains:\n- domain: odooconsole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/odooconsole-com/security/odooconsole-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- ERP
- Hosting
- Odoo
---
