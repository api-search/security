---
api_key_in:
- header
api_specs:
- filename: keller-williams-listings-search-openapi.json
  format: json
  label: KW Worldwide Listings Search API
  slug: keller-williams-worldwide-listings-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/openapi/keller-williams-listings-search-openapi.json
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Keller Williams Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- tokenExchange
- jwtBearer
- refreshToken
overview: Keller Williams secures its APIs with apiKey, http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, tokenExchange, jwtBearer, and refreshToken flow(s).
provider_name: Keller Williams
provider_slug: keller-williams
scheme_count: 4
schemes:
- aliases:
  - API-Key
  applies_to: all partner gateway requests
  in: header
  name: apiKeyHeader
  parameter: api-key
  source: https://developer.kw.com/docs-authentication
  type: apiKey
- applies_to: Resources that are not scoped to an individual KW user, the Listings Search API as documented in its OpenAPI, and the client authentication leg of /idp/token and /idp/revoke.
  name: basicAuth
  scheme: basic
  source: openapi/keller-williams-listings-search-openapi.json
  type: http
  value: base64(API_KEY:API_SECRET)
- applies_to: user-owned Command data (contacts, tasks, opportunities, listings, marketing profiles)
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  source: https://developer.kw.com/docs-getting-started
  type: http
- endpoints:
    authorize: https://partners.api.kw.com/idp/authorize
    device_authorization: https://partners.api.kw.com/idp/device_authorization
    end_session: https://partners.api.kw.com/idp/end_session
    introspect: https://partners.api.kw.com/idp/introspect
    jwks_uri: https://partners.api.kw.com/idp/keys
    revoke: https://partners.api.kw.com/idp/revoke
    token: https://partners.api.kw.com/idp/token
    userinfo: https://partners.api.kw.com/idp/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://partners.api.kw.com
  jwks_note: The advertised jwks_uri returns HTTP 404 ("Resourse not supported.") to an anonymous client, so ID-token signature verification keys are not publicly retrievable. Probed 2026-07-26.
  name: openIdConnect
  openIdConnectUrl: https://partners.api.kw.com/idp/.well-known/openid-configuration
  pkce:
  - S256
  response_types:
  - code
  - id_token
  - id_token token
  scopes: scopes/keller-williams-scopes.yml
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: keller-williams-authentication
source_filename: keller-williams-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developer.kw.com/docs-authentication\nsource:\n  - https://developer.kw.com/getting-started\n  - https://developer.kw.com/docs-getting-started\n  - https://developer.kw.com/docs-authentication\n  - https://developer.kw.com/docs-refresh-token\n  - https://partners.api.kw.com/idp/.well-known/openid-configuration\n  - openapi/keller-williams-listings-search-openapi.json\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  api_key_names: [api-key, API-Key]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, tokenExchange, jwtBearer, refreshToken]\n  paired_credentials: true\n  note: >-\n    Every Keller Williams partner request carries TWO credentials: the\n    application's `api-key` header (the DevHub app API Key) and an\n    `Authorization` header. Which Authorization credential depends on the\n    resource: user-owned Command data uses an OAuth\
  \ 2.0 / OpenID Connect\n    Bearer access token minted for one individual KW user; non-user-scoped\n    or more public resources use HTTP Basic with\n    base64(API_KEY:API_SECRET). The published Listings OpenAPI declares NO\n    `components.securitySchemes` at all — authorization is modelled as an\n    explicit required `Authorization` header parameter on all seven\n    operations, described as \"Basic token is created by base 64 encoding\n    your credentials: <Basic base64Encode(API_KEY:API_SECRET)>\". That is a\n    real contract-quality gap: a machine reading the spec alone cannot\n    discover the api-key header or the OAuth flows at all.\ncredential_issuance:\n  self_serve: false\n  process:\n    - Submit a partnership application via the \"Apply to Integrate\" HubSpot form.\n    - KWRI reviews and approves; a DevHub account is provisioned (SAML sign-in).\n    - Sign the KW API License Agreement and the DevHub Terms and Conditions.\n    - Create an App in DevHub (name, description,\
  \ owner or team, selected APIs + scopes, one callback URL).\n    - API Key and Secret are revealed on the app record; only Owner and App Admin roles can view the Secret.\n    - Keys can be rotated (\"Add Key\") and revoked (\"Revoke\") from the app record.\n  callback_urls: one per application (redirect URI must be https)\n  teams: Owner / Administrator / Viewer permission levels\nschemes:\n  - name: apiKeyHeader\n    type: apiKey\n    in: header\n    parameter: api-key\n    aliases: [API-Key]\n    applies_to: all partner gateway requests\n    source: https://developer.kw.com/docs-authentication\n  - name: basicAuth\n    type: http\n    scheme: basic\n    value: base64(API_KEY:API_SECRET)\n    applies_to: >-\n      Resources that are not scoped to an individual KW user, the Listings\n      Search API as documented in its OpenAPI, and the client\n      authentication leg of /idp/token and /idp/revoke.\n    source: openapi/keller-williams-listings-search-openapi.json\n  - name: bearerAuth\n\
  \    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to: user-owned Command data (contacts, tasks, opportunities, listings, marketing profiles)\n    source: https://developer.kw.com/docs-getting-started\n  - name: openIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://partners.api.kw.com/idp/.well-known/openid-configuration\n    issuer: https://partners.api.kw.com\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    pkce: [S256]\n    response_types: [code, id_token, \"id_token token\"]\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    scopes: scopes/keller-williams-scopes.yml\n    endpoints:\n      authorize: https://partners.api.kw.com/idp/authorize\n      token: https://partners.api.kw.com/idp/token\n\
  \      introspect: https://partners.api.kw.com/idp/introspect\n      userinfo: https://partners.api.kw.com/idp/userinfo\n      revoke: https://partners.api.kw.com/idp/revoke\n      end_session: https://partners.api.kw.com/idp/end_session\n      device_authorization: https://partners.api.kw.com/idp/device_authorization\n      jwks_uri: https://partners.api.kw.com/idp/keys\n    jwks_note: >-\n      The advertised jwks_uri returns HTTP 404 (\"Resourse not supported.\")\n      to an anonymous client, so ID-token signature verification keys are\n      not publicly retrievable. Probed 2026-07-26.\ntoken_lifetimes:\n  access_token: 2 days\n  refresh_token: 365 days\n  rotation: >-\n    Refresh tokens are single-use — refreshing invalidates the old refresh\n    token and returns a new one in the same payload.\n  expired_refresh: Contact KW; a new refresh token cannot be self-issued.\n  docs: https://developer.kw.com/docs-authentication\npartner_token_refresh:\n  endpoint: https://partners.api.kw.com/v2/oauth2/partner/token\n\
  \  method: POST\n  content_type: application/x-www-form-urlencoded\n  auth: Basic <base64 API_KEY:API_SECRET> + api-key header\n  parameters: [grant_type=refresh_token, account_identifier, refresh_token]\n  response_fields:\n    - access_token\n    - refresh_token\n    - refresh_token_expires_in\n    - refresh_token_status\n    - refresh_token_issued_at\n    - refresh_count\n    - old_access_token_life_time\n    - token_type\n    - expires_in\n    - issued_at\n    - status\n    - client_id\n    - application_name\n    - organization_name\n    - developer.email\n  docs: https://developer.kw.com/docs-refresh-token\nmarketplace_token_minting:\n  note: >-\n    For KW Marketplace integrations, per-user access and refresh tokens\n    are not obtained through the /authorize redirect at all — they are\n    delivered to the partner inside the SUBSCRIPTION_ORDER and\n    USER_ASSIGNMENT webhook payloads as `access-token` and\n    `refresh-token` fields. See asyncapi/keller-williams-marketplace-webhooks.yml.\n\
  \  docs: https://developer.kw.com/docs-getting-started\ntransport:\n  https_required: true\n  note: Calls made over plain HTTP fail; unauthenticated requests fail.\nauthorization_model:\n  granularity: path + verb pair\n  note: >-\n    KW describes a fine-grained access policy where a resource is defined\n    by a path and verb pair — GET /v3/contacts and POST /v3/contacts are\n    granted separately, per partnership.\n  docs: https://developer.kw.com/docs-getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/authentication/keller-williams-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 4 schemes
tags:
- Real-Estate
- United States
- Residential Real Estate
- Brokerage
- Franchise
- Property Listings
- PropTech
- Agent Platform
- CRM
- Partner APIs
- Marketplace
- Austin Texas
---
