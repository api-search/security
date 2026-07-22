---
api_specs:
- filename: super-payments-openapi.yml
  format: yaml
  label: Super Payments API
  slug: super-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/openapi/super-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superpayments.com
  spf: true
hosts:
- cert_expires: Aug 27 15:00:12 2026 GMT
  host: www.superpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:11:41 2026 GMT
  host: docs.superpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 10:46:00 2026 GMT
  host: api.superpayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Super Payments
provider_slug: super-payments
slug: super-payments-domain-security
source_filename: super-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.superpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:11:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.superpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 10:46:00 2026 GMT\n  hsts: null\ndomains:\n- domain: superpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-payments/refs/heads/main/security/super-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Open Banking
- Cash Rewards
- Checkout
- Fintech
- United Kingdom
- Pay by Bank
---
