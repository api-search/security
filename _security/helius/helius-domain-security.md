---
api_specs:
- filename: helius-asyncapi.yml
  format: yaml
  label: Helius Solana RPC
  slug: rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/asyncapi/helius-asyncapi.yml
- filename: helius-addresses-api-openapi.yml
  format: yaml
  label: Helius Addresses API
  slug: helius-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-addresses-api-openapi.yml
- filename: helius-admin-api-openapi.yml
  format: yaml
  label: Helius Admin API
  slug: helius-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-admin-api-openapi.yml
- filename: helius-balances-api-openapi.yml
  format: yaml
  label: Helius Balances API
  slug: helius-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-balances-api-openapi.yml
- filename: helius-funding-api-openapi.yml
  format: yaml
  label: Helius Funding API
  slug: helius-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-funding-api-openapi.yml
- filename: helius-helius-api-catalog-api-openapi.yml
  format: yaml
  label: Helius Helius API Catalog API
  slug: helius-helius-api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-helius-api-catalog-api-openapi.yml
- filename: helius-history-api-openapi.yml
  format: yaml
  label: Helius History API
  slug: helius-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-history-api-openapi.yml
- filename: helius-identity-api-openapi.yml
  format: yaml
  label: Helius Identity API
  slug: helius-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-identity-api-openapi.yml
- filename: helius-nfts-api-openapi.yml
  format: yaml
  label: Helius NFTs API
  slug: helius-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-nfts-api-openapi.yml
- filename: helius-sender-api-openapi.yml
  format: yaml
  label: Helius Sender API
  slug: helius-sender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-sender-api-openapi.yml
- filename: helius-tokens-api-openapi.yml
  format: yaml
  label: Helius Tokens API
  slug: helius-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-tokens-api-openapi.yml
- filename: helius-transactions-api-openapi.yml
  format: yaml
  label: Helius Transactions API
  slug: helius-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-transactions-api-openapi.yml
- filename: helius-transfers-api-openapi.yml
  format: yaml
  label: Helius Transfers API
  slug: helius-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-transfers-api-openapi.yml
- filename: helius-webhooks-api-openapi.yml
  format: yaml
  label: Helius Webhooks API
  slug: helius-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/openapi/helius-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: helius.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: helius.xyz
  spf: true
hosts:
- cert_expires: Sep  4 07:05:23 2026 GMT
  host: www.helius.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 09:05:41 2026 GMT
  host: api.helius.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:59:43 2026 GMT
  host: laserstream-mainnet.helius-rpc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helius, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Helius
provider_slug: helius
slug: helius-domain-security
source_filename: helius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helius.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:05:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.helius.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:05:41 2026 GMT\n  hsts: null\n- host: laserstream-mainnet.helius-rpc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:59:43 2026 GMT\n  hsts: false\ndomains:\n- domain: helius.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: helius.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helius/refs/heads/main/security/helius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- Solana
- RPC
- DAS
- Streams
---
