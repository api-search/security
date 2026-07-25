---
api_specs:
- filename: fordefi-address-book-api-openapi.yml
  format: yaml
  label: Fordefi Address Book API
  slug: fordefi-address-book-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-address-book-api-openapi.yml
- filename: fordefi-assets-api-openapi.yml
  format: yaml
  label: Fordefi Assets API
  slug: fordefi-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-assets-api-openapi.yml
- filename: fordefi-audit-log-api-openapi.yml
  format: yaml
  label: Fordefi Audit Log API
  slug: fordefi-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-audit-log-api-openapi.yml
- filename: fordefi-authorization-tokens-api-openapi.yml
  format: yaml
  label: Fordefi Authorization Tokens API
  slug: fordefi-authorization-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-authorization-tokens-api-openapi.yml
- filename: fordefi-batch-transactions-api-openapi.yml
  format: yaml
  label: Fordefi Batch Transactions API
  slug: fordefi-batch-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-batch-transactions-api-openapi.yml
- filename: fordefi-blockchains-api-openapi.yml
  format: yaml
  label: Fordefi Blockchains API
  slug: fordefi-blockchains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-blockchains-api-openapi.yml
- filename: fordefi-enclave-keys-api-openapi.yml
  format: yaml
  label: Fordefi Enclave Keys API
  slug: fordefi-enclave-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-enclave-keys-api-openapi.yml
- filename: fordefi-end-users-api-openapi.yml
  format: yaml
  label: Fordefi End Users API
  slug: fordefi-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-end-users-api-openapi.yml
- filename: fordefi-exports-api-openapi.yml
  format: yaml
  label: Fordefi Exports API
  slug: fordefi-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-exports-api-openapi.yml
- filename: fordefi-organizations-api-openapi.yml
  format: yaml
  label: Fordefi Organizations API
  slug: fordefi-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-organizations-api-openapi.yml
- filename: fordefi-swaps-api-openapi.yml
  format: yaml
  label: Fordefi Swaps API
  slug: fordefi-swaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-swaps-api-openapi.yml
- filename: fordefi-transactions-api-openapi.yml
  format: yaml
  label: Fordefi Transactions API
  slug: fordefi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-transactions-api-openapi.yml
- filename: fordefi-user-groups-api-openapi.yml
  format: yaml
  label: Fordefi User Groups API
  slug: fordefi-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-user-groups-api-openapi.yml
- filename: fordefi-users-api-openapi.yml
  format: yaml
  label: Fordefi Users API
  slug: fordefi-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-users-api-openapi.yml
- filename: fordefi-vault-groups-api-openapi.yml
  format: yaml
  label: Fordefi Vault Groups API
  slug: fordefi-vault-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-vault-groups-api-openapi.yml
- filename: fordefi-vaults-api-openapi.yml
  format: yaml
  label: Fordefi Vaults API
  slug: fordefi-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-vaults-api-openapi.yml
- filename: fordefi-webhooks-api-openapi.yml
  format: yaml
  label: Fordefi Webhooks API
  slug: fordefi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fordefi.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: fordefi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.fordefi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fordefi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fordefi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fordefi
provider_slug: fordefi
slug: fordefi-domain-security
source_filename: fordefi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fordefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fordefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fordefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/security/fordefi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cryptocurrency
- Digital Assets
- Wallet
- Custody
- Blockchain
- DeFi
- MPC
- Payments
---
