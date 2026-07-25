---
api_specs:
- filename: blockstream-addresses-api-openapi.yml
  format: yaml
  label: Blockstream Addresses API
  slug: blockstream-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-addresses-api-openapi.yml
- filename: blockstream-assets-api-openapi.yml
  format: yaml
  label: Blockstream Assets API
  slug: blockstream-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-assets-api-openapi.yml
- filename: blockstream-blocks-api-openapi.yml
  format: yaml
  label: Blockstream Blocks API
  slug: blockstream-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-blocks-api-openapi.yml
- filename: blockstream-fee-estimates-api-openapi.yml
  format: yaml
  label: Blockstream Fee Estimates API
  slug: blockstream-fee-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-fee-estimates-api-openapi.yml
- filename: blockstream-mempool-api-openapi.yml
  format: yaml
  label: Blockstream Mempool API
  slug: blockstream-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-mempool-api-openapi.yml
- filename: blockstream-mining-api-openapi.yml
  format: yaml
  label: Blockstream Mining API
  slug: blockstream-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-mining-api-openapi.yml
- filename: blockstream-transactions-api-openapi.yml
  format: yaml
  label: Blockstream Transactions API
  slug: blockstream-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: blockstream.info
  spf: true
hosts:
- cert_expires: Oct  6 00:48:23 2026 GMT
  host: blockstream.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Blockstream
provider_slug: blockstream
slug: blockstream-domain-security
source_filename: blockstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockstream.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:48:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockstream.info\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/security/blockstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Bitcoin
- Blockchain
- Cryptocurrency
- Block Explorer
- Financial Services
- Infrastructure
---
