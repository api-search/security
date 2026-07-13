---
api_specs:
- filename: zcash-cli.1
  format: yaml
  label: Zcash JSON-RPC API (zcashd)
  slug: zcash-json-rpc-api-zcashd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/zcash/zcash/master/doc/man/zcash-cli.1
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: lightwalletd.com
  spf: false
hosts:
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: zcash.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
- host: mainnet.lightwalletd.com
  https: false
kind: domain-security
layout: security
method: probed
name: Zcash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zcash, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zcash
provider_slug: zcash
slug: zcash-domain-security
source_filename: zcash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zcash.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\n- host: mainnet.lightwalletd.com\n  https: false\ndomains:\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: false\n  dmarc: false\n- domain: lightwalletd.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zcash/refs/heads/main/security/zcash-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Privacy
- Blockchain
- Zero-Knowledge Proofs
- Shielded Transactions
- ZEC
---
