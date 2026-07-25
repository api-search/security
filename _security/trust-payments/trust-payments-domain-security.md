---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trustpayments.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: securetrading.net
  spf: true
hosts:
- cert_expires: Oct  8 00:29:04 2026 GMT
  host: www.trustpayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:41:42 2026 GMT
  host: help.trustpayments.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: webservices.securetrading.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trust Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trust Payments, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trust Payments
provider_slug: trust-payments
slug: trust-payments-domain-security
source_filename: trust-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trustpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:29:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.trustpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:41:42 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: webservices.securetrading.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trustpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: securetrading.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trust-payments/refs/heads/main/security/trust-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- Tokenization
- Subscriptions
- 3-D Secure
- Point of Sale
- Webhooks
- Payouts
---
