---
api_specs:
- filename: origin-protocol-account-api-openapi.yml
  format: yaml
  label: Origin Protocol account API
  slug: origin-protocol-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-account-api-openapi.yml
- filename: origin-protocol-arm-api-openapi.yml
  format: yaml
  label: Origin Protocol arm API
  slug: origin-protocol-arm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-arm-api-openapi.yml
- filename: origin-protocol-beacon-chain-api-openapi.yml
  format: yaml
  label: Origin Protocol beacon-chain API
  slug: origin-protocol-beacon-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-beacon-chain-api-openapi.yml
- filename: origin-protocol-cache-api-openapi.yml
  format: yaml
  label: Origin Protocol cache API
  slug: origin-protocol-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-cache-api-openapi.yml
- filename: origin-protocol-coingecko-api-openapi.yml
  format: yaml
  label: Origin Protocol coingecko API
  slug: origin-protocol-coingecko-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-coingecko-api-openapi.yml
- filename: origin-protocol-defillama-api-openapi.yml
  format: yaml
  label: Origin Protocol defillama API
  slug: origin-protocol-defillama-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-defillama-api-openapi.yml
- filename: origin-protocol-dune-api-openapi.yml
  format: yaml
  label: Origin Protocol dune API
  slug: origin-protocol-dune-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-dune-api-openapi.yml
- filename: origin-protocol-hyperliquid-api-openapi.yml
  format: yaml
  label: Origin Protocol hyperliquid API
  slug: origin-protocol-hyperliquid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-hyperliquid-api-openapi.yml
- filename: origin-protocol-merkl-api-openapi.yml
  format: yaml
  label: Origin Protocol merkl API
  slug: origin-protocol-merkl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-merkl-api-openapi.yml
- filename: origin-protocol-oeth-api-openapi.yml
  format: yaml
  label: Origin Protocol oeth API
  slug: origin-protocol-oeth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-oeth-api-openapi.yml
- filename: origin-protocol-ofac-api-openapi.yml
  format: yaml
  label: Origin Protocol ofac API
  slug: origin-protocol-ofac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-ofac-api-openapi.yml
- filename: origin-protocol-ogn-api-openapi.yml
  format: yaml
  label: Origin Protocol ogn API
  slug: origin-protocol-ogn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-ogn-api-openapi.yml
- filename: origin-protocol-protocol-api-openapi.yml
  format: yaml
  label: Origin Protocol protocol API
  slug: origin-protocol-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-protocol-api-openapi.yml
- filename: origin-protocol-reports-api-openapi.yml
  format: yaml
  label: Origin Protocol reports API
  slug: origin-protocol-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-reports-api-openapi.yml
- filename: origin-protocol-strapi-api-openapi.yml
  format: yaml
  label: Origin Protocol strapi API
  slug: origin-protocol-strapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-strapi-api-openapi.yml
- filename: origin-protocol-supply-api-openapi.yml
  format: yaml
  label: Origin Protocol supply API
  slug: origin-protocol-supply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-supply-api-openapi.yml
- filename: origin-protocol-token-api-openapi.yml
  format: yaml
  label: Origin Protocol token API
  slug: origin-protocol-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/openapi/origin-protocol-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: originprotocol.com
  spf: false
hosts:
- cert_expires: Sep 18 09:15:48 2026 GMT
  host: www.originprotocol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Origin Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Origin Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Origin Protocol
provider_slug: origin-protocol
slug: origin-protocol-domain-security
source_filename: origin-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.originprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 09:15:48 2026 GMT\n  hsts: false\ndomains:\n- domain: originprotocol.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin-protocol/refs/heads/main/security/origin-protocol-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto
- DeFi
- Analytics
- Ethereum
- Stablecoin
- Liquid Staking
- Yield
- Blockchain
---
