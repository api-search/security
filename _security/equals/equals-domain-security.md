---
api_specs:
- filename: equals-memories-api-openapi.yml
  format: yaml
  label: Equals Memories API
  slug: equals-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equals/refs/heads/main/openapi/equals-memories-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: equals.com
  spf: true
hosts:
- cert_expires: Sep 21 20:43:50 2026 GMT
  host: equals.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:49:50 2026 GMT
  host: docs.equals.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 14:28:21 2026 GMT
  host: go.equals.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equals, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Equals
provider_slug: equals
slug: equals-domain-security
source_filename: equals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.equals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:49:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: go.equals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:28:21 2026 GMT\n  hsts: null\ndomains:\n- domain: equals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equals/refs/heads/main/security/equals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Spreadsheets
- Business Intelligence
- Dashboards
- Data
- Revenue Operations
- Reporting
- MCP
---
