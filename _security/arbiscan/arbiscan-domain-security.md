---
api_specs:
- filename: arbiscan-accounts-api-openapi.yml
  format: yaml
  label: Arbiscan Accounts API
  slug: arbiscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-accounts-api-openapi.yml
- filename: arbiscan-blocks-api-openapi.yml
  format: yaml
  label: Arbiscan Blocks API
  slug: arbiscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-blocks-api-openapi.yml
- filename: arbiscan-contracts-api-openapi.yml
  format: yaml
  label: Arbiscan Contracts API
  slug: arbiscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-contracts-api-openapi.yml
- filename: arbiscan-gas-tracker-api-openapi.yml
  format: yaml
  label: Arbiscan Gas Tracker API
  slug: arbiscan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-gas-tracker-api-openapi.yml
- filename: arbiscan-logs-api-openapi.yml
  format: yaml
  label: Arbiscan Logs API
  slug: arbiscan-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-logs-api-openapi.yml
- filename: arbiscan-stats-api-openapi.yml
  format: yaml
  label: Arbiscan Stats API
  slug: arbiscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-stats-api-openapi.yml
- filename: arbiscan-tokens-api-openapi.yml
  format: yaml
  label: Arbiscan Tokens API
  slug: arbiscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-tokens-api-openapi.yml
- filename: arbiscan-transactions-api-openapi.yml
  format: yaml
  label: Arbiscan Transactions API
  slug: arbiscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: arbiscan.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: etherscan.io
  spf: true
hosts:
- cert_expires: Aug 26 02:02:03 2026 GMT
  host: arbiscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 02:02:03 2026 GMT
  host: docs.arbiscan.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arbiscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbiscan, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Arbiscan
provider_slug: arbiscan
slug: arbiscan-domain-security
source_filename: arbiscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbiscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:02:03 2026 GMT\n  hsts: false\n- host: docs.arbiscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: arbiscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: etherscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/security/arbiscan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Arbitrum
- Layer 2
- EVM
- Web3
- L2
---
