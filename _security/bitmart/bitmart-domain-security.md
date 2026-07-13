---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bitmart.com
  spf: true
hosts:
- cert_expires: Jan 30 01:46:09 2027 GMT
  host: developer-pro.bitmart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 01:46:09 2027 GMT
  host: api-cloud.bitmart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 01:46:09 2027 GMT
  host: ws-manager-compress.bitmart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitMart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BitMart
provider_slug: bitmart
slug: bitmart-domain-security
source_filename: bitmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer-pro.bitmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 01:46:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-cloud.bitmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 01:46:09 2027 GMT\n  hsts: null\n- host: ws-manager-compress.bitmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 01:46:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitmart.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmart/refs/heads/main/security/bitmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- Market Data
- Futures
---
