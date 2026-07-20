---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fawaterk.com
  spf: true
hosts:
- cert_expires: Aug 29 08:15:35 2026 GMT
  host: fawaterk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 20:31:14 2026 GMT
  host: app.fawaterk.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easypay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EasyPay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EasyPay
provider_slug: easypay
slug: easypay-domain-security
source_filename: easypay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fawaterk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:15:35 2026 GMT\n  hsts: false\n- host: app.fawaterk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: fawaterk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easypay/refs/heads/main/security/easypay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Gateway
- Invoicing
- Fintech
- E-commerce
- Egypt
- Online Payments
---
