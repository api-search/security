---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beingjuice.com
  spf: false
hosts:
- cert_expires: Sep 16 04:58:27 2026 GMT
  host: beingjuice.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Being Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Being, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Being
provider_slug: being
slug: being-domain-security
source_filename: being-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beingjuice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:58:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beingjuice.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/being/refs/heads/main/security/being-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverages
- Juice
- Smoothies
- Cold-Pressed Juice
- Food and Beverage
- Consumer
- Retail
- Health and Wellness
- Malaysia
---
