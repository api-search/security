---
api_specs:
- filename: astrada-openapi-original.json
  format: json
  label: Astrada API
  slug: astrada-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrada.co
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: astrada.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astrada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astrada
provider_slug: astrada
slug: astrada-domain-security
source_filename: astrada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astrada.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: astrada.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/security/astrada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Card Data
- Transaction Data
- Reconciliation
- Expense Management
- Data Infrastructure
---
