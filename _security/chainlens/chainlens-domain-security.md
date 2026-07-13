---
api_specs:
- filename: chainlens-openapi.yml
  format: yaml
  label: Chainlens Blockchain Explorer API
  slug: chainlens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chainlens/refs/heads/main/openapi/chainlens-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chainlens.com
  spf: false
hosts:
- cert_expires: Sep 29 04:24:46 2026 GMT
  host: www.chainlens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.chainlens.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chainlens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chainlens, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chainlens
provider_slug: chainlens
slug: chainlens-domain-security
source_filename: chainlens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chainlens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:24:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chainlens.com\n  https: false\ndomains:\n- domain: chainlens.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainlens/refs/heads/main/security/chainlens-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Analytics
- Blockchain
- Block Explorer
- Cryptocurrencies
- DeFi
- Ethereum
- EVM
- NFTs
- Smart Contracts
- Web3
---
