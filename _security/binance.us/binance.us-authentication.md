---
api_key_in:
- header
- query
api_specs:
- filename: binance.us-websocket-api-asyncapi.yml
  format: yaml
  label: Binance.US WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/asyncapi/binance.us-websocket-api-asyncapi.yml
- filename: binance.us-websocket-streams-asyncapi.yml
  format: yaml
  label: Binance.US WebSocket Streams
  slug: websocket-streams
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/asyncapi/binance.us-websocket-streams-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Binance.Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: Binance.US secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Binance.US
provider_slug: binance.us
scheme_count: 2
schemes:
- description: The API key is passed to the REST API in the X-MBX-APIKEY header. API keys and secret keys are case-sensitive. Keys can be restricted so one key reaches only certain endpoint classes (e.g. TRADE only); by default a key can access all secure routes. IP binding is recommended by Binance.US.
  in: header
  name: X-MBX-APIKEY
  parameter: X-MBX-APIKEY
  sources:
  - https://docs.binance.us/#authentication-types
  type: apiKey
- description: 'SIGNED endpoints require a `signature` parameter: the HMAC SHA-256 of the total request payload (query string and/or request body, concatenated) keyed with the account secret key. The signature is not case-sensitive and may be sent in the query string or the request body; if sent in both, the query string value is used.'
  in: query
  name: signature
  parameter: signature
  sources:
  - https://docs.binance.us/#signature-authentication
  type: apiKey
slug: binance.us-authentication
source_filename: binance.us-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: searched\nsource: https://docs.binance.us/#authentication\ndocs: https://docs.binance.us/#authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  request_signing: HMAC SHA-256\n  note: >-\n    Binance.US uses API key + HMAC SHA-256 request signing. There is no OAuth 2.0, OpenID Connect or\n    mutual-TLS surface, so no scopes/ artifact applies — permissions are configured per API key in the\n    account UI rather than requested as OAuth scopes.\nschemes:\n- name: X-MBX-APIKEY\n  type: apiKey\n  in: header\n  parameter: X-MBX-APIKEY\n  description: >-\n    The API key is passed to the REST API in the X-MBX-APIKEY header. API keys and secret keys are\n    case-sensitive. Keys can be restricted so one key reaches only certain endpoint classes (e.g. TRADE only);\n    by default a key can access all secure routes. IP binding is recommended by Binance.US.\n  sources:\n  - https://docs.binance.us/#authentication-types\n\
  - name: signature\n  type: apiKey\n  in: query\n  parameter: signature\n  description: >-\n    SIGNED endpoints require a `signature` parameter: the HMAC SHA-256 of the total request payload (query\n    string and/or request body, concatenated) keyed with the account secret key. The signature is not\n    case-sensitive and may be sent in the query string or the request body; if sent in both, the query string\n    value is used.\n  sources:\n  - https://docs.binance.us/#signature-authentication\ntiming:\n  timestamp_parameter: timestamp\n  timestamp_unit: milliseconds\n  recv_window_parameter: recvWindow\n  recv_window_default_ms: 5000\n  recv_window_max_ms: 60000\n  rule: >-\n    A request is processed when `timestamp < (serverTime + 1000)` and `(serverTime - timestamp) <= recvWindow`.\n    Binance.US recommends a recvWindow of 5000 ms or less.\nsecurity_types:\n- id: NONE\n  description: Endpoint can be accessed freely.\n  requires_api_key: false\n  requires_signature: false\n- id: TRADE\n\
  \  description: Endpoint requires sending a valid API key and signature.\n  requires_api_key: true\n  requires_signature: true\n- id: USER_DATA\n  description: Endpoint requires sending a valid API key and signature.\n  requires_api_key: true\n  requires_signature: true\n- id: USER_STREAM\n  description: Endpoint requires sending a valid API key.\n  requires_api_key: true\n  requires_signature: false\n- id: MARKET_DATA\n  description: Endpoint requires sending a valid API key.\n  requires_api_key: true\n  requires_signature: false\nkey_types:\n- id: exchange\n  name: Exchange API Keys\n  availability: self-serve\n  description: >-\n    Private API keys for the majority of API users to interact with Binance.US API endpoints. Provides access\n    to markets and real-time trading services. Created from the account profile menu > API Management, with\n    2FA confirmation. KYC must be completed before an API key can be created.\n  covers:\n  - REST API\n  - WebSocket API\n  - WebSocket Streams\n\
  \  - OTC endpoints (requires 'Enable Spot Trading' restriction)\n- id: custodial-solution\n  name: Custodial Solution API Keys\n  availability: agreement-required\n  description: >-\n    Only available to users who have entered into a Custody Exchange Network agreement between a participating\n    custody partner and Binance.US. Provides access to Custodial Solution endpoints only.\n  covers:\n  - Custodial Solution endpoints\n- id: credit-line\n  name: Credit Line API Keys\n  availability: agreement-required\n  description: >-\n    Only available to institutional users who have signed a credit line agreement with Binance.US. Provides\n    access to Credit Line endpoints only.\n  covers:\n  - Credit Line endpoints\nkey_management:\n  console: https://www.binance.us/ (profile menu > API Management)\n  two_factor_required: true\n  kyc_required: true\n  ip_allowlisting: recommended\nerrors:\n- code: -1022\n  meaning: Signature for this request is not valid.\n- code: -1021\n  meaning: Timestamp\
  \ for this request is outside of the recvWindow.\n- code: -2014\n  meaning: API-key format invalid.\n- code: -2015\n  meaning: Invalid API-key, IP, or permissions for action.\nx-evidence:\n  fetched: '2026-08-07'\n  url: https://docs.binance.us/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binance.us/refs/heads/main/authentication/binance.us-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- Market Data
- Financial-Services
- WebSocket
- Custody
- Staking
---
