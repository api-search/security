---
api_specs:
- filename: dfns-auth-api-openapi.yml
  format: yaml
  label: Dfns Auth API
  slug: dfns-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-auth-api-openapi.yml
- filename: dfns-keys-api-openapi.yml
  format: yaml
  label: Dfns Keys API
  slug: dfns-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-keys-api-openapi.yml
- filename: dfns-networks-api-openapi.yml
  format: yaml
  label: Dfns Networks API
  slug: dfns-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-networks-api-openapi.yml
- filename: dfns-permissions-api-openapi.yml
  format: yaml
  label: Dfns Permissions API
  slug: dfns-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-permissions-api-openapi.yml
- filename: dfns-policies-api-openapi.yml
  format: yaml
  label: Dfns Policies API
  slug: dfns-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-policies-api-openapi.yml
- filename: dfns-wallets-api-openapi.yml
  format: yaml
  label: Dfns Wallets API
  slug: dfns-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-wallets-api-openapi.yml
- filename: dfns-webhooks-api-openapi.yml
  format: yaml
  label: Dfns Webhooks API
  slug: dfns-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-webhooks-api-openapi.yml
- filename: dfns-address-watches-api-openapi.yml
  format: yaml
  label: Dfns Address Watches API
  slug: dfns-address-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-address-watches-api-openapi.yml
- filename: dfns-agreements-api-openapi.yml
  format: yaml
  label: Dfns Agreements API
  slug: dfns-agreements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-agreements-api-openapi.yml
- filename: dfns-allocations-api-openapi.yml
  format: yaml
  label: Dfns Allocations API
  slug: dfns-allocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-allocations-api-openapi.yml
- filename: dfns-exchanges-api-openapi.yml
  format: yaml
  label: Dfns Exchanges API
  slug: dfns-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-exchanges-api-openapi.yml
- filename: dfns-fee-sponsors-api-openapi.yml
  format: yaml
  label: Dfns Fee Sponsors API
  slug: dfns-fee-sponsors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-fee-sponsors-api-openapi.yml
- filename: dfns-payins-api-openapi.yml
  format: yaml
  label: Dfns Payins API
  slug: dfns-payins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-payins-api-openapi.yml
- filename: dfns-payouts-api-openapi.yml
  format: yaml
  label: Dfns Payouts API
  slug: dfns-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-payouts-api-openapi.yml
- filename: dfns-signers-api-openapi.yml
  format: yaml
  label: Dfns Signers API
  slug: dfns-signers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-signers-api-openapi.yml
- filename: dfns-staking-api-openapi.yml
  format: yaml
  label: Dfns Staking API
  slug: dfns-staking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-staking-api-openapi.yml
- filename: dfns-swaps-api-openapi.yml
  format: yaml
  label: Dfns Swaps API
  slug: dfns-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-swaps-api-openapi.yml
- filename: dfns-tenant-api-openapi.yml
  format: yaml
  label: Dfns Tenant API
  slug: dfns-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-tenant-api-openapi.yml
- filename: dfns-vaults-api-openapi.yml
  format: yaml
  label: Dfns Vaults API
  slug: dfns-vaults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfns/openapi/dfns-vaults-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dfns.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dfns.io
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.dfns.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:55:59 2026 GMT
  host: docs.dfns.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: api.dfns.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dfns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dfns, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dfns
provider_slug: dfns
slug: dfns-domain-security
source_filename: dfns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dfns.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dfns.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dfns.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dfns.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dfns.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dfns/security/dfns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Wallets
- MPC
- Key Management
- Digital Assets
- Web3
- Non-Custodial
---
