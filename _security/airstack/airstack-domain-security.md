---
api_specs:
- filename: farcaster-hub-rest-api.json
  format: json
  label: Airstack Farcaster Hub API
  slug: airstack-farcaster-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-hub-rest-api.json
- filename: farcaster-webhooks-api.json
  format: json
  label: Airstack Farcaster Webhooks API
  slug: airstack-farcaster-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/openapi/farcaster-webhooks-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: airstack.xyz
  spf: true
hosts:
- cert_expires: Sep 21 13:44:22 2026 GMT
  host: docs.airstack.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 11:52:31 2026 GMT
  host: api.airstack.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:02:27 2026 GMT
  host: hubs.airstack.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airstack, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Airstack
provider_slug: airstack
slug: airstack-domain-security
source_filename: airstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.airstack.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:44:22 2026 GMT\n  hsts: null\n- host: api.airstack.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:52:31 2026 GMT\n  hsts: null\n- host: hubs.airstack.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:02:27 2026 GMT\n  hsts: null\ndomains:\n- domain: airstack.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airstack/refs/heads/main/security/airstack-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- GraphQL
- NFT
- Tokens
- On-Chain Data
- Ethereum
- Polygon
- Base
- ENS
- POAP
- Social Graph
- Wallet
- Identity
---
