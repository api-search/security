---
api_specs:
- filename: magic-eden-solana-openapi.yml
  format: yaml
  label: Magic Eden Solana API
  slug: solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-solana-openapi.yml
- filename: magic-eden-evm-openapi.yml
  format: yaml
  label: Magic Eden EVM API
  slug: evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-evm-openapi.yml
- filename: magic-eden-ordinals-openapi.yml
  format: yaml
  label: Magic Eden Bitcoin Ordinals & Runes API
  slug: ordinals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/openapi/magic-eden-ordinals-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magiceden.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: magiceden.dev
  spf: false
hosts:
- cert_expires: Oct  6 21:49:44 2026 GMT
  host: magiceden.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:13:29 2026 GMT
  host: docs.magiceden.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:07:19 2026 GMT
  host: api-mainnet.magiceden.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Eden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Eden, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Magic Eden
provider_slug: magic-eden
slug: magic-eden-domain-security
source_filename: magic-eden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magiceden.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:49:44 2026 GMT\n  hsts: false\n- host: docs.magiceden.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:13:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-mainnet.magiceden.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:07:19 2026 GMT\n  hsts: null\ndomains:\n- domain: magiceden.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: magiceden.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-eden/refs/heads/main/security/magic-eden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NFT
- Web3
- Blockchain
- Marketplace
- Solana
- Ethereum
- Bitcoin
- Ordinals
- Runes
- Multi-chain
---
