---
api_specs:
- filename: openapi.yml
  format: yaml
  label: NEAR RPC API
  slug: near-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi.yml
- filename: fastnear-api.json
  format: json
  label: FASTNEAR Indexed REST API
  slug: fastnear-indexed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi/fastnear-api.json
- filename: nearblocks-api.json
  format: json
  label: NearBlocks Explorer API
  slug: nearblocks-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/openapi/nearblocks-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: near.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fastnear.com
  spf: false
hosts:
- cert_expires: Aug 21 10:07:37 2026 GMT
  host: docs.near.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 16:07:12 2026 GMT
  host: rpc.mainnet.near.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 01:03:50 2026 GMT
  host: docs.fastnear.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Near Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NEAR Protocol, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NEAR Protocol
provider_slug: near
slug: near-domain-security
source_filename: near-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.near.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:07:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.mainnet.near.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:07:12 2026 GMT\n  hsts: null\n- host: docs.fastnear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:03:50 2026 GMT\n  hsts: false\ndomains:\n- domain: near.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fastnear.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/near/refs/heads/main/security/near-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Web3
- NEAR
- NFT
- Tokens
- Staking
- Crypto
---
