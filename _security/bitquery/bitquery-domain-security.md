---
api_specs:
- filename: bitquery-asyncapi.yml
  format: yaml
  label: Bitquery Streaming Subscriptions
  slug: streaming-subscriptions
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitquery/refs/heads/main/asyncapi/bitquery-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitquery.io
  spf: true
hosts:
- cert_expires: Sep  9 09:05:54 2026 GMT
  host: bitquery.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 09:05:54 2026 GMT
  host: docs.bitquery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 09:07:00 2026 GMT
  host: streaming.bitquery.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitquery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitquery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitquery
provider_slug: bitquery
slug: bitquery-domain-security
source_filename: bitquery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:05:54 2026 GMT\n  hsts: false\n- host: docs.bitquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:05:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: streaming.bitquery.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:07:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitquery.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitquery/refs/heads/main/security/bitquery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain Data
- GraphQL
- Streaming
- Indexer
- DEX
- NFT
- Crypto
- Web3
---
