---
api_specs:
- filename: fat-zebra-gateway.json
  format: json
  label: Fat Zebra Gateway API
  slug: fat-zebra-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-gateway.json
- filename: fat-zebra-partner.json
  format: json
  label: Fat Zebra Partner API
  slug: fat-zebra-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-partner.json
- filename: fat-zebra-billing.json
  format: json
  label: Fat Zebra Billing API
  slug: fat-zebra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-billing.json
- filename: fat-zebra-fdms-tpp-merchant-onboarding.json
  format: json
  label: Fat Zebra FDMS TPP Merchant Onboarding API
  slug: fat-zebra-fdms-tpp-merchant-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/openapi/fat-zebra-fdms-tpp-merchant-onboarding.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fatzebra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pmnts.io
  spf: true
hosts:
- cert_expires: Sep 30 22:35:26 2026 GMT
  host: www.fatzebra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:55:15 2026 GMT
  host: docs.fatzebra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: gateway.pmnts.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fat Zebra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fat Zebra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fat Zebra
provider_slug: fat-zebra
slug: fat-zebra-domain-security
source_filename: fat-zebra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fatzebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:35:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fatzebra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:55:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.pmnts.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fatzebra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: pmnts.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fat-zebra/refs/heads/main/security/fat-zebra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- Tokenization
- Recurring Billing
- Direct Debit
- Hosted Payment Pages
- Merchant Onboarding
---
