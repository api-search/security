---
api_specs:
- filename: global-payments-unified-payments-api-openapi.yml
  format: yaml
  label: Global Payments Unified Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-payments/refs/heads/main/openapi/global-payments-unified-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globalpayments.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: globalpay.com
  spf: true
hosts:
- cert_expires: Aug 22 23:59:59 2026 GMT
  host: developer.globalpayments.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:46:13 2026 GMT
  host: www.globalpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: apis.globalpay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Global Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Payments, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Global Payments
provider_slug: global-payments
slug: global-payments-domain-security
source_filename: global-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.globalpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.globalpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:46:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.globalpay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: globalpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: globalpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-payments/refs/heads/main/security/global-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Payment Processing
- Payment Technology
- Payments
- POS
- Fortune 1000
---
