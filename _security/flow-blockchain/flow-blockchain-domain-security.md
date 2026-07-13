---
api_specs:
- filename: access.yaml
  format: yaml
  label: Flow Access REST API
  slug: flow-access-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/onflow/flow/master/openapi/access.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flow.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onflow.org
  spf: true
hosts:
- cert_expires: Sep 26 14:30:05 2026 GMT
  host: developers.flow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 12:20:54 2026 GMT
  host: rest-mainnet.onflow.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 16:45:40 2026 GMT
  host: rest-testnet.onflow.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flow Blockchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flow
provider_slug: flow-blockchain
slug: flow-blockchain-domain-security
source_filename: flow-blockchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.flow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:30:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rest-mainnet.onflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:20:54 2026 GMT\n  hsts: null\n- host: rest-testnet.onflow.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:45:40 2026 GMT\n  hsts: null\ndomains:\n- domain: flow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: onflow.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow-blockchain/refs/heads/main/security/flow-blockchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- NFTs
- Games
- DeFi
- Layer 1
- Cadence
- Smart Contracts
- Web3
---
