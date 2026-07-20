---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: klasha.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: klasapps.com
  spf: false
hosts:
- cert_expires: Oct 13 01:50:05 2026 GMT
  host: www.klasha.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:17:11 2026 GMT
  host: developers.klasha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: gate.klasapps.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Klasha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klasha, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Klasha
provider_slug: klasha
slug: klasha-domain-security
source_filename: klasha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klasha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:50:05 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developers.klasha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gate.klasapps.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: klasha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: klasapps.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klasha/refs/heads/main/security/klasha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Africa
- Emerging Markets
- Mobile Money
- Payouts
- Foreign Exchange
- Virtual Accounts
- Checkout
- Financial Services
---
