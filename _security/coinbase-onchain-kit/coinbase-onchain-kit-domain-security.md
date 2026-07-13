---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: base.org
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Aug 24 08:27:22 2026 GMT
  host: www.base.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 03:32:48 2026 GMT
  host: docs.base.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinbase Onchain Kit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbase OnchainKit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Coinbase OnchainKit
provider_slug: coinbase-onchain-kit
slug: coinbase-onchain-kit-domain-security
source_filename: coinbase-onchain-kit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.base.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:27:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.base.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:32:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: base.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase-onchain-kit/refs/heads/main/security/coinbase-onchain-kit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Onchain
- Web3
- React
- SDK
- Base
- Smart Wallet
- Frames
- Mini Apps
---
