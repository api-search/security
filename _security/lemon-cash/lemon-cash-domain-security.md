---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lemon.me
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mintlify.app
  spf: false
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: lemon.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 02:10:29 2026 GMT
  host: lemoncash.mintlify.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 05:00:19 2026 GMT
  host: www.lemon.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemon Cash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemon Cash, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lemon Cash
provider_slug: lemon-cash
slug: lemon-cash-domain-security
source_filename: lemon-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lemon.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lemoncash.mintlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:10:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.lemon.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lemon.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mintlify.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemon-cash/refs/heads/main/security/lemon-cash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Digital Wallet
- Fintech
- Payments
- Banking
- Blockchain
- Web3
- Argentina
- Latin America
- Mini Apps
- SDK
---
