---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Flo Ev Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: FLO secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: FLO
provider_slug: flo-ev
scheme_count: 2
schemes:
- authorizationUrl: https://shopify.com/authentication/85271511350/oauth/authorize
  bearer_methods:
  - header
  covers: FLO store customer accounts and authenticated use of the storefront MCP server at https://store.flo.com/api/mcp. Anonymous callers can still list tools and search the catalogue.
  host: store.flo.com
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/85271511350
  jwks_uri: https://shopify.com/authentication/85271511350/.well-known/jwks.json
  name: shopify-customer-accounts
  openIdConnectUrl: https://store.flo.com/.well-known/openid-configuration
  protected_resource: https://store.flo.com
  protected_resource_metadata: https://store.flo.com/.well-known/oauth-protected-resource
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  sources:
  - well-known/flo-ev-store-openid-configuration.json
  - well-known/flo-ev-store-oauth-protected-resource.json
  tokenUrl: https://shopify.com/authentication/85271511350/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- authorizationUrl: https://network.flo.com/services/oauth2/authorize
  covers: The login-gated FLO community/partner portal. Salesforce's own REST API version index is anonymously readable at https://network.flo.com/services/data/ (HTTP 200) but every data endpoint behind it requires an authenticated Salesforce session.
  dynamic_registration: gated
  dynamic_registration_note: POST /services/oauth2/register returns 401 invalid_client - open dynamic client registration is not available to unaffiliated developers.
  end_session_endpoint: https://network.flo.com/services/auth/idp/oidc/logout
  host: network.flo.com
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://network.flo.com/services/oauth2/introspect
  issuer: https://network.flo.com
  jwks_uri: https://network.flo.com/id/keys
  name: salesforce-experience-cloud
  openIdConnectUrl: https://network.flo.com/.well-known/openid-configuration
  registration_endpoint: https://network.flo.com/services/oauth2/register
  response_types:
  - code
  - token
  - token id_token
  revocation_endpoint: https://network.flo.com/services/oauth2/revoke
  sources:
  - well-known/flo-ev-network-openid-configuration.json
  tokenUrl: https://network.flo.com/services/oauth2/token
  type: openIdConnect
  userinfo_endpoint: https://network.flo.com/services/oauth2/userinfo
slug: flo-ev-authentication
source_filename: flo-ev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  live /.well-known/ discovery documents on store.flo.com and network.flo.com,\n  plus FLO's own published human-authentication surfaces\nnote: >-\n  FLO documents no API authentication scheme, because it documents no API. What\n  IS live and machine-readable is the identity layer of the two SaaS platforms\n  FLO runs on its own hosts - Shopify Customer Accounts (store.flo.com) and\n  Salesforce Experience Cloud (network.flo.com). Both are captured here verbatim\n  from their discovery documents. Everything else in FLO's estate authenticates\n  humans, not programs.\nsummary:\n  types: [openIdConnect, oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  first_party_api_auth: none-published\nschemes:\n- name: shopify-customer-accounts\n  type: openIdConnect\n  host: store.flo.com\n  issuer: https://shopify.com/authentication/85271511350\n  openIdConnectUrl: https://store.flo.com/.well-known/openid-configuration\n\
  \  authorizationUrl: https://shopify.com/authentication/85271511350/oauth/authorize\n  tokenUrl: https://shopify.com/authentication/85271511350/oauth/token\n  jwks_uri: https://shopify.com/authentication/85271511350/.well-known/jwks.json\n  response_types: [code]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  protected_resource: https://store.flo.com\n  protected_resource_metadata: https://store.flo.com/.well-known/oauth-protected-resource\n  bearer_methods: [header]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  sources: [well-known/flo-ev-store-openid-configuration.json, well-known/flo-ev-store-oauth-protected-resource.json]\n  covers: >-\n    FLO store customer accounts and authenticated use of the storefront MCP\n    server at https://store.flo.com/api/mcp. Anonymous callers can still list\n    tools and search the catalogue.\n- name: salesforce-experience-cloud\n  type: openIdConnect\n  host: network.flo.com\n\
  \  issuer: https://network.flo.com\n  openIdConnectUrl: https://network.flo.com/.well-known/openid-configuration\n  authorizationUrl: https://network.flo.com/services/oauth2/authorize\n  tokenUrl: https://network.flo.com/services/oauth2/token\n  userinfo_endpoint: https://network.flo.com/services/oauth2/userinfo\n  revocation_endpoint: https://network.flo.com/services/oauth2/revoke\n  introspection_endpoint: https://network.flo.com/services/oauth2/introspect\n  registration_endpoint: https://network.flo.com/services/oauth2/register\n  end_session_endpoint: https://network.flo.com/services/auth/idp/oidc/logout\n  jwks_uri: https://network.flo.com/id/keys\n  response_types: [code, token, 'token id_token']\n  id_token_signing_alg: [RS256]\n  dynamic_registration: gated\n  dynamic_registration_note: >-\n    POST /services/oauth2/register returns 401 invalid_client - open dynamic\n    client registration is not available to unaffiliated developers.\n  sources: [well-known/flo-ev-network-openid-configuration.json]\n\
  \  covers: >-\n    The login-gated FLO community/partner portal. Salesforce's own REST API\n    version index is anonymously readable at\n    https://network.flo.com/services/data/ (HTTP 200) but every data endpoint\n    behind it requires an authenticated Salesforce session.\nhuman_authentication:\n- surface: https://account.flo.com/Account/Login\n  kind: web form login (ASP.NET)\n  audience: drivers and station owners\n  status: 200\n- surface: FLO mobile app\n  kind: account login, then session start/stop at the station\n- surface: in-station driver authentication\n  kind: FLO mobile app, RFID card, credit card (FLO states PCI-DSS compliant payment), or GM Plug and Charge autocharge\n- surface: https://network.flo.com/login\n  kind: Salesforce Experience Cloud community login\ngated_api_infrastructure:\n- host: auth.flo.com\n  evidence: 'HTTP 403 {\"message\":\"Missing Authentication Token\"} on every path probed'\n  inference: AWS API Gateway fronting a private FLO authentication service.\
  \ No public route, no spec, no documentation.\n- host: mqtt-production.ems.flo.com\n  evidence: 'HTTP 404 {\"message\":\"Not Found\",\"traceId\":\"...\"} on every path probed'\n  inference: FLO energy-management-system service endpoint. Responds with a structured JSON error envelope but exposes no public route.\nnot_found:\n  api_keys: no published issuance path\n  mtls: not published\n  oauth_scopes_defined_by_flo: none - every scope observed is a Shopify or Salesforce platform scope\n  security_txt: absent on all hosts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flo-ev/refs/heads/main/authentication/flo-ev-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Energy
- Canada
- EV Charging
- Electricity
- Grid
- Demand Response
- Interoperability
- OCPP
- OCPI
- OpenADR
- Charge Point Operator
- Quebec
---
