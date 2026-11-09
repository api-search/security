---
api_specs:
- filename: datamcp-app-openapi-generated.yml
  format: yaml
  label: datamcp API
  slug: datamcp-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datamcp-app/openapi/_ae-authored/datamcp-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datamcp.app
  spf: true
hosts:
- cert_expires: Jan  1 11:08:34 2027 GMT
  host: datamcp.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datamcp App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for datamcp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: datamcp
provider_slug: datamcp-app
slug: datamcp-app-domain-security
source_filename: datamcp-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datamcp.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 11:08:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datamcp.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datamcp-app/security/datamcp-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- MCP
- OpenAPI
- Artificial Intelligence
---
