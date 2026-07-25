---
api_specs:
- filename: till-payments-gateway.yml
  format: yaml
  label: Till Payments Gateway API
  slug: till-payments-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-gateway.yml
- filename: till-payments-direct-pci.yml
  format: yaml
  label: Till Payments Direct PCI-enabled API
  slug: till-payments-direct-pci
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-direct-pci.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tillpayments.com
  spf: true
hosts:
- cert_expires: Sep 20 22:22:15 2026 GMT
  host: tillpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 18:15:56 2026 GMT
  host: gateway.tillpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 19:53:21 2026 GMT
  host: secure.tillpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Till Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Till Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Till Payments
provider_slug: till-payments
slug: till-payments-domain-security
source_filename: till-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tillpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:22:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.tillpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:15:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.tillpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:53:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tillpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/security/till-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- Card Payments
- In-Person Payments
---
