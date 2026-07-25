---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: limepay.com.au
  spf: true
hosts:
- cert_expires: Oct 16 11:01:10 2026 GMT
  host: www.limepay.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:21:11 2026 GMT
  host: docs.limepay.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limepay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limepay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Limepay
provider_slug: limepay
slug: limepay-domain-security
source_filename: limepay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.limepay.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:01:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.limepay.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:21:11 2026 GMT\n  hsts: false\ndomains:\n- domain: limepay.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limepay/refs/heads/main/security/limepay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- BNPL
- Payment Gateway
- Checkout
- Embedded Payments
- White Label
- Card Payments
- Marketplace
- Instalments
---
