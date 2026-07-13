---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Firstrade Account Data API (via Plaid)
  slug: firstrade-account-data-api-via-plaid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firstrade.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plaid.com
  spf: true
hosts:
- cert_expires: Sep 28 17:50:12 2026 GMT
  host: www.firstrade.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: plaid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: production.plaid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Firstrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firstrade, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Firstrade
provider_slug: firstrade
slug: firstrade-domain-security
source_filename: firstrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:50:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: plaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.plaid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: firstrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: plaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstrade/refs/heads/main/security/firstrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Brokerage
- Commission-Free Trading
- Stocks
- ETFs
- Options
- Mutual Funds
- Fixed Income
- Retirement
- IRA
- Investing
- Finance
- Open Banking
---
