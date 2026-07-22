---
api_specs:
- filename: yokoy-openapi-original.json
  format: json
  label: Yokoy API
  slug: yokoy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/openapi/yokoy-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yokoy.io
  spf: true
hosts:
- cert_expires: Sep 28 19:43:59 2026 GMT
  host: yokoy.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yokoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yokoy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yokoy
provider_slug: yokoy
slug: yokoy-domain-security
source_filename: yokoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yokoy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:43:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yokoy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/security/yokoy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Spend Management
- Expense Management
- Invoice Management
- Finance Automation
- Corporate Cards
- Fintech
- SaaS
---
