---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 21market.kr
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: 21market.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 21 Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 21 Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 21 Market
provider_slug: 21-market
slug: 21-market-domain-security
source_filename: 21-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 21market.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 21market.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/21-market/refs/heads/main/security/21-market-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer Electronics
- Ecommerce
- Resale
- Secondhand
- Mobile Devices
- Trade-In
- South Korea
---
