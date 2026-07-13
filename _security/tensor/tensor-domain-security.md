---
api_specs:
- filename: tensor-api-openapi.yml
  format: yaml
  label: Tensor API
  slug: tensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-api-openapi.yml
- filename: tensor-tx-api-openapi.yml
  format: yaml
  label: Tensor Transaction API
  slug: tensor-tx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/openapi/tensor-tx-api-openapi.yml
- filename: tensor-websocket-api-asyncapi.yml
  format: yaml
  label: Tensor WebSocket API
  slug: tensor-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/asyncapi/tensor-websocket-api-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tensor.trade
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tensor.foundation
  spf: true
hosts:
- cert_expires: Aug  9 04:57:13 2026 GMT
  host: tensor.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:11:53 2026 GMT
  host: www.tensor.foundation
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:31:34 2026 GMT
  host: dev.tensor.trade
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tensor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tensor
provider_slug: tensor
slug: tensor-domain-security
source_filename: tensor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tensor.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 04:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.tensor.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:11:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.tensor.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: tensor.trade\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tensor.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensor/refs/heads/main/security/tensor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NFT
- Marketplace
- Solana
- Blockchain
- Web3
- Cryptocurrency
- Trading
- DAO
- DeFi
- AMM
---
