---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eliq-auth-api-openapi.yaml
  format: yaml
  label: Eliq Auth API
  slug: auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-auth-api-openapi.yaml
- filename: eliq-data-management-api-openapi.json
  format: json
  label: Eliq Data Management API
  slug: data-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-data-management-api-openapi.json
- filename: eliq-insights-api-openapi.yaml
  format: yaml
  label: Eliq Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-insights-api-openapi.yaml
- filename: eliq-intelligence-api-openapi.json
  format: json
  label: Eliq Intelligence API
  slug: intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-intelligence-api-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Eliq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eliq secures its APIs with oauth2 and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eliq
provider_slug: eliq
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Access token issued by the Eliq Auth API, sent as Authorization: Bearer <token>.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/eliq-insights-api-openapi.yaml
  - openapi/eliq-intelligence-api-openapi.json
  - https://developer.eliq.com/doc/authentication
  type: http
slug: eliq-authentication
source_filename: eliq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# Eliq authentication profile.\ngenerated: '2026-09-06'\nmethod: searched\nsource: https://developer.eliq.com/doc/authentication\ndocs: https://developer.eliq.com/doc/authentication\nprovider: Eliq\nproviderId: eliq\nsummary:\n  types:\n  - oauth2\n  - http\n  primary: OAuth 2.0 client credentials issuing a signed JWT bearer token\n  note: Derived from the specs this reads as a bare `http bearer` scheme, because the Insights and Intelligence\n    documents declare only the bearer half. The provider documents the full OAuth 2.0 client-credentials flow behind\n    it, so this file is upgraded to `searched`.\nauthorization_server:\n  issuer: https://auth-api.eliq.com\n  token_endpoint: https://auth-api.eliq.com/oauth/token\n  jwks_uri: https://auth-api.eliq.com/.well-known/jwks.json\n  discovery: https://auth-api.eliq.com/.well-known/openid-configuration\n  uat_issuer: https://auth-api-uat.eliq.com\n  signing_alg: RS256 (asymmetric)\n  grant_types:\n  - client_credentials\n  -\
  \ refresh_token\n  request_content_types:\n  - application/json\n  - application/x-www-form-urlencoded\n  access_token_lifetime_seconds: 3600\n  refresh_token_lifetime_seconds: 2592000\nflows:\n- name: App token\n  grant_type: client_credentials\n  use: server-to-server, no end-user context\n  fields:\n  - grant_type\n  - client_id\n  - client_secret\n  - aud\n  - scope (optional)\n  note: '`aud` names the target API — data-management-api or insights-api. A token is scoped to one API.'\n- name: Delegated token\n  grant_type: client_credentials\n  use: acting on behalf of one end user; required where the target API enforces user context\n  fields:\n  - grant_type\n  - client_id\n  - client_secret\n  - aud\n  - scope\n  - sub\n  - sub_type\n  - issue_refresh_token (optional)\n  note: '`sub` is the user id, `sub_type` typically `user`. This is the delegated-identity mechanism an agent would\n    use to act for a named customer.'\n- name: Token refresh\n  grant_type: refresh_token\n  use:\
  \ exchange a refresh token for a new access token\n  fields:\n  - grant_type\n  - refresh_token\ntoken_claims:\n- claim: iss\n  description: Token issuer\n  example: https://auth-api.eliq.com\n- claim: aud\n  description: Target API the token is scoped to\n  example: data-management-api\n- claim: client_id\n  description: OAuth application the token belongs to\n- claim: org\n  description: Organization ID\n- claim: org_type\n  description: Type of organization\n  example: utility\n- claim: sub\n  description: Identity the token represents (user id, or the client id for an app token)\n- claim: sub_type\n  description: Type of subject\n  example: user | client\n- claim: scope\n  description: Scopes granted\n  example: data.read data.write\n- claim: access_type\n  description: How access was granted\n  example: application | delegated\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Access token issued by the Eliq Auth API, sent as Authorization:\
  \ Bearer <token>.'\n  sources:\n  - openapi/eliq-insights-api-openapi.yaml\n  - openapi/eliq-intelligence-api-openapi.json\n  - https://developer.eliq.com/doc/authentication\ncredential_management:\n  issuance: client_id is issued by an Eliq account manager when the integration is set up.\n  secrets: Client secrets are generated via the Client Admin API or by the account manager. Multiple secrets per\n    client are supported so secrets can be rotated without downtime.\n  portal: Client Admin Portal — shows which APIs the client can reach, the access types and scopes available per\n    API, and manages/rotates secrets.\n  dynamic_client_registration: false\n  note: No DCR, no self-serve key issuance. An agent cannot obtain credentials without a human commercial step.\nlegacy:\n  model: Auth v1 (numeric Utility ClientId)\n  status: still supported unchanged; migration offered, not forced\nwebhook_auth:\n  inbound: Eliq signs outbound webhook events with HMAC-SHA256 over \"{timestamp}.{json_payload}\"\
  , carried in the\n    X-Eliq-Signature header as t=<unix>,sha256=<hex>. Consumer endpoints must be HTTPS and may additionally require\n    Basic auth or OAuth2.\n  docs: https://developer.eliq.com/doc/webhooks\nrequirements:\n- TLS (HTTPS) must always be used\n- Client secrets and tokens must never be exposed in client-side applications or public repositories\n- Compromised tokens must be revoked immediately\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/authentication/eliq-authentication.yml
summary_line: oauth2/http · 1 scheme
tags:
- Energy
- Utilities
- Analytics
- Sustainability
- Energy Data
- Smart Meter
- Disaggregation
- Forecasting
- Segmentation
- Consumption
- Tariffs
- Insights
---
