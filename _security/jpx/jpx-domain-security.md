---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jpx.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jpx-jquants.com
  spf: false
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: www.jpx.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: jpx-jquants.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.jquants.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jpx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JPX (Japan Exchange Group), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JPX (Japan Exchange Group)
provider_slug: jpx
slug: jpx-domain-security
source_filename: jpx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jpx.co.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jpx-jquants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jquants.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jpx.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jpx-jquants.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jpx/refs/heads/main/security/jpx-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Market Data
- Stocks
- Exchange
- Trading
- Derivatives
- Indices
- Reference Data
- Japan
---
