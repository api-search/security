---
api_key_in: []
api_specs:
- filename: flume-health-account-contracts-api-openapi.yml
  format: yaml
  label: Flume Health Account Contracts API
  slug: flume-health-account-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-account-contracts-api-openapi.yml
- filename: flume-health-accounts-api-openapi.yml
  format: yaml
  label: Flume Health Accounts API
  slug: flume-health-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-accounts-api-openapi.yml
- filename: flume-health-automapjobs-api-openapi.yml
  format: yaml
  label: Flume Health Automap Jobs API
  slug: flume-health-automapjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-automapjobs-api-openapi.yml
- filename: flume-health-connections-api-openapi.yml
  format: yaml
  label: Flume Health Connections API
  slug: flume-health-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-connections-api-openapi.yml
- filename: flume-health-context-discovery-api-openapi.yml
  format: yaml
  label: Flume Health Context Discovery API
  slug: flume-health-context-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-context-discovery-api-openapi.yml
- filename: flume-health-context-graph-api-openapi.yml
  format: yaml
  label: Flume Health Context Graph API
  slug: flume-health-context-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-context-graph-api-openapi.yml
- filename: flume-health-context-knowledge-api-openapi.yml
  format: yaml
  label: Flume Health Context Knowledge API
  slug: flume-health-context-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-context-knowledge-api-openapi.yml
- filename: flume-health-endpoint-maps-api-openapi.yml
  format: yaml
  label: Flume Health Endpoint Maps API
  slug: flume-health-endpoint-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-endpoint-maps-api-openapi.yml
- filename: flume-health-endpoints-api-openapi.yml
  format: yaml
  label: Flume Health Endpoints API
  slug: flume-health-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-endpoints-api-openapi.yml
- filename: flume-health-flags-api-openapi.yml
  format: yaml
  label: Flume Health Flags API
  slug: flume-health-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-flags-api-openapi.yml
- filename: flume-health-jobs-v2-api-openapi.yml
  format: yaml
  label: Flume Health Jobs v2 API
  slug: flume-health-jobs-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-jobs-v2-api-openapi.yml
- filename: flume-health-objects-api-openapi.yml
  format: yaml
  label: Flume Health Objects API
  slug: flume-health-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-objects-api-openapi.yml
- filename: flume-health-reports-api-openapi.yml
  format: yaml
  label: Flume Health Reports API
  slug: flume-health-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-reports-api-openapi.yml
- filename: flume-health-shards-api-openapi.yml
  format: yaml
  label: Flume Health Shards API
  slug: flume-health-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-shards-api-openapi.yml
- filename: flume-health-sourcefile-api-openapi.yml
  format: yaml
  label: Flume Health Source File API
  slug: flume-health-sourcefile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-sourcefile-api-openapi.yml
- filename: flume-health-telemetry-api-openapi.yml
  format: yaml
  label: Flume Health Telemetry API
  slug: flume-health-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-telemetry-api-openapi.yml
- filename: flume-health-transactions-api-openapi.yml
  format: yaml
  label: Flume Health Transactions API
  slug: flume-health-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-transactions-api-openapi.yml
- filename: flume-health-users-api-openapi.yml
  format: yaml
  label: Flume Health Users API
  slug: flume-health-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-users-api-openapi.yml
- filename: flume-health-workersizes-api-openapi.yml
  format: yaml
  label: Flume Health Worker Sizes API
  slug: flume-health-workersizes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/openapi/flume-health-workersizes-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Flume Health Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- authorization_code
- client_credentials
- refresh_token
- device_code
- token_exchange
overview: Flume Health secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, authorization_code, client_credentials, refresh_token, device_code, and token_exchange flow(s).
provider_name: Flume Health
provider_slug: flume-health
scheme_count: 3
schemes:
- declared_in: openapi/flume-health-console-api-openapi.yml
  flows:
  - authorizationUrl: https://auth.flumehealth.com/authorize?audience=https://console.flumehealth.com/api
    flow: implicit
    scopes:
    - openid
    - profile
    - email
  name: OAuth2Implicit
  note: The browser flow the Flume Console itself uses. It is the ONLY scheme the published contract declares.
  sources:
  - openapi/flume-health-console-api-openapi.yml
  type: oauth2
- code_challenge_methods_supported:
  - S256
  - plain
  declared_in: https://auth.flumehealth.com/.well-known/openid-configuration
  dpop_signing_alg_values_supported:
  - ES256
  dynamic_client_registration: true
  endpoints:
    authorization: https://auth.flumehealth.com/authorize
    backchannel_authentication: https://auth.flumehealth.com/bc-authorize
    device_authorization: https://auth.flumehealth.com/oauth/device/code
    end_session: https://auth.flumehealth.com/oidc/logout
    jwks: https://auth.flumehealth.com/.well-known/jwks.json
    mfa_challenge: https://auth.flumehealth.com/mfa/challenge
    registration: https://auth.flumehealth.com/oidc/register
    revocation: https://auth.flumehealth.com/oauth/revoke
    token: https://auth.flumehealth.com/oauth/token
    userinfo: https://auth.flumehealth.com/userinfo
  grant_types_supported:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  - PS256
  - HS256
  issuer: https://auth.flumehealth.com/
  mfa: true
  name: Flume authorization server (live)
  sources:
  - well-known/flume-health-oauth-authorization-server.json
  - well-known/flume-health-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- authorization_servers:
  - https://auth.flumehealth.com
  bearer_methods_supported:
  - header
  declared_in: https://console.flumehealth.com/.well-known/oauth-protected-resource
  name: MCP protected resource
  note: Correct RFC 9728 implementation — the MCP endpoint answers an anonymous JSON-RPC POST with HTTP 401 and WWW-Authenticate Bearer carrying a resource_metadata pointer back to this document.
  resource: https://console.flumehealth.com/api/v1/context/mcp
  rfc9728: true
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  sources:
  - well-known/flume-health-oauth-protected-resource.json
  type: oauth2
slug: flume-health-authentication
source_filename: flume-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: >-\n  https://auth.flumehealth.com/.well-known/oauth-authorization-server +\n  https://console.flumehealth.com/.well-known/oauth-protected-resource + openapi/flume-health-console-api-openapi.yml\nnote: >-\n  Upgraded from the spec-only derivation. The Flume Console API's Swagger 2.0 contract declares exactly one security\n  scheme — an OAuth 2.0 implicit flow — which understates what is actually deployed. The live authorization server\n  at auth.flumehealth.com (an Auth0 tenant on Flume's own domain, issuer https://auth.flumehealth.com/) publishes\n  RFC 8414 / OIDC discovery metadata advertising 13 grant types including authorization_code with PKCE,\n  client_credentials, refresh_token, device_code and token exchange, plus dynamic client registration and DPoP.\n  Machine-to-machine integrators should use those, not the implicit flow in the spec. Flume publishes no\n  authentication documentation page — there is nothing to search\
  \ — so every fact below comes from the contract or\n  from a live probe.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - implicit\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - device_code\n  - token_exchange\n  primary: OAuth 2.0 bearer token in the Authorization header\n  api_keys: false\n  mutual_tls: false\n  basic_auth: false\ndocs: null\ndocs_note: Flume publishes no public authentication guide. The only machine-readable auth description is the securityDefinitions block in the contract plus the discovery documents below.\n\nschemes:\n- name: OAuth2Implicit\n  type: oauth2\n  declared_in: openapi/flume-health-console-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.flumehealth.com/authorize?audience=https://console.flumehealth.com/api\n    scopes:\n    - openid\n    - profile\n    - email\n  note: The browser flow the Flume Console itself uses. It is the ONLY scheme the published contract declares.\n\
  \  sources:\n  - openapi/flume-health-console-api-openapi.yml\n\n- name: Flume authorization server (live)\n  type: openIdConnect\n  declared_in: https://auth.flumehealth.com/.well-known/openid-configuration\n  issuer: https://auth.flumehealth.com/\n  endpoints:\n    authorization: https://auth.flumehealth.com/authorize\n    token: https://auth.flumehealth.com/oauth/token\n    userinfo: https://auth.flumehealth.com/userinfo\n    jwks: https://auth.flumehealth.com/.well-known/jwks.json\n    registration: https://auth.flumehealth.com/oidc/register\n    revocation: https://auth.flumehealth.com/oauth/revoke\n    device_authorization: https://auth.flumehealth.com/oauth/device/code\n    end_session: https://auth.flumehealth.com/oidc/logout\n    backchannel_authentication: https://auth.flumehealth.com/bc-authorize\n    mfa_challenge: https://auth.flumehealth.com/mfa/challenge\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n\
  \  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - RS256\n  - PS256\n  - HS256\n  dpop_signing_alg_values_supported:\n  - ES256\n  dynamic_client_registration: true\n  mfa: true\n  sources:\n  - well-known/flume-health-oauth-authorization-server.json\n  - well-known/flume-health-openid-configuration.json\n\n- name: MCP protected resource\n  type: oauth2\n  declared_in: https://console.flumehealth.com/.well-known/oauth-protected-resource\n  resource: https://console.flumehealth.com/api/v1/context/mcp\n  authorization_servers:\n  - https://auth.flumehealth.com\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - openid\n  - profile\n  - email\n \
  \ - offline_access\n  rfc9728: true\n  note: >-\n    Correct RFC 9728 implementation — the MCP endpoint answers an anonymous JSON-RPC POST with HTTP 401 and\n    WWW-Authenticate Bearer carrying a resource_metadata pointer back to this document.\n  sources:\n  - well-known/flume-health-oauth-protected-resource.json\n\nauthorization_context:\n  account_scoping_header: X-Flume-Account-ID\n  required_on: 122 of 153 operations\n  note: >-\n    Bearer authentication alone is not sufficient. Nearly every operation additionally requires the\n    X-Flume-Account-ID header naming the health-plan account. Missing or wrong values surface as 403.\n\nevidence:\n- url: https://auth.flumehealth.com/.well-known/oauth-authorization-server\n  http_status: 200\n- url: https://auth.flumehealth.com/.well-known/openid-configuration\n  http_status: 200\n- url: https://auth.flumehealth.com/.well-known/jwks.json\n  http_status: 200\n- url: https://console.flumehealth.com/.well-known/oauth-protected-resource\n\
  \  http_status: 200\n- url: https://console.flumehealth.com/api/v1/accounts\n  http_status: 401\n  detail: bare request rejected; no WWW-Authenticate on the REST path (unlike the MCP path, which does send one)\n- url: https://console.flumehealth.com/api/docs/docs.json\n  http_status: 200\nchecked: '2026-08-16'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flume-health/refs/heads/main/authentication/flume-health-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Healthcare
- Health Plans
- Payers
- Healthcare Data
- Data Integration
- iPaaS
- Eligibility
- Claims
- Knowledge Graph
- MCP
- agent-native
- Authentication
- Data Engineering
- Interoperability
---
