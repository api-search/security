---
api_specs:
- filename: monero-daemon-rpc-openapi.json
  format: json
  label: Monero Daemon RPC API
  slug: monero-daemon-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-daemon-rpc-openapi.json
- filename: monero-wallet-rpc-openapi.json
  format: json
  label: Monero Wallet RPC API
  slug: monero-wallet-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/openapi/monero-wallet-rpc-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: getmonero.org
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.getmonero.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:00:28 2026 GMT
  host: docs.getmonero.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monero, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Monero
provider_slug: monero
slug: monero-domain-security
source_filename: monero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmonero.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.getmonero.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:00:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getmonero.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monero/refs/heads/main/security/monero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Cryptocurrency
- Privacy
- Blockchain
- JSON-RPC
- Wallet
- Mining
- Transactions
---
