---
api_specs:
- filename: camdentools-com-mcp-api-openapi.yml
  format: yaml
  label: Camden Tools MCP API
  slug: camdentools-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/camdentools-com/openapi/camdentools-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: camdentools.com
  spf: true
hosts:
- cert_expires: Jan 27 21:14:35 2027 GMT
  host: camdentools.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Camden Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camden Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Camden Tools
provider_slug: camdentools-com
slug: camdentools-com-domain-security
source_filename: camdentools-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: camdentools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 21:14:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: camdentools.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/camdentools-com/security/camdentools-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tools
- Construction
- Retail
- United Kingdom
---
