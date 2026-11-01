---
api_specs:
- filename: lovedone-app-content-api-openapi.yml
  format: yaml
  label: lovedone-app Content API
  slug: lovedone-app-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-content-api-openapi.yml
- filename: lovedone-app-discovery-api-openapi.yml
  format: yaml
  label: lovedone-app Discovery API
  slug: lovedone-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-discovery-api-openapi.yml
- filename: lovedone-app-mcp-api-openapi.yml
  format: yaml
  label: lovedone-app MCP API
  slug: lovedone-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lovedone-app/openapi/lovedone-app-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lovedone.app
  spf: true
hosts:
- cert_expires: Dec 19 01:52:01 2026 GMT
  host: lovedone.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lovedone App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lovedone-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: lovedone-app
provider_slug: lovedone-app
slug: lovedone-app-domain-security
source_filename: lovedone-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovedone.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:52:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lovedone.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lovedone-app/security/lovedone-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Family Care
- Inbox
- Healthcare
- Communication
- Privacy
---
