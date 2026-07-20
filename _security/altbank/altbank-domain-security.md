---
api_specs:
- filename: altbank-guard-openapi.yml
  format: yaml
  label: alt.bank GUARD API
  slug: altbank-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altbank/refs/heads/main/openapi/altbank-guard-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: altbank.com.br
  spf: false
hosts:
- cert_expires: Aug 20 22:20:08 2026 GMT
  host: www.altbank.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for alt.bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: alt.bank
provider_slug: altbank
slug: altbank-domain-security
source_filename: altbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:20:08 2026 GMT\n  hsts: false\ndomains:\n- domain: altbank.com.br\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altbank/refs/heads/main/security/altbank-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Banking
- Credit Cards
- Card Issuing
- Underwriting
- Payments
- Brazil
- KYC
---
