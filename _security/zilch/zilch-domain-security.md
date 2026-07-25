---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zilch.com
  spf: true
hosts:
- cert_expires: Sep 14 07:13:04 2026 GMT
  host: www.zilch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zilch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zilch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zilch
provider_slug: zilch
slug: zilch-domain-security
source_filename: zilch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zilch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:13:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zilch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zilch/refs/heads/main/security/zilch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- BNPL
- Buy Now Pay Later
- Consumer Credit
- Digital Wallet
- Card
- Mastercard
- Fintech
---
