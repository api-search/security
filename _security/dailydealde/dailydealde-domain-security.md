---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dailydeal.de
  spf: true
hosts:
- cert_expires: Aug 20 22:02:37 2026 GMT
  host: www.dailydeal.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dailydealde Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DailyDeal.de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DailyDeal.de
provider_slug: dailydealde
slug: dailydealde-domain-security
source_filename: dailydealde-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dailydeal.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:02:37 2026 GMT\n  hsts: false\ndomains:\n- domain: dailydeal.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailydealde/refs/heads/main/security/dailydealde-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deals
- Coupons
- Discounts
- E-Commerce
- Consumer
- Retail
- Vouchers
- Shopping
- Germany
---
