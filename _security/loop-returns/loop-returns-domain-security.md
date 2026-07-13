---
api_specs:
- filename: loop-returns-returns-openapi.yml
  format: yaml
  label: Loop Returns API
  slug: loop-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop-returns/refs/heads/main/openapi/loop-returns-returns-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loopreturns.com
  spf: true
hosts:
- cert_expires: Sep 23 07:57:33 2026 GMT
  host: www.loopreturns.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:47:30 2026 GMT
  host: docs.loopreturns.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 07:09:38 2026 GMT
  host: api.loopreturns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loop Returns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loop Returns, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loop Returns
provider_slug: loop-returns
slug: loop-returns-domain-security
source_filename: loop-returns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loopreturns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.loopreturns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:47:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.loopreturns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 07:09:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loopreturns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop-returns/refs/heads/main/security/loop-returns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Returns
- E-Commerce
- Exchanges
- Refunds
- Shipping
- Post-Purchase
- Shopify
- Fraud Prevention
- Retail
---
