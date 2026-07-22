---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bayapay.com
  spf: false
hosts:
- cert_expires: Aug 15 14:54:33 2026 GMT
  host: bayapay.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bayapay Sdn Bhd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bayapay Sdn Bhd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bayapay Sdn Bhd
provider_slug: bayapay-sdn-bhd
slug: bayapay-sdn-bhd-domain-security
source_filename: bayapay-sdn-bhd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bayapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:54:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bayapay.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bayapay-sdn-bhd/refs/heads/main/security/bayapay-sdn-bhd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Fintech
- Prepaid Cards
- Expense Management
- Fleet
- Mastercard
- Malaysia
- APAC
---
