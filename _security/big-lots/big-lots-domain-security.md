---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biglots.com
  spf: true
hosts:
- cert_expires: Nov 10 19:48:43 2026 GMT
  host: www.biglots.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Big Lots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Lots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Big Lots
provider_slug: big-lots
slug: big-lots-domain-security
source_filename: big-lots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biglots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 19:48:43 2026 GMT\n  hsts: false\ndomains:\n- domain: biglots.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-lots/refs/heads/main/security/big-lots-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Discounts
- Consumer Goods
- E-Commerce
- Closeout
- Bankruptcy
- Fortune 500
---
