---
api_key_in: []
api_specs:
- filename: sp-global-auditors-api-openapi.yml
  format: yaml
  label: S&P Global LLM-Ready API (kFinance)
  slug: kensho-llm-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-auditors-api-openapi.yml
- filename: sp-global-extractions-api-openapi.yml
  format: yaml
  label: Kensho Extract API
  slug: kensho-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-extractions-api-openapi.yml
- filename: sp-global-annotations-async-api-openapi.yml
  format: yaml
  label: Kensho NERD API
  slug: kensho-nerd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-annotations-async-api-openapi.yml
- filename: sp-global-transcription-api-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v2
  slug: kensho-scribe-batch-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-transcription-api-openapi.yml
- filename: kensho-scribe-realtime-asyncapi.yml
  format: yaml
  label: Kensho Scribe Real Time API
  slug: kensho-scribe-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/asyncapi/kensho-scribe-realtime-asyncapi.yml
- filename: sp-global-transcription-api-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v1
  slug: kensho-scribe-batch-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-transcription-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Sp Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: S&P Global secures its APIs with http, oauth2, and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: S&P Global
provider_slug: sp-global
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sp-global-annotations-async-api-openapi.yml
  - openapi/sp-global-auditors-api-openapi.yml
  - openapi/sp-global-ciqpro-api-openapi.yml
  - openapi/sp-global-company-groups-api-openapi.yml
  - openapi/sp-global-competitors-api-openapi.yml
  - openapi/sp-global-cusip-api-openapi.yml
  - openapi/sp-global-earnings-api-openapi.yml
  - openapi/sp-global-estimates-api-openapi.yml
  - openapi/sp-global-extractions-api-openapi.yml
  - openapi/sp-global-fundinground-api-openapi.yml
  - openapi/sp-global-fundingrounds-api-openapi.yml
  - openapi/sp-global-id-api-openapi.yml
  - openapi/sp-global-ids-api-openapi.yml
  - openapi/sp-global-info-api-openapi.yml
  - openapi/sp-global-isin-api-openapi.yml
  - openapi/sp-global-latest-api-openapi.yml
  - openapi/sp-global-line-item-api-openapi.yml
  - openapi/sp-global-market-cap-api-openapi.yml
  - openapi/sp-global-merger-api-openapi.yml
  - openapi/sp-global-mergers-api-openapi.yml
  - openapi/sp-global-price-chart-api-openapi.yml
  - openapi/sp-global-pricing-api-openapi.yml
  - openapi/sp-global-relationship-api-openapi.yml
  - openapi/sp-global-securities-api-openapi.yml
  - openapi/sp-global-segments-api-openapi.yml
  - openapi/sp-global-statements-api-openapi.yml
  - openapi/sp-global-ticker-groups-api-openapi.yml
  - openapi/sp-global-trading-item-groups-api-openapi.yml
  - openapi/sp-global-trading-items-api-openapi.yml
  - openapi/sp-global-transcript-api-openapi.yml
  - openapi/sp-global-transcription-api-openapi.yml
  - openapi/sp-global-upload-url-api-openapi.yml
  - openapi/sp-global-user-info-api-openapi.yml
  - openapi/sp-global-users-api-openapi.yml
  type: http
slug: sp-global-authentication
source_filename: sp-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\ndocs: https://docs.kensho.com/authentication\nsource: openapi/sp-global-annotations-async-api-openapi.yml, openapi/sp-global-auditors-api-openapi.yml,\n  openapi/sp-global-ciqpro-api-openapi.yml, openapi/sp-global-company-groups-api-openapi.yml,\n  openapi/sp-global-competitors-api-openapi.yml, openapi/sp-global-cusip-api-openapi.yml, openapi/sp-global-earnings-api-openapi.yml,\n  openapi/sp-global-estimates-api-openapi.yml, openapi/sp-global-extractions-api-openapi.yml,\n  openapi/sp-global-fundinground-api-openapi.yml, openapi/sp-global-fundingrounds-api-openapi.yml,\n  openapi/sp-global-id-api-openapi.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\noidc:\n  # Searched: docs.kensho.com/authentication + live RFC 8414/9728 metadata on kfinance.kensho.com\n  model: OpenID Connect on OAuth 2.0; all Kensho APIs accept the resulting JWT as a Bearer token\n  methods:\n    - name: keypair\n      use: production (server-to-server,\
  \ long-term unattended)\n      docs: https://docs.kensho.com/authentication/keypair\n    - name: refresh-token\n      use: development/testing; tokens expire after 7 days\n      docs: https://docs.kensho.com/authentication/personal-token\n  authorization_server:\n    issuer: https://kfinance.kensho.com/integrations\n    authorizationUrl: https://kfinance.kensho.com/integrations/authorize\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n    registration: https://kfinance.kensho.com/integrations/register\n    pkce: S256\n    metadata: well-known/sp-global-oauth-authorization-server.json\n  scopes: scopes/sp-global-scopes.yml\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/sp-global-annotations-async-api-openapi.yml\n  - openapi/sp-global-auditors-api-openapi.yml\n  - openapi/sp-global-ciqpro-api-openapi.yml\n  - openapi/sp-global-company-groups-api-openapi.yml\n  - openapi/sp-global-competitors-api-openapi.yml\n  -\
  \ openapi/sp-global-cusip-api-openapi.yml\n  - openapi/sp-global-earnings-api-openapi.yml\n  - openapi/sp-global-estimates-api-openapi.yml\n  - openapi/sp-global-extractions-api-openapi.yml\n  - openapi/sp-global-fundinground-api-openapi.yml\n  - openapi/sp-global-fundingrounds-api-openapi.yml\n  - openapi/sp-global-id-api-openapi.yml\n  - openapi/sp-global-ids-api-openapi.yml\n  - openapi/sp-global-info-api-openapi.yml\n  - openapi/sp-global-isin-api-openapi.yml\n  - openapi/sp-global-latest-api-openapi.yml\n  - openapi/sp-global-line-item-api-openapi.yml\n  - openapi/sp-global-market-cap-api-openapi.yml\n  - openapi/sp-global-merger-api-openapi.yml\n  - openapi/sp-global-mergers-api-openapi.yml\n  - openapi/sp-global-price-chart-api-openapi.yml\n  - openapi/sp-global-pricing-api-openapi.yml\n  - openapi/sp-global-relationship-api-openapi.yml\n  - openapi/sp-global-securities-api-openapi.yml\n  - openapi/sp-global-segments-api-openapi.yml\n  - openapi/sp-global-statements-api-openapi.yml\n\
  \  - openapi/sp-global-ticker-groups-api-openapi.yml\n  - openapi/sp-global-trading-item-groups-api-openapi.yml\n  - openapi/sp-global-trading-items-api-openapi.yml\n  - openapi/sp-global-transcript-api-openapi.yml\n  - openapi/sp-global-transcription-api-openapi.yml\n  - openapi/sp-global-upload-url-api-openapi.yml\n  - openapi/sp-global-user-info-api-openapi.yml\n  - openapi/sp-global-users-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/authentication/sp-global-authentication.yml
summary_line: http/oauth2/openIdConnect · 1 scheme
tags:
- Capital IQ
- Commodity Insights
- Credit Ratings
- Document Extraction
- ESG
- Financial Data
- Index Data
- LLM
- MCP
- Market Intelligence
- Mobility
- Named Entity Recognition
- Speech to Text
---
