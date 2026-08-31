---
api_key_in: []
api_specs:
- filename: green-button-alliance-applicationinformation-api-openapi.yml
  format: yaml
  label: Green Button Alliance Application Information API
  slug: green-button-alliance-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-applicationinformation-api-openapi.yml
- filename: green-button-alliance-authorization-api-openapi.yml
  format: yaml
  label: Green Button Alliance Authorization API
  slug: green-button-alliance-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-authorization-api-openapi.yml
- filename: green-button-alliance-batch-api-openapi.yml
  format: yaml
  label: Green Button Alliance Batch API
  slug: green-button-alliance-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-batch-api-openapi.yml
- filename: green-button-alliance-datacustodian-integration-api-openapi.yml
  format: yaml
  label: Green Button Alliance DataCustodian Integration API
  slug: green-button-alliance-datacustodian-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-datacustodian-integration-api-openapi.yml
- filename: green-button-alliance-oauth2-client-management-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Client Management API
  slug: green-button-alliance-oauth2-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-client-management-api-openapi.yml
- filename: green-button-alliance-oauth2-standard-api-openapi.yml
  format: yaml
  label: Green Button Alliance OAuth2 Standard API
  slug: green-button-alliance-oauth2-standard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oauth2-standard-api-openapi.yml
- filename: green-button-alliance-oidc-api-openapi.yml
  format: yaml
  label: Green Button Alliance OIDC API
  slug: green-button-alliance-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-oidc-api-openapi.yml
- filename: green-button-alliance-usagepoint-api-openapi.yml
  format: yaml
  label: Green Button Alliance Usage Point API
  slug: green-button-alliance-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/openapi/green-button-alliance-usagepoint-api-openapi.yml
auth_types:
- http
- mutualTLS
- oauth2
- openIdConnect
description: Three distinct authentication surfaces sit under the Green Button Alliance name and must not be conflated. (1) The CMD ESPI resource server contract - OAuth 2.0 authorization_code and client_credentials, bearer tokens, ESPI Function Block scope grammar; this is the interface every certified Data Custodian implements, not a service GBA runs. (2) The OpenESPI Authorization Server GBA publishes as a reference implementation - JWT bearer, HTTP basic client credentials, and X.509 mutual TLS client certificates, TLS 1.3 only. (3) GBA's own member single sign-on - a standard OIDC provider for the association's membership system, which grants no access to any energy data at all.
kind: authentication
layout: security
method: searched
name: Green Button Alliance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Green Button Alliance secures its APIs with http, mutualTLS, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Green Button Alliance
provider_slug: green-button-alliance
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/green-button-alliance-authorization-server-openapi.yml
  type: http
- description: HTTP Basic client authentication (client_secret_basic) at the token endpoint.
  name: ClientCredentials
  scheme: basic
  sources:
  - openapi/green-button-alliance-authorization-server-openapi.yml
  type: http
- description: X.509 client certificate authentication (tls_client_auth). The authorization server spec states "TLS 1.3 ONLY", "Certificate Authentication - Support for X.509 client certificates" and "Perfect Forward Secrecy - All cipher suites support PFS".
  name: ClientCertificate
  sources:
  - openapi/green-button-alliance-authorization-server-openapi.yml
  type: mutualTLS
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  scope_model: ESPI Function Block grammar (FB=1_3_4_5;IntervalDuration=900;...). The spec declares an empty scopes map; see scopes/green-button-alliance-scopes.yml.
  sources:
  - openapi/green-button-alliance-green-button-api-openapi.yml
  type: oauth2
slug: green-button-alliance-authentication
source_filename: green-button-alliance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/green-button-alliance-authorization-server-openapi.yml, openapi/green-button-alliance-green-button-api-openapi.yml\ndocs: https://www.greenbuttonalliance.org/access-tokens\nadditional_docs:\n- https://www.greenbuttonalliance.org/oauth-20-access-and-refresh-token-duration\n- https://www.greenbuttonalliance.org/function-blocks\n- https://github.com/GreenButtonAlliance/OpenESPI-GreenButton-Java/blob/main/openespi-authserver/docs/OAUTH2_CLIENT_MANAGEMENT_API.md\n- https://github.com/GreenButtonAlliance/OpenESPI-GreenButton-Java/blob/main/openespi-authserver/docs/OIDC_USERINFO_ENDPOINT.md\n- https://archive.greenbuttondata.org/espi/access_tokens/\ndescription: >-\n  Three distinct authentication surfaces sit under the Green Button Alliance name\n  and must not be conflated. (1) The CMD ESPI resource server contract - OAuth 2.0\n  authorization_code and client_credentials, bearer tokens, ESPI Function Block\n  scope grammar;\
  \ this is the interface every certified Data Custodian implements,\n  not a service GBA runs. (2) The OpenESPI Authorization Server GBA publishes as a\n  reference implementation - JWT bearer, HTTP basic client credentials, and X.509\n  mutual TLS client certificates, TLS 1.3 only. (3) GBA's own member single sign-on\n  - a standard OIDC provider for the association's membership system, which grants\n  no access to any energy data at all.\nsummary:\n  types:\n  - http\n  - mutualTLS\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  api_key_in: []\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/green-button-alliance-authorization-server-openapi.yml\n- name: ClientCredentials\n  type: http\n  scheme: basic\n  description: HTTP Basic client authentication (client_secret_basic) at the token endpoint.\n  sources:\n  - openapi/green-button-alliance-authorization-server-openapi.yml\n\
  - name: ClientCertificate\n  type: mutualTLS\n  description: >-\n    X.509 client certificate authentication (tls_client_auth). The authorization\n    server spec states \"TLS 1.3 ONLY\", \"Certificate Authentication - Support for\n    X.509 client certificates\" and \"Perfect Forward Secrecy - All cipher suites\n    support PFS\".\n  sources:\n  - openapi/green-button-alliance-authorization-server-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  scope_model: >-\n    ESPI Function Block grammar (FB=1_3_4_5;IntervalDuration=900;...). The spec\n    declares an empty scopes map; see scopes/green-button-alliance-scopes.yml.\n  sources:\n  - openapi/green-button-alliance-green-button-api-openapi.yml\n\
  client_authentication_methods:\n- client_secret_basic\n- client_secret_post\n- tls_client_auth\ngrant_types:\n- authorization_code\n- client_credentials\n- refresh_token\ndynamic_client_registration:\n  supported: true\n  specs:\n  - RFC 7591 OAuth 2.0 Dynamic Client Registration\n  - RFC 7592 OAuth 2.0 Dynamic Client Registration Management\n  evidence: >-\n    Both RFCs are listed as normative references on GBA's /developer-resources, and\n    the published ApplicationInformation resource carries the full RFC 7591/7592\n    field set (client_id, client_secret, client_id_issued_at,\n    client_secret_expires_at, registration_client_uri, registration_access_token,\n    token_endpoint_auth_method, grant_types, response_types).\n  registration_endpoint_field: authorizationServerRegistrationEndpoint\ntoken_types:\n  source: https://www.greenbuttonalliance.org/access-tokens\n  values:\n  - access_token\n  - refresh_token\n  - datacustodian_access_token\n  - client_access_token\n  - upload_access_token\n\
  \  - registration_access_token\n  detail: scopes/green-button-alliance-scopes.yml\ntoken_duration_guidance:\n  source: https://www.greenbuttonalliance.org/oauth-20-access-and-refresh-token-duration\n  summary: >-\n    GBA publishes a guidance article on OAuth 2.0 access and refresh token duration\n    in the Green Button Connect context - access tokens short-lived; refresh tokens\n    \"long lifespans (days to weeks) and be rotated whenever used to meet best\n    practice security standards\". Verbatim numeric ceilings live in the paywalled\n    NAESB REQ.21 ESPI standard and are not reproduced.\nmember_sso:\n  note: Association membership single sign-on. NOT a route to energy data.\n  type: openIdConnect\n  discovery: https://www.greenbuttonalliance.org/.well-known/openid-configuration\n  file: well-known/green-button-alliance-openid-configuration.json\n  issuer: https://www.greenbuttonalliance.org\n  grant_types: [authorization_code, refresh_token]\n  scopes: [openid, email, profile]\n\
  \  pkce: [S256]\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\ntransport_security:\n  espi_v4_0: TLS 1.3 minimum\n  espi_v3_3: TLS 1.2\n  authorization_server: TLS 1.3 only (stated in the OpenESPI Authorization Server spec)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-button-alliance/refs/heads/main/authentication/green-button-alliance-authentication.yml
summary_line: http/mutualTLS/oauth2/openIdConnect · 4 schemes
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Water
- Smart Metering
- Green Button
- ESPI
- Standards Body
- Certification
- Consumer Energy Data
---
