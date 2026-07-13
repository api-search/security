---
api_specs:
- filename: opay-cashier-api-openapi.yml
  format: yaml
  label: OPay Cashier API
  slug: opay-cashier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/openapi/opay-cashier-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opayweb.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opaycheckout.com
  spf: false
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.opayweb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: documentation.opaycheckout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: liveapi.opaycheckout.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OPay, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OPay
provider_slug: opay
slug: opay-domain-security
source_filename: opay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opayweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: documentation.opaycheckout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: false\n- host: liveapi.opaycheckout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: opayweb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: opaycheckout.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opay/refs/heads/main/security/opay-domain-security.yml
summary_line: TLSv1.3
tags:
- Payments
- Mobile Money
- Fintech
- Super App
- Nigeria
- Africa
- Wallet
- Savings
- BNPL
- Bank Transfer
- Card Payments
- USSD
- Agent Banking
- POS
- Bill Payments
- Airtime
- Cashier
- Checkout
- Merchant Acquiring
---
