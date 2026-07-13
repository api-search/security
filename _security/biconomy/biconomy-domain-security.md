---
api_specs:
- filename: biconomy-supertransaction-api-openapi.yml
  format: yaml
  label: Biconomy Supertransaction API
  slug: biconomy-supertransaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/openapi/biconomy-supertransaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biconomy.io
  spf: true
hosts:
- cert_expires: Aug 16 21:13:15 2026 GMT
  host: www.biconomy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 16:06:44 2026 GMT
  host: docs.biconomy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 05:36:04 2026 GMT
  host: api.biconomy.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biconomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biconomy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Biconomy
provider_slug: biconomy
slug: biconomy-domain-security
source_filename: biconomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biconomy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 21:13:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.biconomy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:06:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.biconomy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:36:04 2026 GMT\n  hsts: null\ndomains:\n- domain: biconomy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biconomy/refs/heads/main/security/biconomy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account Abstraction
- Blockchain
- Bundler
- Cross-Chain
- DeFi
- ERC-4337
- ERC-7579
- ERC-7702
- Ethereum
- Gas Abstraction
- Gasless
- MEE
- Paymaster
- Smart Accounts
- Smart Sessions
- Wallets
- Web3
---
