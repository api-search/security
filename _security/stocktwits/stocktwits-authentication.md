---
api_key_in:
- query
api_specs:
- filename: stocktwits-account-api-openapi.yml
  format: yaml
  label: StockTwits Account API
  slug: stocktwits-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-account-api-openapi.yml
- filename: stocktwits-deletions-api-openapi.yml
  format: yaml
  label: StockTwits Deletions API
  slug: stocktwits-deletions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-deletions-api-openapi.yml
- filename: stocktwits-friendships-api-openapi.yml
  format: yaml
  label: StockTwits Friendships API
  slug: stocktwits-friendships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-friendships-api-openapi.yml
- filename: stocktwits-graph-social-api-openapi.yml
  format: yaml
  label: StockTwits Graph (Social) API
  slug: stocktwits-graph-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-graph-social-api-openapi.yml
- filename: stocktwits-messages-api-openapi.yml
  format: yaml
  label: StockTwits Messages API
  slug: stocktwits-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-messages-api-openapi.yml
- filename: stocktwits-search-api-openapi.yml
  format: yaml
  label: StockTwits Search API
  slug: stocktwits-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-search-api-openapi.yml
- filename: stocktwits-streams-api-openapi.yml
  format: yaml
  label: StockTwits Streams API
  slug: stocktwits-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-streams-api-openapi.yml
- filename: stocktwits-trending-api-openapi.yml
  format: yaml
  label: StockTwits Trending API
  slug: stocktwits-trending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-trending-api-openapi.yml
- filename: stocktwits-watchlists-api-openapi.yml
  format: yaml
  label: StockTwits Watchlists API
  slug: stocktwits-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/openapi/stocktwits-watchlists-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Stocktwits Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: StockTwits secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: StockTwits
provider_slug: stocktwits
scheme_count: 2
schemes:
- description: StockTwits uses OAuth 2.0 for authentication. Some endpoints are available without authentication using just an access_token query parameter.
  flows:
  - authorizationUrl: https://api.stocktwits.com/api/2/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api.stocktwits.com/api/2/oauth/token
  name: oauth2
  sources:
  - openapi/stocktwits-openapi-original.json
  type: oauth2
- description: Access token passed as a query parameter. Can be an application-level token for public endpoints or a user-level OAuth token for authenticated endpoints.
  in: query
  name: accessToken
  parameter: access_token
  sources:
  - openapi/stocktwits-openapi-original.json
  type: apiKey
slug: stocktwits-authentication
source_filename: stocktwits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/stocktwits-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.stocktwits.com/api/2/oauth/authorize\n    tokenUrl: https://api.stocktwits.com/api/2/oauth/token\n    scopes: 5\n  description: StockTwits uses OAuth 2.0 for authentication. Some endpoints are available without\n    authentication using just an access_token query parameter.\n  sources:\n  - openapi/stocktwits-openapi-original.json\n- name: accessToken\n  type: apiKey\n  in: query\n  parameter: access_token\n  description: Access token passed as a query parameter. Can be an application-level token for\n    public endpoints or a user-level OAuth token for authenticated endpoints.\n  sources:\n  - openapi/stocktwits-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stocktwits/refs/heads/main/authentication/stocktwits-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Fintech
- Social
- Stocks
- Trading
- Investing
- Market Data
- Social Finance
- Watchlist
- Messaging
---
