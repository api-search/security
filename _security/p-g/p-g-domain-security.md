---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pg.com
  spf: true
hosts:
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: developer.pg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: www.pg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: P G Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P&G, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: P&G
provider_slug: p-g
slug: p-g-domain-security
source_filename: p-g-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.pg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.pg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p-g/refs/heads/main/security/p-g-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Marketplace
- Consumer Goods
---
