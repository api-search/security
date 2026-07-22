---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: babylist.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: babylist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Babylist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BabyList, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BabyList
provider_slug: babylist
slug: babylist-domain-security
source_filename: babylist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babylist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: babylist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babylist/refs/heads/main/security/babylist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Baby Registry
- E-Commerce
- Retail
- Family
- Parenting
- Health
- Shopping
---
