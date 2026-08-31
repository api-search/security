---
api_specs:
- filename: metalend-ai-agent-guide-api-openapi.yml
  format: yaml
  label: MetaLend AI Agent Guide API
  slug: metalend-ai-agent-guide-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-ai-agent-guide-api-openapi.yml
- filename: metalend-auth-api-openapi.yml
  format: yaml
  label: MetaLend Auth API
  slug: metalend-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-auth-api-openapi.yml
- filename: metalend-balances-api-openapi.yml
  format: yaml
  label: MetaLend Balances API
  slug: metalend-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-balances-api-openapi.yml
- filename: metalend-deposits-api-openapi.yml
  format: yaml
  label: MetaLend Deposits API
  slug: metalend-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-deposits-api-openapi.yml
- filename: metalend-pools-api-openapi.yml
  format: yaml
  label: MetaLend Pools API
  slug: metalend-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-pools-api-openapi.yml
- filename: metalend-rewards-api-openapi.yml
  format: yaml
  label: MetaLend Rewards API
  slug: metalend-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-rewards-api-openapi.yml
- filename: metalend-services-api-openapi.yml
  format: yaml
  label: MetaLend Services API
  slug: metalend-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-services-api-openapi.yml
- filename: metalend-transaction-costs-api-openapi.yml
  format: yaml
  label: MetaLend Transaction Costs API
  slug: metalend-transaction-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-transaction-costs-api-openapi.yml
- filename: metalend-user-configuration-api-openapi.yml
  format: yaml
  label: MetaLend User Configuration API
  slug: metalend-user-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-user-configuration-api-openapi.yml
- filename: metalend-withdrawals-api-openapi.yml
  format: yaml
  label: MetaLend Withdrawals API
  slug: metalend-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/openapi/metalend-withdrawals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: metalend.tech
  spf: true
hosts:
- cert_expires: Sep  4 15:01:52 2026 GMT
  host: metalend.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:01:52 2026 GMT
  host: api.metalend.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metalend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetaLend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MetaLend
provider_slug: metalend
slug: metalend-domain-security
source_filename: metalend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metalend.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:01:52 2026 GMT\n  hsts: false\n- host: api.metalend.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:01:52 2026 GMT\n  hsts: null\ndomains:\n- domain: metalend.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metalend/refs/heads/main/security/metalend-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto
- DeFi
- Lending
- Yield
- Rebalancing
- Web3
- Stablecoins
- Payments
- Agent Native
- Blockchain
---
