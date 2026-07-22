---
api_specs:
- filename: thorchain-thornode-openapi.yaml
  format: yaml
  label: THORNode API
  slug: thornode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/openapi/thorchain-thornode-openapi.yaml
- filename: thorchain-midgard-openapi.json
  format: json
  label: Midgard API
  slug: midgard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/openapi/thorchain-midgard-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thorchain.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liquify.com
  spf: false
hosts:
- cert_expires: Oct 12 22:58:40 2026 GMT
  host: thorchain.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 22:58:40 2026 GMT
  host: dev.thorchain.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: gateway.liquify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thorchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for THORChain, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: THORChain
provider_slug: thorchain
slug: thorchain-domain-security
source_filename: thorchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thorchain.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: dev.thorchain.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: gateway.liquify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: thorchain.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: liquify.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thorchain/refs/heads/main/security/thorchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- DeFi
- Cross-chain
- Liquidity
- Decentralized Exchange
- Cosmos
- Web3 Infrastructure
---
