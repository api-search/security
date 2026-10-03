---
api_specs:
- filename: babylon-labs-shared-api-openapi.yml
  format: yaml
  label: Babylon Labs Shared API
  slug: babylon-labs-shared-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-shared-api-openapi.yml
- filename: babylon-labs-apr-api-openapi.yml
  format: yaml
  label: Babylon Labs Apr API
  slug: babylon-labs-apr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-apr-api-openapi.yml
- filename: babylon-labs-delegation-api-openapi.yml
  format: yaml
  label: Babylon Labs Delegation API
  slug: babylon-labs-delegation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-delegation-api-openapi.yml
- filename: babylon-labs-delegations-api-openapi.yml
  format: yaml
  label: Babylon Labs Delegations API
  slug: babylon-labs-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-delegations-api-openapi.yml
- filename: babylon-labs-finality-providers-api-openapi.yml
  format: yaml
  label: Babylon Labs Finality Providers API
  slug: babylon-labs-finality-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-finality-providers-api-openapi.yml
- filename: babylon-labs-global-params-api-openapi.yml
  format: yaml
  label: Babylon Labs Global Params API
  slug: babylon-labs-global-params-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-global-params-api-openapi.yml
- filename: babylon-labs-network-info-api-openapi.yml
  format: yaml
  label: Babylon Labs Network Info API
  slug: babylon-labs-network-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-network-info-api-openapi.yml
- filename: babylon-labs-prices-api-openapi.yml
  format: yaml
  label: Babylon Labs Prices API
  slug: babylon-labs-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-prices-api-openapi.yml
- filename: babylon-labs-staker-api-openapi.yml
  format: yaml
  label: Babylon Labs Staker API
  slug: babylon-labs-staker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-staker-api-openapi.yml
- filename: babylon-labs-stats-api-openapi.yml
  format: yaml
  label: Babylon Labs Stats API
  slug: babylon-labs-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-stats-api-openapi.yml
- filename: babylon-labs-unbonding-api-openapi.yml
  format: yaml
  label: Babylon Labs Unbonding API
  slug: babylon-labs-unbonding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/openapi/babylon-labs-unbonding-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: babylonlabs.io
  spf: true
hosts:
- cert_expires: Aug 21 20:15:16 2026 GMT
  host: babylonlabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Babylon Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Babylon Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Babylon Labs
provider_slug: babylon-labs
slug: babylon-labs-domain-security
source_filename: babylon-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: babylonlabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 20:15:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: babylonlabs.io\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/babylon-labs/refs/heads/main/security/babylon-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Defi
- Bitcoin
- Bitcoin Staking
- Blockchain
- Cosmos
- Proof of Stake
- DeFi
- Staking
---
