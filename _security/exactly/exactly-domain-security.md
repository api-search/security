---
api_specs:
- filename: exactly-erc-4626-api-openapi.yml
  format: yaml
  label: Exactly Protocol ERC-4626 API
  slug: exactly-erc-4626-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-erc-4626-api-openapi.yml
- filename: exactly-fixed-rate-api-openapi.yml
  format: yaml
  label: Exactly Protocol Fixed Rate API
  slug: exactly-fixed-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-fixed-rate-api-openapi.yml
- filename: exactly-liquidations-api-openapi.yml
  format: yaml
  label: Exactly Protocol Liquidations API
  slug: exactly-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-liquidations-api-openapi.yml
- filename: exactly-liquidity-api-openapi.yml
  format: yaml
  label: Exactly Protocol Liquidity API
  slug: exactly-liquidity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-liquidity-api-openapi.yml
- filename: exactly-market-management-api-openapi.yml
  format: yaml
  label: Exactly Protocol Market Management API
  slug: exactly-market-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-market-management-api-openapi.yml
- filename: exactly-market-state-api-openapi.yml
  format: yaml
  label: Exactly Protocol Market State API
  slug: exactly-market-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-market-state-api-openapi.yml
- filename: exactly-markets-api-openapi.yml
  format: yaml
  label: Exactly Protocol Markets API
  slug: exactly-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-markets-api-openapi.yml
- filename: exactly-previewer-api-openapi.yml
  format: yaml
  label: Exactly Protocol Previewer API
  slug: exactly-previewer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-previewer-api-openapi.yml
- filename: exactly-reward-configuration-api-openapi.yml
  format: yaml
  label: Exactly Protocol Reward Configuration API
  slug: exactly-reward-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-reward-configuration-api-openapi.yml
- filename: exactly-rewards-claims-api-openapi.yml
  format: yaml
  label: Exactly Protocol Rewards Claims API
  slug: exactly-rewards-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-rewards-claims-api-openapi.yml
- filename: exactly-rewards-query-api-openapi.yml
  format: yaml
  label: Exactly Protocol Rewards Query API
  slug: exactly-rewards-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-rewards-query-api-openapi.yml
- filename: exactly-variable-rate-api-openapi.yml
  format: yaml
  label: Exactly Protocol Variable Rate API
  slug: exactly-variable-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/openapi/exactly-variable-rate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exact.ly
  spf: true
hosts:
- cert_expires: Sep 13 16:43:41 2026 GMT
  host: exact.ly
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 22:03:36 2026 GMT
  host: docs.exact.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 12:09:16 2026 GMT
  host: app.exact.ly
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exactly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exactly Protocol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Exactly Protocol
provider_slug: exactly
slug: exactly-domain-security
source_filename: exactly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 22:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.exact.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:09:16 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: exact.ly\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exactly/refs/heads/main/security/exactly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DeFi
- Lending
- Borrowing
- Fixed Rate
- Variable Rate
- Ethereum
- Optimism
- Base
- ERC-4626
- Credit Markets
---
