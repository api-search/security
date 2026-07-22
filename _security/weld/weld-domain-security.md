---
api_specs:
- filename: weld-connect-openapi.json
  format: json
  label: Weld Connect API
  slug: weld-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-connect-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weld.app
  spf: true
hosts:
- cert_expires: Sep 18 23:11:47 2026 GMT
  host: weld.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: connect.weld.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Weld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weld, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Weld
provider_slug: weld
slug: weld-domain-security
source_filename: weld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weld.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: connect.weld.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: weld.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/security/weld-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Data
- ETL
- ELT
- Reverse ETL
- Data Pipelines
- Data Integration
- Change Data Capture
- Transformations
- Analytics
- MCP
- AI Agents
---
