---
api_specs:
- filename: surf-dex-api-openapi.yml
  format: yaml
  label: Surf DEX API
  slug: surf-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-dex-api-openapi.yml
- filename: surf-exchange-api-openapi.yml
  format: yaml
  label: Surf Exchange API
  slug: surf-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-exchange-api-openapi.yml
- filename: surf-fund-api-openapi.yml
  format: yaml
  label: Surf Fund API
  slug: surf-fund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-fund-api-openapi.yml
- filename: surf-hyperliquid-api-openapi.yml
  format: yaml
  label: Surf Hyperliquid API
  slug: surf-hyperliquid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-hyperliquid-api-openapi.yml
- filename: surf-market-api-openapi.yml
  format: yaml
  label: Surf Market API
  slug: surf-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-market-api-openapi.yml
- filename: surf-news-api-openapi.yml
  format: yaml
  label: Surf News API
  slug: surf-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-news-api-openapi.yml
- filename: surf-onchain-api-openapi.yml
  format: yaml
  label: Surf Onchain API
  slug: surf-onchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-onchain-api-openapi.yml
- filename: surf-prediction-market-api-openapi.yml
  format: yaml
  label: Surf Prediction Market API
  slug: surf-prediction-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-prediction-market-api-openapi.yml
- filename: surf-project-api-openapi.yml
  format: yaml
  label: Surf Project API
  slug: surf-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-project-api-openapi.yml
- filename: surf-search-api-openapi.yml
  format: yaml
  label: Surf Search API
  slug: surf-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-search-api-openapi.yml
- filename: surf-signal-api-openapi.yml
  format: yaml
  label: Surf Signal API
  slug: surf-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-signal-api-openapi.yml
- filename: surf-social-api-openapi.yml
  format: yaml
  label: Surf Social API
  slug: surf-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-social-api-openapi.yml
- filename: surf-token-api-openapi.yml
  format: yaml
  label: Surf Token API
  slug: surf-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-token-api-openapi.yml
- filename: surf-wallet-api-openapi.yml
  format: yaml
  label: Surf Wallet API
  slug: surf-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-wallet-api-openapi.yml
- filename: surf-web-api-openapi.yml
  format: yaml
  label: Surf Web API
  slug: surf-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/openapi/surf-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asksurf.ai
  spf: true
hosts:
- cert_expires: Sep 11 17:36:51 2026 GMT
  host: asksurf.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 02:43:39 2026 GMT
  host: agents.asksurf.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.asksurf.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Surf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Surf, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Surf
provider_slug: surf
slug: surf-domain-security
source_filename: surf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asksurf.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:36:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: agents.asksurf.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.asksurf.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: asksurf.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surf/refs/heads/main/security/surf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- Market Data
- On-Chain Analytics
- Wallet Intelligence
- AI
- DeFi
- Prediction Markets
- Developer API
---
