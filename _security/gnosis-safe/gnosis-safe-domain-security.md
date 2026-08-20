---
api_specs:
- filename: gnosis-safe-4337-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) 4337 API
  slug: gnosis-safe-4337-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-4337-api-openapi.yml
- filename: gnosis-safe-about-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) about API
  slug: gnosis-safe-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-about-api-openapi.yml
- filename: gnosis-safe-analytics-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) analytics API
  slug: gnosis-safe-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-analytics-api-openapi.yml
- filename: gnosis-safe-contracts-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) contracts API
  slug: gnosis-safe-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-contracts-api-openapi.yml
- filename: gnosis-safe-data-decoder-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) data-decoder API
  slug: gnosis-safe-data-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-data-decoder-api-openapi.yml
- filename: gnosis-safe-delegates-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) delegates API
  slug: gnosis-safe-delegates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-delegates-api-openapi.yml
- filename: gnosis-safe-messages-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) messages API
  slug: gnosis-safe-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-messages-api-openapi.yml
- filename: gnosis-safe-modules-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) modules API
  slug: gnosis-safe-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-modules-api-openapi.yml
- filename: gnosis-safe-owners-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) owners API
  slug: gnosis-safe-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-owners-api-openapi.yml
- filename: gnosis-safe-safes-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) safes API
  slug: gnosis-safe-safes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-safes-api-openapi.yml
- filename: gnosis-safe-tokens-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) tokens API
  slug: gnosis-safe-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-tokens-api-openapi.yml
- filename: gnosis-safe-transactions-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) transactions API
  slug: gnosis-safe-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: safe.global
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: developer.safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gnosis Safe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safe (Gnosis Safe), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Safe (Gnosis Safe)
provider_slug: gnosis-safe
slug: gnosis-safe-domain-security
source_filename: gnosis-safe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: safe.global\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/security/gnosis-safe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Multisig
- Smart Contract
- Ethereum
- Web3
- Blockchain
- DeFi
- SAFe
- Gnosis
- Wallets
---
