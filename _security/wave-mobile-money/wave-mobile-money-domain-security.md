---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wave.com
  spf: true
hosts:
- cert_expires: Sep 15 00:55:21 2026 GMT
  host: www.wave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:42:26 2026 GMT
  host: business.wave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 18:17:26 2026 GMT
  host: docs.wave.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wave Mobile Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wave Mobile Money, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wave Mobile Money
provider_slug: wave-mobile-money
slug: wave-mobile-money-domain-security
source_filename: wave-mobile-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:55:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: business.wave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:42:26 2026 GMT\n  hsts: false\n- host: docs.wave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:17:26 2026 GMT\n  hsts: null\ndomains:\n- domain: wave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wave-mobile-money/refs/heads/main/security/wave-mobile-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mobile Money
- Payments
- Fintech
- Financial Inclusion
- Africa
- West Africa
- Senegal
- Cote d'Ivoire
- Uganda
- Mali
- Burkina Faso
- Wallets
- Disbursements
- Checkout
- Payouts
- Money Transfer
---
