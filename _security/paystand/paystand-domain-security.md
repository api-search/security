---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paystand.com
  spf: true
hosts:
- cert_expires: Sep 29 18:11:18 2026 GMT
  host: www.paystand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 08:35:39 2026 GMT
  host: developers.paystand.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 15:30:17 2026 GMT
  host: api.paystand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paystand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayStand, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PayStand
provider_slug: paystand
slug: paystand-domain-security
source_filename: paystand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paystand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:11:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.paystand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 08:35:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paystand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 15:30:17 2026 GMT\n  hsts: null\ndomains:\n- domain: paystand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystand/refs/heads/main/security/paystand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- B2B Payments
- Accounts Receivable
- Accounts Payable
- Fintech
- Blockchain
- ACH
- Billing
- Checkout
---
