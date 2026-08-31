---
api_specs:
- filename: superform-auxiliary-api-openapi.yml
  format: yaml
  label: Superform Auxiliary API
  slug: superform-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-auxiliary-api-openapi.yml
- filename: superform-balances-api-openapi.yml
  format: yaml
  label: Superform Balances API
  slug: superform-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-balances-api-openapi.yml
- filename: superform-contract-checker-api-openapi.yml
  format: yaml
  label: Superform Contract Checker API
  slug: superform-contract-checker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-contract-checker-api-openapi.yml
- filename: superform-data-api-openapi.yml
  format: yaml
  label: Superform Data API
  slug: superform-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-data-api-openapi.yml
- filename: superform-execution-api-openapi.yml
  format: yaml
  label: Superform Execution API
  slug: superform-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-execution-api-openapi.yml
- filename: superform-explorer-api-openapi.yml
  format: yaml
  label: Superform Explorer API
  slug: superform-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-explorer-api-openapi.yml
- filename: superform-health-api-openapi.yml
  format: yaml
  label: Superform Health API
  slug: superform-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-health-api-openapi.yml
- filename: superform-migrate-api-openapi.yml
  format: yaml
  label: Superform Migrate API
  slug: superform-migrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-migrate-api-openapi.yml
- filename: superform-protocol-api-openapi.yml
  format: yaml
  label: Superform Protocol API
  slug: superform-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-protocol-api-openapi.yml
- filename: superform-protocol-rewards-api-openapi.yml
  format: yaml
  label: Superform Protocol Rewards API
  slug: superform-protocol-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-protocol-rewards-api-openapi.yml
- filename: superform-simulator-api-openapi.yml
  format: yaml
  label: Superform Simulator API
  slug: superform-simulator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-simulator-api-openapi.yml
- filename: superform-stats-api-openapi.yml
  format: yaml
  label: Superform Stats API
  slug: superform-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-stats-api-openapi.yml
- filename: superform-superrewardsapi-api-openapi.yml
  format: yaml
  label: Superform SuperRewardsAPI API
  slug: superform-superrewardsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-superrewardsapi-api-openapi.yml
- filename: superform-token-distribution-api-openapi.yml
  format: yaml
  label: Superform Token Distribution API
  slug: superform-token-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-token-distribution-api-openapi.yml
- filename: superform-vault-api-openapi.yml
  format: yaml
  label: Superform Vault API
  slug: superform-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/openapi/superform-vault-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: superform.xyz
  spf: true
hosts:
- cert_expires: Oct 11 17:47:35 2026 GMT
  host: superform.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 09:00:03 2026 GMT
  host: api.superform.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Superform
provider_slug: superform
slug: superform-domain-security
source_filename: superform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superform.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superform.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:00:03 2026 GMT\n  hsts: null\ndomains:\n- domain: superform.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superform/refs/heads/main/security/superform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Defi Yield
- DeFi
- Vault
- Yield Aggregation
- Cross Chain
- Onchain
- Blockchain
- Smart Accounts
---
