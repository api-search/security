---
api_specs:
- filename: tatum-openapi.yml
  format: yaml
  label: Tatum Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tatum/refs/heads/main/openapi/tatum-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tatum.io
  spf: true
hosts:
- cert_expires: Aug 16 17:48:21 2026 GMT
  host: tatum.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 11:05:18 2026 GMT
  host: docs.tatum.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 04:27:54 2026 GMT
  host: api.tatum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tatum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tatum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tatum
provider_slug: tatum
slug: tatum-domain-security
source_filename: tatum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tatum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:48:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tatum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tatum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:27:54 2026 GMT\n  hsts: null\ndomains:\n- domain: tatum.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tatum/refs/heads/main/security/tatum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- RPC
- Multi-chain
- Wallet
- NFT
---
