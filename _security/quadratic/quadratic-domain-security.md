---
api_specs:
- filename: quadratic-openapi.json
  format: json
  label: Quadratic Developer API
  slug: quadratic-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/openapi/quadratic-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: quadratichq.com
  spf: true
hosts:
- cert_expires: Sep 13 21:32:31 2026 GMT
  host: www.quadratichq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quadratic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quadratic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Quadratic
provider_slug: quadratic
slug: quadratic-domain-security
source_filename: quadratic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quadratichq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:32:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quadratichq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quadratic/refs/heads/main/security/quadratic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Spreadsheet
- Analytics
- Data
- Developer Tools
- MCP
- Productivity
---
