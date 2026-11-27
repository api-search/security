---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: market0x.com
  spf: true
hosts:
- cert_expires: Jan  7 19:05:12 2027 GMT
  host: market0x.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Market0x Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Market0x, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Market0x
provider_slug: market0x-com
slug: market0x-com-domain-security
source_filename: market0x-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: market0x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:05:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: market0x.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/market0x-com/security/market0x-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- DeFi
- Blockchain
- Marketplace
- Non-Custodial
---
