---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konga.com
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: www.konga.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Konga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Konga
provider_slug: konga
slug: konga-domain-security
source_filename: konga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.konga.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: konga.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konga/refs/heads/main/security/konga-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Ecommerce
- Marketplace
- Retail
- Online Shopping
- Payments
- Fintech
- Mobile Money
- Wallet
- Pos
- Bill Payments
- Travel
- Flights
- Hotels
- Logistics
- Delivery
- Groceries
- Health
- Nigeria
- West Africa
- Africa
---
