---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: payform.me
  spf: true
hosts:
- cert_expires: Oct 14 21:45:00 2026 GMT
  host: payform.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Payform
provider_slug: payform
slug: payform-domain-security
source_filename: payform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payform.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:45:00 2026 GMT\n  hsts: false\ndomains:\n- domain: payform.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payform/refs/heads/main/security/payform-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Payment Forms
- No-Code
- Recurring Billing
- Subscriptions
- Checkout
- Digital Content
- SaaS
---
