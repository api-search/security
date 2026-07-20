---
api_specs:
- filename: lendapi-openapi.json
  format: json
  label: LendAPI API
  slug: lendapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/openapi/lendapi-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lendapi.com
  spf: true
hosts:
- cert_expires: Oct  2 11:56:38 2026 GMT
  host: lendapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 24 23:59:59 2026 GMT
  host: app.lendapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lendapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LendAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LendAPI
provider_slug: lendapi
slug: lendapi-domain-security
source_filename: lendapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:56:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.lendapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lendapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendapi/refs/heads/main/security/lendapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lending
- Loan Origination
- Financial Services
- Fintech
- Embedded Finance
- Underwriting
- Decision Engine
- Credit
- Banking
- Account Opening
- KYC
- KYB
- Buy Now Pay Later
- Point of Sale
---
