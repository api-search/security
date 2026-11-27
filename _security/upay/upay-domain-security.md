---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upay.co.il
  spf: true
hosts:
- cert_expires: Feb  9 23:11:51 2027 GMT
  host: upay.co.il
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Upay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upay
provider_slug: upay
slug: upay-domain-security
source_filename: upay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upay.co.il\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:11:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upay.co.il\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/upay/security/upay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Credit Cards
- Israel
- Merchant Services
---
