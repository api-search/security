---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: acala.network
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: aca-api.network
  spf: false
hosts:
- cert_expires: Sep  2 06:36:07 2026 GMT
  host: acala.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 01:37:35 2026 GMT
  host: evmdocs.acala.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: eth-rpc-acala.aca-api.network
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Acala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acala, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Acala
provider_slug: acala
slug: acala-domain-security
source_filename: acala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acala.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:36:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: evmdocs.acala.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:37:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eth-rpc-acala.aca-api.network\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: acala.network\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aca-api.network\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acala/refs/heads/main/security/acala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- DeFi
- Polkadot
- Smart Contracts
- EVM
- Stablecoin
- JSON-RPC
- Web3
---
