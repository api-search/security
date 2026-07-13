---
api_specs:
- filename: introducao
  format: yaml
  label: PagBank Orders API
  slug: pagbank-orders-api
  spec_type: OpenAPI
  url: https://developer.pagbank.com.br/reference/introducao
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagbank.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagseguro.com
  spf: true
hosts:
- cert_expires: Oct  3 22:43:13 2026 GMT
  host: pagbank.com.br
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:08:37 2026 GMT
  host: developer.pagbank.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.pagseguro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pagbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PagBank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PagBank
provider_slug: pagbank
slug: pagbank-domain-security
source_filename: pagbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:43:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.pagbank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pagseguro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pagbank.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pagseguro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagbank/refs/heads/main/security/pagbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Digital Banking
- Brazil
- PIX
- Fintech
- E-Commerce
- POS
- Recurring Payments
- Boleto
---
