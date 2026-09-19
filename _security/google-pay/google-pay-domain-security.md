---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Nov  2 08:39:48 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:34 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:34 2026 GMT
  host: pay.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Pay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Pay
provider_slug: google-pay
slug: google-pay-domain-security
source_filename: google-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:39:48 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pay.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pay/refs/heads/main/security/google-pay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic Commerce
- Checkout
- Contactless Payments
- Digital Wallet
- Merchants
- Mobile Payments
- Payments
- Tokenization
---
