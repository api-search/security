---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kupivip.ru
  spf: true
hosts:
- cert_expires: Sep 21 11:01:20 2026 GMT
  host: www.kupivip.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kupivip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KupiVIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KupiVIP
provider_slug: kupivip
slug: kupivip-domain-security
source_filename: kupivip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kupivip.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 11:01:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kupivip.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kupivip/refs/heads/main/security/kupivip-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- E-Commerce
- Retail
- Fashion
- Apparel
- Luxury Goods
- Online Shopping
- Russia
---
