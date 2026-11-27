---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tradingview-account-api-openapi.yml
  format: yaml
  label: TradingView Account API
  slug: tradingview-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-account-api-openapi.yml
- filename: tradingview-authorization-api-openapi.yml
  format: yaml
  label: TradingView Authorization API
  slug: tradingview-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-authorization-api-openapi.yml
- filename: tradingview-broker-configuration-api-openapi.yml
  format: yaml
  label: TradingView Broker Configuration API
  slug: tradingview-broker-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-broker-configuration-api-openapi.yml
- filename: tradingview-data-integration-api-openapi.yml
  format: yaml
  label: TradingView Data Integration API
  slug: tradingview-data-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-integration-api-openapi.yml
- filename: tradingview-data-permissions-api-openapi.yml
  format: yaml
  label: TradingView Data Permissions API
  slug: tradingview-data-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-permissions-api-openapi.yml
- filename: tradingview-market-data-api-openapi.yml
  format: yaml
  label: TradingView Market Data API
  slug: tradingview-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-market-data-api-openapi.yml
- filename: tradingview-trading-api-openapi.yml
  format: yaml
  label: TradingView Trading API
  slug: tradingview-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-trading-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: TradingView Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: TradingView secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: TradingView
provider_slug: tradingview
scheme_count: 4
schemes:
- bearerFormat: Bearer ACCESS_TOKEN
  description: 'This flow uses login and password to authenticate a user. Username and password are sent as parameters

    to the [/authorize](/rest-api-spec/#operation/authorize) endpoint.


    If the username and password are valid, then the broker issues an access token

    and returns it in the response. The access token is sent with every request in the Authorization header.'
  name: PasswordBearer
  scheme: bearer
  sources:
  - openapi/tradingview-broker-rest-api-openapi.yml
  type: http
- description: 'TradingView supports OAuth 2 Authorization Code flow (standard) and OAuth 2 Authorization Code flow with PKCE, as described in [RFC 6749](https://tools.ietf.org/html/rfc6749) and [RFC 7636](https://tools.ietf.org/html/rfc7636), respectively.

    After performing authorization, the access token is sent with every request in the `Authorization` header.


    **Code Flow:**


    For OAuth 2 Code Flow the broker p'
  flows:
  - authorizationUrl: https://your-rest-implementation.com/api/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://your-rest-implementation.com/api/oauth/token
  name: OAuth2Bearer
  sources:
  - openapi/tradingview-broker-rest-api-openapi.yml
  type: oauth2
- description: 'This authentication flow is used for server-to-server requests where authentication needs to be done without human intervention.

    It can be used with the [/history](#operation/getHistory), [/symbol_info](#operation/getSymbolInfo), [/streaming](#operation/streaming)

    and [/groups](#operation/getGroups) endpoints.


    JSON Web Token (JWT) is used to securely transmit information between broker and Tradin'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://your-rest-implementation.com/api/authorize/token
  name: ServerOAuth2Bearer
  sources:
  - openapi/tradingview-broker-rest-api-openapi.yml
  type: oauth2
- description: Authentication is OAuth 2.1 — you log in with your TradingView account, no API keys to manage.
  name: TradingView MCP OAuth 2.1
  sources:
  - https://www.tradingview.com/mcp/docs
  surface: https://mcp.tradingview.com/mcp
  type: oauth2
slug: tradingview-authentication
source_filename: tradingview-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: openapi/tradingview-broker-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: PasswordBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Bearer ACCESS_TOKEN\n  description: 'This flow uses login and password to authenticate a user. Username and password are sent as parameters\n\n    to the [/authorize](/rest-api-spec/#operation/authorize) endpoint.\n\n\n    If the username and password are valid, then the broker issues an access token\n\n    and returns it in the response. The access token is sent with every request in the Authorization header.'\n  sources:\n  - openapi/tradingview-broker-rest-api-openapi.yml\n- name: OAuth2Bearer\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-rest-implementation.com/api/authorize\n    tokenUrl: https://your-rest-implementation.com/api/oauth/token\n\
  \    scopes: 1\n  description: 'TradingView supports OAuth 2 Authorization Code flow (standard) and OAuth 2 Authorization Code flow with PKCE, as described in\n    [RFC 6749](https://tools.ietf.org/html/rfc6749) and [RFC 7636](https://tools.ietf.org/html/rfc7636), respectively.\n\n    After performing authorization, the access token is sent with every request in the `Authorization` header.\n\n\n    **Code Flow:**\n\n\n    For OAuth 2 Code Flow the broker p'\n  sources:\n  - openapi/tradingview-broker-rest-api-openapi.yml\n- name: ServerOAuth2Bearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-rest-implementation.com/api/authorize/token\n    scopes: 1\n  description: 'This authentication flow is used for server-to-server requests where authentication needs to be done without human intervention.\n\n    It can be used with the [/history](#operation/getHistory), [/symbol_info](#operation/getSymbolInfo), [/streaming](#operation/streaming)\n\n    and [/groups](#operation/getGroups)\
  \ endpoints.\n\n\n    JSON Web Token (JWT) is used to securely transmit information between broker and Tradin'\n  sources:\n  - openapi/tradingview-broker-rest-api-openapi.yml\n- name: TradingView MCP OAuth 2.1\n  type: oauth2\n  surface: https://mcp.tradingview.com/mcp\n  description: Authentication is OAuth 2.1 — you log in with your TradingView account, no API keys to manage.\n  sources:\n  - https://www.tradingview.com/mcp/docs\ndocs: https://www.tradingview.com/mcp/docs\nnote: Broker REST API schemes are implemented by the broker (TradingView authenticates to the broker). The MCP server scheme is TradingView-hosted.\n"
source_yaml_url: https://artifacts.apis.io/tradingview/authentication/tradingview-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Company
- Consumer
- Charts
- Charting Library
- Financial Data
- Market Data
- Widgets
- Trading
- Fintech
- Embeddable Components
---
