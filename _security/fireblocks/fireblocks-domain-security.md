---
api_specs:
- filename: fireblocks-vaults-api-openapi.yml
  format: yaml
  label: Fireblocks Vaults API
  slug: fireblocks-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-vaults-api-openapi.yml
- filename: fireblocks-transactions-api-openapi.yml
  format: yaml
  label: Fireblocks Transactions API
  slug: fireblocks-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-transactions-api-openapi.yml
- filename: fireblocks-wallets-api-openapi.yml
  format: yaml
  label: Fireblocks Whitelisted Wallets API
  slug: fireblocks-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-wallets-api-openapi.yml
- filename: fireblocks-assets-api-openapi.yml
  format: yaml
  label: Fireblocks Blockchains and Assets API
  slug: fireblocks-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-assets-api-openapi.yml
- filename: fireblocks-exchange-api-openapi.yml
  format: yaml
  label: Fireblocks Exchange and Fiat Accounts API
  slug: fireblocks-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-exchange-api-openapi.yml
- filename: fireblocks-tokenization-api-openapi.yml
  format: yaml
  label: Fireblocks Tokenization API
  slug: fireblocks-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-tokenization-api-openapi.yml
- filename: fireblocks-contracts-api-openapi.yml
  format: yaml
  label: Fireblocks Smart Contracts API
  slug: fireblocks-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-contracts-api-openapi.yml
- filename: fireblocks-staking-api-openapi.yml
  format: yaml
  label: Fireblocks Staking API
  slug: fireblocks-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-staking-api-openapi.yml
- filename: fireblocks-nfts-api-openapi.yml
  format: yaml
  label: Fireblocks NFTs API
  slug: fireblocks-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-nfts-api-openapi.yml
- filename: fireblocks-payments-api-openapi.yml
  format: yaml
  label: Fireblocks Payments API
  slug: fireblocks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-payments-api-openapi.yml
- filename: fireblocks-network-api-openapi.yml
  format: yaml
  label: Fireblocks Network and Off-Exchange API
  slug: fireblocks-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-network-api-openapi.yml
- filename: fireblocks-compliance-api-openapi.yml
  format: yaml
  label: Fireblocks Compliance and Policy API
  slug: fireblocks-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-compliance-api-openapi.yml
- filename: fireblocks-gas-station-api-openapi.yml
  format: yaml
  label: Fireblocks Gas Station API
  slug: fireblocks-gas-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-gas-station-api-openapi.yml
- filename: fireblocks-workspace-api-openapi.yml
  format: yaml
  label: Fireblocks Workspace Management API
  slug: fireblocks-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-workspace-api-openapi.yml
- filename: fireblocks-webhooks-api-openapi.yml
  format: yaml
  label: Fireblocks Webhooks API
  slug: fireblocks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fireblocks.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fireblocks.io
  spf: true
hosts:
- cert_expires: Sep 15 01:26:05 2026 GMT
  host: www.fireblocks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 08:25:59 2026 GMT
  host: developers.fireblocks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 18:23:03 2026 GMT
  host: api.fireblocks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fireblocks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fireblocks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fireblocks
provider_slug: fireblocks
slug: fireblocks-domain-security
source_filename: fireblocks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fireblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:26:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.fireblocks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:25:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fireblocks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 18:23:03 2026 GMT\n  hsts: null\ndomains:\n- domain: fireblocks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fireblocks.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/security/fireblocks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
