---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shieldpay.com
  spf: true
hosts:
- cert_expires: Sep  1 00:51:32 2026 GMT
  host: shieldpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 12:15:40 2026 GMT
  host: developers.shieldpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: api.partner.shieldpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shieldpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shieldpay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shieldpay
provider_slug: shieldpay
slug: shieldpay-domain-security
source_filename: shieldpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shieldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:51:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.shieldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:15:40 2026 GMT\n  hsts: null\n- host: api.partner.shieldpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shieldpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shieldpay/refs/heads/main/security/shieldpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Escrow
- Legal Technology
- Fintech
- Compliance
- KYC
- Banking
---
