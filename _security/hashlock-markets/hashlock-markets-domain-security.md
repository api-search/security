---
api_specs:
- filename: hashlock-markets-assets-api-openapi.yml
  format: yaml
  label: Hashlock Markets Assets API
  slug: hashlock-markets-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-assets-api-openapi.yml
- filename: hashlock-markets-keys-api-openapi.yml
  format: yaml
  label: Hashlock Markets Keys API
  slug: hashlock-markets-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-keys-api-openapi.yml
- filename: hashlock-markets-me-api-openapi.yml
  format: yaml
  label: Hashlock Markets Me API
  slug: hashlock-markets-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-me-api-openapi.yml
- filename: hashlock-markets-rfqs-api-openapi.yml
  format: yaml
  label: Hashlock Markets Rfqs API
  slug: hashlock-markets-rfqs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-rfqs-api-openapi.yml
- filename: hashlock-markets-swaps-api-openapi.yml
  format: yaml
  label: Hashlock Markets Swaps API
  slug: hashlock-markets-swaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-swaps-api-openapi.yml
- filename: hashlock-markets-threads-api-openapi.yml
  format: yaml
  label: Hashlock Markets Threads API
  slug: hashlock-markets-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-threads-api-openapi.yml
- filename: hashlock-markets-tx-api-openapi.yml
  format: yaml
  label: Hashlock Markets Tx API
  slug: hashlock-markets-tx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-tx-api-openapi.yml
- filename: hashlock-markets-wallets-api-openapi.yml
  format: yaml
  label: Hashlock Markets Wallets API
  slug: hashlock-markets-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-wallets-api-openapi.yml
- filename: hashlock-markets-webhooks-api-openapi.yml
  format: yaml
  label: Hashlock Markets Webhooks API
  slug: hashlock-markets-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashlock-markets/openapi/hashlock-markets-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hashlock.markets
  spf: true
hosts:
- cert_expires: Jan 10 17:15:58 2027 GMT
  host: hashlock.markets
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hashlock Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hashlock Markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hashlock Markets
provider_slug: hashlock-markets
slug: hashlock-markets-domain-security
source_filename: hashlock-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hashlock.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 17:15:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hashlock.markets\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hashlock-markets/security/hashlock-markets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Cryptocurrency
- AtomicSwap
- Non-Custodial
- Cross-Chain
---
