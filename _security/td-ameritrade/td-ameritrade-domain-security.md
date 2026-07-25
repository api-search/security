---
api_specs:
- filename: td-ameritrade-instruments-api-openapi.yml
  format: yaml
  label: TD Ameritrade Instruments API
  slug: td-ameritrade-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-instruments-api-openapi.yml
- filename: td-ameritrade-authentication-api-openapi.yml
  format: yaml
  label: TD Ameritrade Authentication API
  slug: td-ameritrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-authentication-api-openapi.yml
- filename: td-ameritrade-accounts-and-trading-api-openapi.yml
  format: yaml
  label: TD Ameritrade Accounts and Trading API
  slug: td-ameritrade-accounts-and-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-accounts-and-trading-api-openapi.yml
- filename: td-ameritrade-authentication-api-openapi.yml
  format: yaml
  label: TD Ameritrade Authentication API
  slug: td-ameritrade-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-authentication-api-openapi.yml
- filename: td-ameritrade-instruments-api-openapi.yml
  format: yaml
  label: TD Ameritrade Instruments API
  slug: td-ameritrade-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-instruments-api-openapi.yml
- filename: td-ameritrade-market-hours-api-openapi.yml
  format: yaml
  label: TD Ameritrade Market Hours API
  slug: td-ameritrade-market-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-market-hours-api-openapi.yml
- filename: td-ameritrade-movers-api-openapi.yml
  format: yaml
  label: TD Ameritrade Movers API
  slug: td-ameritrade-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-movers-api-openapi.yml
- filename: td-ameritrade-option-chains-api-openapi.yml
  format: yaml
  label: TD Ameritrade Option Chains API
  slug: td-ameritrade-option-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-option-chains-api-openapi.yml
- filename: td-ameritrade-price-history-api-openapi.yml
  format: yaml
  label: TD Ameritrade Price History API
  slug: td-ameritrade-price-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-price-history-api-openapi.yml
- filename: td-ameritrade-quotes-api-openapi.yml
  format: yaml
  label: TD Ameritrade Quotes API
  slug: td-ameritrade-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-quotes-api-openapi.yml
- filename: td-ameritrade-transaction-history-api-openapi.yml
  format: yaml
  label: TD Ameritrade Transaction History API
  slug: td-ameritrade-transaction-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-transaction-history-api-openapi.yml
- filename: td-ameritrade-user-info-preferences-api-openapi.yml
  format: yaml
  label: TD Ameritrade User Info & Preferences API
  slug: td-ameritrade-user-info-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-user-info-preferences-api-openapi.yml
- filename: td-ameritrade-watchlist-api-openapi.yml
  format: yaml
  label: TD Ameritrade Watchlist API
  slug: td-ameritrade-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/openapi/td-ameritrade-watchlist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tdameritrade.com
  spf: true
hosts:
- host: developer.tdameritrade.com
  https: false
- host: api.tdameritrade.com
  https: false
- host: streamer-ws.tdameritrade.com
  https: false
kind: domain-security
layout: security
method: probed
name: Td Ameritrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TD Ameritrade, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TD Ameritrade
provider_slug: td-ameritrade
slug: td-ameritrade-domain-security
source_filename: td-ameritrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tdameritrade.com\n  https: false\n- host: api.tdameritrade.com\n  https: false\n- host: streamer-ws.tdameritrade.com\n  https: false\ndomains:\n- domain: tdameritrade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-ameritrade/refs/heads/main/security/td-ameritrade-domain-security.yml
summary_line: DMARC
tags:
- Brokerage
- Trading
- Finance
- Equities
- Options
- Market Data
- Streaming
---
