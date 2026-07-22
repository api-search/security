---
api_specs:
- filename: sequence-indexer.json
  format: json
  label: Sequence Indexer API
  slug: sequence-indexer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-indexer.json
- filename: sequence-metadata.json
  format: json
  label: Sequence Metadata API
  slug: sequence-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-metadata.json
- filename: sequence-marketplace.json
  format: json
  label: Sequence Marketplace API
  slug: sequence-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-marketplace.json
- filename: sequence-transactions.json
  format: json
  label: Sequence Transactions (Relayer) API
  slug: sequence-transactions-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-transactions.json
- filename: sequence-analytics.json
  format: json
  label: Sequence Analytics API
  slug: sequence-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-analytics.json
- filename: sequence-builder.json
  format: json
  label: Sequence Builder API
  slug: sequence-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-builder.json
- filename: sequence-infrastructure.json
  format: json
  label: Sequence API (Infrastructure)
  slug: sequence-api-infrastructure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/openapi/sequence-infrastructure.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sequence.xyz
  spf: true
hosts:
- cert_expires: Sep 27 23:29:55 2026 GMT
  host: sequence.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sequence
provider_slug: sequence
slug: sequence-domain-security
source_filename: sequence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequence.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:29:55 2026 GMT\n  hsts: false\ndomains:\n- domain: sequence.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence/refs/heads/main/security/sequence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web3
- Blockchain
- Wallets
- Payments
- Crypto
- Indexer
- NFT
- Developer Platform
- Gaming
---
