---
api_specs:
- filename: light-openapi-original.json
  format: json
  label: Light API
  slug: light-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/openapi/light-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: light.inc
  spf: true
hosts:
- cert_expires: Oct 14 07:38:44 2026 GMT
  host: light.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Light Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Light, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Light
provider_slug: light
slug: light-domain-security
source_filename: light-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: light.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: light.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light/refs/heads/main/security/light-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Finance
- ERP
- Accounts Payable
- Accounts Receivable
- General Ledger
- Spend Management
- Invoicing
- Corporate Cards
- Expense Management
- Financial Operations
- Agents
- Company
---
