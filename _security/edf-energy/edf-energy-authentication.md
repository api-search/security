---
api_key_in:
- header
api_specs:
- filename: edf-energy-account-import-api-openapi.yml
  format: yaml
  label: EDF Energy Account Import API
  slug: edf-energy-account-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-account-import-api-openapi.yml
- filename: edf-energy-data-import-api-openapi.yml
  format: yaml
  label: EDF Energy Data Import API
  slug: edf-energy-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-data-import-api-openapi.yml
- filename: edf-energy-external-client-healthcheck-api-openapi.yml
  format: yaml
  label: EDF Energy External Client Healthcheck API
  slug: edf-energy-external-client-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-external-client-healthcheck-api-openapi.yml
- filename: edf-energy-external-events-api-openapi.yml
  format: yaml
  label: EDF Energy External Events API
  slug: edf-energy-external-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-external-events-api-openapi.yml
- filename: edf-energy-post-account-import-api-openapi.yml
  format: yaml
  label: EDF Energy Post Account Import API
  slug: edf-energy-post-account-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-post-account-import-api-openapi.yml
- filename: edf-energy-query-api-openapi.yml
  format: yaml
  label: EDF Energy Query API
  slug: edf-energy-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-query-api-openapi.yml
- filename: edf-energy-v1-api-openapi.yml
  format: yaml
  label: EDF Energy V1 API
  slug: edf-energy-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-v1-api-openapi.yml
- filename: edf-energy-v2-api-openapi.yml
  format: yaml
  label: EDF Energy V2 API
  slug: edf-energy-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/openapi/edf-energy-v2-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: 'EDF Energy''s API authentication is Kraken''s. There are two co-existing layers. The first is the platform''s own token model, declared in the two OpenAPI documents as six named security schemes, all of which put the credential in the Authorization header (either "Token <key>" or a Kraken JWT, or HTTP Basic where the token is the username). The second is a full OAuth 2.0 / OpenID Connect authorisation server at auth.edfgb-kraken.energy, which is how a third party gets delegated access to a named EDF customer''s data. That server documents four grant types — authorization code with PKCE, client credentials, device code (RFC 8628) and token exchange (RFC 8693) — serves its OpenID Provider Metadata anonymously with 111 scopes, and publishes a JWKS. Onboarding is not self-service: the auth server''s getting-started section instructs a developer to contact EDF/Kraken to request an OAuth application, supplying the client type (public or confidential), the grant type, the allowed
  redirect URIs and the resources to be accessed. Some surface needs no credential at all — REST GET /v1/products/ declares an empty security option and the GraphQL energyProducts query resolves anonymously — which is why EDF markets these as "open tariff APIs".'
kind: authentication
layout: security
method: searched
name: Edf Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- tokenExchange
overview: EDF Energy secures its APIs with apiKey, http, oauth2, and openIdConnect across 8 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and tokenExchange flow(s).
provider_name: EDF Energy
provider_slug: edf-energy
scheme_count: 8
schemes:
- description: Token-based authentication with required prefix "Token "
  format: Token <api-key>
  in: header
  name: KeyAuthentication
  parameter: Authorization
  sources:
  - openapi/edf-energy-kraken-openapi.yml
  type: apiKey
- description: JWT-based authentication
  format: Kraken JWT
  in: header
  name: DRFKrakenTokenAuthentication
  parameter: Authorization
  sources:
  - openapi/edf-energy-kraken-openapi.yml
  - openapi/edf-energy-kraken-data-import-openapi.yml
  type: apiKey
- description: Token-based authentication with required prefix "Token " (data-import viewer)
  format: Token <api-key>
  in: header
  name: DataImportViewerAPIKeyAuthentication
  parameter: Authorization
  sources:
  - openapi/edf-energy-kraken-data-import-openapi.yml
  type: apiKey
- description: Token-based authentication where the token is passed as the username for basic auth
  name: AccountUserAPIKeyAuthentication
  scheme: basic
  sources:
  - openapi/edf-energy-kraken-openapi.yml
  type: http
- description: Basic authentication for affiliate organisations
  name: AffiliateAuthentication
  scheme: basic
  sources:
  - openapi/edf-energy-kraken-openapi.yml
  type: http
- description: Basic authentication for partner organisations
  name: PartnerUserOnlyAuthentication
  scheme: basic
  sources:
  - openapi/edf-energy-kraken-openapi.yml
  type: http
- description: OAuth 2.0 authorisation server for delegated third-party access to customer-scoped data. Not declared in the OpenAPI documents; documented on the auth server itself and discoverable via OpenID Connect metadata.
  flows:
  - authorizationUrl: https://auth.edfgb-kraken.energy/authorize/
    code_challenge_method: S256
    flow: authorizationCode
    pkce: true
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - client_auth: HTTP Basic (base64 client_id:client_secret)
    flow: clientCredentials
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - deviceAuthorizationUrl: https://auth.edfgb-kraken.energy/device-authorization/
    flow: deviceCode
    rfc: RFC 8628
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  - flow: tokenExchange
    rfc: RFC 8693
    tokenUrl: https://auth.edfgb-kraken.energy/token/
  name: KrakenOAuth2
  scopes: scopes/edf-energy-scopes.yml
  sources:
  - https://auth.edfgb-kraken.energy/
  type: oauth2
- claims_supported:
  - sub
  end_session_endpoint: https://auth.edfgb-kraken.energy/logout/
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  issuer: https://auth.edfgb-kraken.energy/token/
  jwks_uri: https://auth.edfgb-kraken.energy/.well-known/jwks.json
  name: KrakenOpenIDConnect
  openIdConnectUrl: https://auth.edfgb-kraken.energy/.well-known/openid-configuration
  revocation_endpoint: https://auth.edfgb-kraken.energy/revoke-token/
  sources:
  - well-known/edf-energy-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  userinfo_endpoint: https://auth.edfgb-kraken.energy/userinfo/
slug: edf-energy-authentication
source_filename: edf-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://auth.edfgb-kraken.energy/ (OAuth server documentation, HTTP 200),\n  https://auth.edfgb-kraken.energy/.well-known/openid-configuration (HTTP 200),\n  https://developer.edfgb-kraken.energy/rest/guides/api-basics/ (HTTP 200),\n  https://developer.edfgb-kraken.energy/graphql/guides/basics/ (HTTP 200), and the\n  securitySchemes declared in openapi/edf-energy-kraken-openapi.yml and\n  openapi/edf-energy-kraken-data-import-openapi.yml.\ndocs: https://auth.edfgb-kraken.energy/\ndescription: >-\n  EDF Energy's API authentication is Kraken's. There are two co-existing layers. The\n  first is the platform's own token model, declared in the two OpenAPI documents as\n  six named security schemes, all of which put the credential in the Authorization\n  header (either \"Token <key>\" or a Kraken JWT, or HTTP Basic where the token is the\n  username). The second is a full OAuth 2.0 / OpenID Connect authorisation server at\n\
  \  auth.edfgb-kraken.energy, which is how a third party gets delegated access to a\n  named EDF customer's data. That server documents four grant types — authorization\n  code with PKCE, client credentials, device code (RFC 8628) and token exchange\n  (RFC 8693) — serves its OpenID Provider Metadata anonymously with 111 scopes, and\n  publishes a JWKS. Onboarding is not self-service: the auth server's getting-started\n  section instructs a developer to contact EDF/Kraken to request an OAuth application,\n  supplying the client type (public or confidential), the grant type, the allowed\n  redirect URIs and the resources to be accessed. Some surface needs no credential at\n  all — REST GET /v1/products/ declares an empty security option and the GraphQL\n  energyProducts query resolves anonymously — which is why EDF markets these as\n  \"open tariff APIs\".\nsummary:\n  types: [apiKey, http, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials,\
  \ deviceCode, tokenExchange]\n  pkce: true\n  anonymous_surface: true\n  self_service_signup: false\nschemes:\n- name: KeyAuthentication\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api-key>'\n  description: Token-based authentication with required prefix \"Token \"\n  sources: [openapi/edf-energy-kraken-openapi.yml]\n- name: DRFKrakenTokenAuthentication\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: Kraken JWT\n  description: JWT-based authentication\n  sources:\n  - openapi/edf-energy-kraken-openapi.yml\n  - openapi/edf-energy-kraken-data-import-openapi.yml\n- name: DataImportViewerAPIKeyAuthentication\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api-key>'\n  description: Token-based authentication with required prefix \"Token \" (data-import viewer)\n  sources: [openapi/edf-energy-kraken-data-import-openapi.yml]\n- name: AccountUserAPIKeyAuthentication\n  type: http\n  scheme: basic\n  description:\
  \ Token-based authentication where the token is passed as the username for basic auth\n  sources: [openapi/edf-energy-kraken-openapi.yml]\n- name: AffiliateAuthentication\n  type: http\n  scheme: basic\n  description: Basic authentication for affiliate organisations\n  sources: [openapi/edf-energy-kraken-openapi.yml]\n- name: PartnerUserOnlyAuthentication\n  type: http\n  scheme: basic\n  description: Basic authentication for partner organisations\n  sources: [openapi/edf-energy-kraken-openapi.yml]\n- name: KrakenOAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorisation server for delegated third-party access to customer-scoped\n    data. Not declared in the OpenAPI documents; documented on the auth server itself\n    and discoverable via OpenID Connect metadata.\n  flows:\n  - flow: authorizationCode\n    pkce: true\n    code_challenge_method: S256\n    authorizationUrl: https://auth.edfgb-kraken.energy/authorize/\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n \
  \ - flow: clientCredentials\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n    client_auth: HTTP Basic (base64 client_id:client_secret)\n  - flow: deviceCode\n    rfc: RFC 8628\n    deviceAuthorizationUrl: https://auth.edfgb-kraken.energy/device-authorization/\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n  - flow: tokenExchange\n    rfc: RFC 8693\n    tokenUrl: https://auth.edfgb-kraken.energy/token/\n  scopes: scopes/edf-energy-scopes.yml\n  sources: [https://auth.edfgb-kraken.energy/]\n- name: KrakenOpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.edfgb-kraken.energy/.well-known/openid-configuration\n  issuer: https://auth.edfgb-kraken.energy/token/\n  jwks_uri: https://auth.edfgb-kraken.energy/.well-known/jwks.json\n  id_token_signing_alg_values_supported: [HS256, RS256]\n  token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n  subject_types_supported: [public]\n  claims_supported: [sub]\n  userinfo_endpoint: https://auth.edfgb-kraken.energy/userinfo/\n\
  \  revocation_endpoint: https://auth.edfgb-kraken.energy/revoke-token/\n  end_session_endpoint: https://auth.edfgb-kraken.energy/logout/\n  sources: [well-known/edf-energy-openid-configuration.json]\nanonymous_operations:\n- operation: List Products\n  path: GET /v1/products/\n  source: openapi/edf-energy-kraken-openapi.yml\n  evidence: security includes an empty option; returned HTTP 200 with 21 live products anonymously\n- operation: List Industry Grid Supply Points\n  path: GET /v1/industry/grid-supply-points/\n  source: openapi/edf-energy-kraken-openapi.yml\n  evidence: resolved postcode SW1A1AA to GSP group _C anonymously (HTTP 200)\n- operation: energyProducts\n  path: POST /v1/graphql/\n  source: graphql/edf-energy-schema.graphql\n  evidence: returned live EDF tariffs anonymously with brand \"EDF\" (HTTP 200)\n- operation: IntrospectionQuery\n  path: POST /v1/graphql/\n  source: graphql/edf-energy-schema.graphql\n  evidence: full GraphQL introspection returned HTTP 200 with no credential\n\
  errors:\n  missing_header: KT-CT-1112 — 'Authorization' header not provided\n  unauthorized: KT-CT-1111 / KT-CT-1132 — the viewer is not authorized to execute the query/mutation\n  expired_token: KT-CT-1120 — the Kraken Token has expired\n  catalog: errors/edf-energy-error-codes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edf-energy/refs/heads/main/authentication/edf-energy-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 8 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Retailer
- Energy Supplier
- Smart Metering
- Nuclear
- Renewables
- EV Charging
- Demand Response
- Tariffs
- Energy Markets
---
