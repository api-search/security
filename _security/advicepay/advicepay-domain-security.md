---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: advicepay.com
  spf: true
hosts:
- cert_expires: Nov 16 03:01:30 2026 GMT
  host: advicepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: docs.advicepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: app.advicepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Advicepay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdvicePay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AdvicePay
provider_slug: advicepay
slug: advicepay-domain-security
source_filename: advicepay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advicepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 03:01:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.advicepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.advicepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: advicepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advicepay/refs/heads/main/security/advicepay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Payments
- Billing
- Invoicing
- Financial Planning
- Wealth Management
- Subscriptions
- eSignature
- Compliance
- FinTech
---
