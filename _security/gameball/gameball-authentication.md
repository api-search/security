---
api_key_in:
- header
api_specs:
- filename: gameball-openapi.json
  format: json
  label: Gameball REST API
  slug: gameball-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Gameball Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gameball secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gameball
provider_slug: gameball
scheme_count: 2
schemes:
- description: Primary account API key sent on every request. Sufficient on its own for standard, non-sensitive endpoints.
  in: header
  name: APIKey
  parameter_name: APIKey
  required: true
  source: https://docs.gameball.co/api-reference/overview/authentication
  type: apiKey
- description: Transaction/secret key. Required alongside APIKey for sensitive operations (transactions, redemptions, holds, coupon burns) and for ALL requests when High Security Mode is enabled. Must only be sent from server-side code.
  in: header
  name: SecretKey
  parameter_name: SecretKey
  required: false
  source: https://docs.gameball.co/api-reference/overview/authentication
  type: apiKey
slug: gameball-authentication
source_filename: gameball-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.gameball.co/api-reference/overview/authentication\ndocs: https://docs.gameball.co/api-reference/overview/authentication\nopenapi: openapi/gameball-openapi.json\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Gameball authenticates server-to-server API calls with two API-key headers.\n    APIKey identifies the account/workspace and is required on every request.\n    SecretKey is additionally required on sensitive/transactional operations, and\n    on all operations when \"High Security Mode\" is enabled for the account. No\n    OAuth 2.0 flow or bearer-token grant is used. Requests must originate\n    server-side so the SecretKey is never exposed to the client.\nschemes:\n  - name: APIKey\n    type: apiKey\n    in: header\n    parameter_name: APIKey\n    required: true\n    description: >-\n      Primary account API key sent on every request. Sufficient on its own\
  \ for\n      standard, non-sensitive endpoints.\n    source: https://docs.gameball.co/api-reference/overview/authentication\n  - name: SecretKey\n    type: apiKey\n    in: header\n    parameter_name: SecretKey\n    required: false\n    description: >-\n      Transaction/secret key. Required alongside APIKey for sensitive operations\n      (transactions, redemptions, holds, coupon burns) and for ALL requests when\n      High Security Mode is enabled. Must only be sent from server-side code.\n    source: https://docs.gameball.co/api-reference/overview/authentication\nwidget_auth:\n  mechanism: customer hash\n  description: >-\n    Client-side widget/mobile SDK sessions are secured with a per-customer hash\n    (HMAC of the customer id using the account transaction/secret key) generated\n    server-side and passed to the SDK. See the Get Customer Hash operation.\n  docs: https://docs.gameball.co/api-reference/customers/management/get-customer-hash\nopenapi_declared:\n  source: openapi/gameball-openapi.json\n\
  \  checked: '2026-08-13'\n  security_schemes:\n    - name: apiKey\n      type: apiKey\n      in: header\n      parameter_name: apikey\n      note: >-\n        The published specification spells the header lowercase (\"apikey\") while\n        the documentation writes it \"APIKey\". HTTP header names are\n        case-insensitive, so both work.\n    - name: secretKey\n      type: apiKey\n      in: header\n      parameter_name: secretkey\n      note: Documentation spells it \"SecretKey\"; same case-insensitivity applies.\n    - name: bearerAuth\n      type: http\n      scheme: bearer\n      documented: false\n      finding: undocumented-scheme\n      note: >-\n        DECLARED BUT UNDOCUMENTED. bearerAuth is the document-level default\n        security requirement in the published specification, yet\n        https://docs.gameball.co/api-reference/overview/authentication describes\n        no bearer-token grant for the REST API. In practice it applies to only\n        3 of 78 operations —\
  \ the three /plants paths left over from the\n        Mintlify OpenAPI starter template. Every real Gameball operation\n        overrides the default explicitly. Treat bearerAuth as specification\n        residue, not as an available credential. Flagged in\n        overlays/gameball-openapi-overlay.yaml.\n  per_operation_requirements:\n    - requirement: apiKey + secretKey\n      operations: 54\n      note: >-\n        Two thirds of the surface requires BOTH headers even without High\n        Security Mode — all transaction, coupon, batch and configuration-write\n        operations.\n    - requirement: apiKey only\n      operations: 21\n    - requirement: inherits document default (bearerAuth)\n      operations: 3\n      note: The three template-residue /plants operations.\n  live_probe:\n    url: https://api.gameball.co/api/v4.0/openapi.json\n    http_status: 401\n    body: >-\n      {\"code\": 1000, \"type\": \"AUTHENTICATION_ERROR\", \"message\": \"Unauthorized\n      access. Please\
  \ authenticate to proceed.\"}\n    checked: '2026-08-13'\n    note: >-\n      Confirms the API host rejects unauthenticated calls with the Gameball\n      error envelope rather than a WWW-Authenticate challenge.\nmcp_authentication:\n  surface: https://mcp.gameball.co/mcp\n  type: oauth2\n  detail: >-\n    Gameball's MCP server is a SEPARATE authentication surface from the REST\n    API and it does use OAuth 2.0 — authorization_code + refresh_token with\n    PKCE (S256) and RFC 7591 dynamic client registration, advertising a single\n    scope \"mcp\". This is the only OAuth at Gameball; the REST API has none.\n  cross_ref: scopes/gameball-scopes.yml\n  metadata:\n    - well-known/gameball-oauth-authorization-server.json\n    - well-known/gameball-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/authentication/gameball-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Loyalty
- Rewards
- Gamification
- Customer Engagement
- Retention
- Referrals
- Marketing
- E-Commerce
---
