---
api_key_in: []
api_specs:
- filename: alltick-api-quote-b-api-api-openapi.yml
  format: yaml
  label: AllTick API Quote B API
  slug: alltick-api-quote-b-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/openapi/alltick-api-quote-b-api-api-openapi.yml
- filename: alltick-api-quote-stock-b-api-api-openapi.yml
  format: yaml
  label: AllTick API Quote Stock B API
  slug: alltick-api-quote-stock-b-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/openapi/alltick-api-quote-stock-b-api-api-openapi.yml
- filename: alltick-api-suspension-api-openapi.yml
  format: yaml
  label: AllTick API Suspension API
  slug: alltick-api-suspension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/openapi/alltick-api-suspension-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Alltick Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: AllTick API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AllTick API
provider_slug: alltick-api
scheme_count: 1
schemes:
- applies_to:
  - https://quote.alltick.co/quote-stock-b-api/*
  - https://quote.alltick.co/quote-b-api/*
  - https://quote.alltick.co/api/suspension/*
  - wss://quote.alltick.co/quote-stock-b-ws-api
  - wss://quote.alltick.co/quote-b-ws-api
  example_form: https://quote.alltick.co/quote-stock-b-api/kline?token=yourToken&query=queryData
  expiry: tied to subscription validity — an expired account yields ret 401 "token invalid"
  format: opaque string; no documented prefix, length or structure
  id: token
  in: query
  name: token
  required: true
  rotation: not documented
  type: apiKey
  websocket_form: wss://quote.alltick.co/quote-stock-b-ws-api?token=yourToken
slug: alltick-api-authentication
source_filename: alltick-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: searched\nsource: >-\n  https://en.apis.alltick.co/integration-process/token-application +\n  https://en.apis.alltick.co/integration-process/market-address-description/http-quotes-api-address-description +\n  https://en.apis.alltick.co/integration-process/market-address-description/websocket-quotes-api-address-description +\n  openapi/alltick-api-openapi.json\ndocs: https://en.apis.alltick.co/integration-process/token-application\nchecked: '2026-08-18'\nsummary: >-\n  One credential, one mechanism, everywhere: a single opaque account token passed as the `token`\n  QUERY STRING parameter, on both the HTTPS endpoints and the WebSocket handshake URL. There is no\n  OAuth, no OIDC, no mTLS, no signing, no header-based key, no per-key scoping and no documented\n  rotation or expiry story beyond \"the token expires when the account does\". Entitlement is carried\n  by the token itself: which symbols and which markets you may read is a property of\
  \ the plan the\n  token belongs to (errors 604 `code unauthorized` and 603 `token level not enough`).\nschemes:\n  - id: token\n    type: apiKey\n    in: query\n    name: token\n    required: true\n    applies_to:\n      - https://quote.alltick.co/quote-stock-b-api/*\n      - https://quote.alltick.co/quote-b-api/*\n      - https://quote.alltick.co/api/suspension/*\n      - wss://quote.alltick.co/quote-stock-b-ws-api\n      - wss://quote.alltick.co/quote-b-ws-api\n    example_form: https://quote.alltick.co/quote-stock-b-api/kline?token=yourToken&query=queryData\n    websocket_form: wss://quote.alltick.co/quote-stock-b-ws-api?token=yourToken\n    format: opaque string; no documented prefix, length or structure\n    rotation: not documented\n    expiry: tied to subscription validity — an expired account yields ret 401 \"token invalid\"\nissuance:\n  self_serve: true\n  steps:\n    - Register at https://alltick.co/register with an email address and password.\n    - Confirm the emailed verification\
  \ code.\n    - On success you land in the dashboard.\n    - Read the token from the dashboard \"API keys\" section.\n  url: https://alltick.co/register\n  approval_required: false\n  note: AllTick's FAQ states registration includes a one-week free trial.\nmissing_from_spec:\n  components_securitySchemes: false\n  root_security: false\n  note: >-\n    openapi/alltick-api-openapi.json has NO components.securitySchemes block and NO top-level\n    `security` requirement. The token appears only as an ordinary required query parameter on each\n    operation, carrying the literal default value \"YOUR_TOKEN_HERE\". A generator reading this spec\n    produces a client with no auth concept at all. Adding an `apiKey`/`in: query` scheme and applying\n    it globally is a one-block fix.\ncredential_exposure:\n  concern: >-\n    Passing a long-lived bearer credential in the query string, on both HTTP and the WebSocket URL,\n    puts it in proxy logs, browser history, Referer headers and server access\
  \ logs. AllTick's own\n    guidance is limited to \"keep your token secure and avoid sharing it\". A header (or\n    `Authorization: Bearer`) alternative is not offered.\n  documented_by_provider: false\nscopes:\n  present: false\n  note: >-\n    No OAuth scopes exist, so no scopes/ artifact is written. Authorization is plan-level, not\n    scope-level: the token's plan determines symbol basket, market coverage, request rate and\n    history depth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alltick-api/refs/heads/main/authentication/alltick-api-authentication.yml
summary_line: 1 scheme
tags:
- financial-market-data
- real-time-data
- stock-market-data
- forex-data
- Cryptocurrency Data
- commodities-data
- tick-data
- websocket-streaming
- Fintech
- quantitative-trading
- market-data-api
- trading-halts
---
