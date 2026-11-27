---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: giftroam.com
  spf: true
hosts:
- cert_expires: Jan 15 06:15:23 2027 GMT
  host: giftroam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GiftRoam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GiftRoam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GiftRoam
provider_slug: giftroam-com
slug: giftroam-com-domain-security
source_filename: giftroam-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: giftroam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 06:15:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: giftroam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/giftroam-com/security/giftroam-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gifting
- E-Commerce
- International
---
