---
api_specs:
- filename: mvmnt-openapi-original.yml
  format: yaml
  label: MVMNT API
  slug: mvmnt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/openapi/mvmnt-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mvmnt.io
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.mvmnt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mvmnt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MVMNT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MVMNT
provider_slug: mvmnt
slug: mvmnt-domain-security
source_filename: mvmnt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.mvmnt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mvmnt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/security/mvmnt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Freight
- Logistics
- Transportation Management System
- Supply Chain
- Brokerage
- Shipping
- Payments
- Company
---
