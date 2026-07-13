---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bravenewcoin.com
  spf: true
hosts:
- cert_expires: Sep 19 13:13:37 2026 GMT
  host: bravenewcoin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brave Newcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brave NewCoin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brave NewCoin
provider_slug: brave-newcoin
slug: brave-newcoin-domain-security
source_filename: brave-newcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bravenewcoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:13:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bravenewcoin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave-newcoin/refs/heads/main/security/brave-newcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
