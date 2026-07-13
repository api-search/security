---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blockscout.com
  spf: true
hosts:
- cert_expires: Sep  2 16:44:20 2026 GMT
  host: www.blockscout.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 16:44:20 2026 GMT
  host: docs.blockscout.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 16:44:20 2026 GMT
  host: eth.blockscout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockscout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockscout, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blockscout
provider_slug: blockscout
slug: blockscout-domain-security
source_filename: blockscout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blockscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:44:20 2026 GMT\n  hsts: null\n- host: docs.blockscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: eth.blockscout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockscout.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockscout/refs/heads/main/security/blockscout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Explorer
- Open Source
- EVM
- Multi-Chain
- GraphQL
- REST
- Etherscan-Compatible
---
