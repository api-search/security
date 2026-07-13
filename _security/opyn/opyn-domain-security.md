---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opyn.co
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Aug 13 04:13:48 2026 GMT
  host: www.opyn.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 16:26:23 2026 GMT
  host: squeeth.opyn.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:32:21 2026 GMT
  host: thegraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opyn, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Opyn
provider_slug: opyn
slug: opyn-domain-security
source_filename: opyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opyn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 04:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: squeeth.opyn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:26:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:32:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opyn.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opyn/refs/heads/main/security/opyn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Options
- Ethereum
- Squeeth
- Power Perpetual
- Derivatives
- Cryptocurrency
- Web3
- Smart Contracts
- Subgraph
- Crab Strategy
- Vault
---
