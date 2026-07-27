---
api_key_in:
- header
- query
- path
api_specs:
- filename: hometrack-valuation-api-v1-openapi.yml
  format: yaml
  label: Hometrack Valuation API
  slug: hometrack-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-valuation-api-v1-openapi.yml
- filename: hometrack-broker-avm-api-openapi.yml
  format: yaml
  label: Hometrack Broker AVM API
  slug: hometrack-broker-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-broker-avm-api-openapi.yml
- filename: hometrack-prh-core-external-client-api-v2-openapi.yml
  format: yaml
  label: Hometrack PRH Core External Client API v2.0
  slug: hometrack-prh-core-external-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-prh-core-external-client-api-v2-openapi.yml
- filename: hometrack-climate-api-v2-openapi.yml
  format: yaml
  label: Hometrack Climate API (v2)
  slug: hometrack-climate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-api-v2-openapi.yml
- filename: hometrack-climate-graphql-api-openapi.yml
  format: yaml
  label: Hometrack Climate GraphQL API
  slug: hometrack-climate-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-climate-graphql-api-openapi.yml
- filename: hometrack-api-public-openapi.yml
  format: yaml
  label: Hometrack API Public
  slug: hometrack-api-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/openapi/hometrack-api-public-openapi.yml
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Hometrack Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hometrack secures its APIs with oauth2, apiKey, and http across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hometrack
provider_slug: hometrack
scheme_count: 5
schemes:
- audience: https://api.hometrack.com
  flow: clientCredentials
  name: OAuth2ClientCredentials
  note: Documented on the portal but NOT declared in any harvested OpenAPI — the APIM export emits only the gateway subscription-key schemes. This is a genuine spec/doc divergence worth reporting to Hometrack.
  scopes:
  - read:valuations
  - write:valuations
  sources:
  - https://developer.hometrack.com/api-authentication
  tokenUrl: https://hometrack-prod.eu.auth0.com/oauth/token
  type: oauth2
- in: header
  layer: azure-api-management
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/hometrack-api-public-openapi.yml
  - openapi/hometrack-broker-avm-api-openapi.yml
  - openapi/hometrack-climate-api-v2-openapi.yml
  - openapi/hometrack-climate-graphql-api-openapi.yml
  - openapi/hometrack-prh-core-external-client-api-v2-openapi.yml
  - openapi/hometrack-valuation-api-v1-openapi.yml
  type: apiKey
- in: query
  layer: azure-api-management
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/hometrack-api-public-openapi.yml
  - openapi/hometrack-broker-avm-api-openapi.yml
  - openapi/hometrack-climate-api-v2-openapi.yml
  - openapi/hometrack-climate-graphql-api-openapi.yml
  - openapi/hometrack-prh-core-external-client-api-v2-openapi.yml
  - openapi/hometrack-valuation-api-v1-openapi.yml
  type: apiKey
- exchange_operation: openapi/hometrack-valuation-api-v1-openapi.yml#authentication
  format: Token token="<guid>"
  in: header
  name: ValuationApiToken
  note: POST /authentication/{apiKey} returns a temporary token "valid for 5 minutes". The spec documents that the header is also accepted without the quotes and without the `token=` prefix.
  parameter: Authorization
  scheme: Token
  sources:
  - openapi/hometrack-valuation-api-v1-openapi.yml
  ttl_seconds: 300
  type: http
- exchange_operation: openapi/hometrack-api-public-openapi.yml#AuthenticationApi_Post
  in: path
  name: PublicApiPathToken
  note: POST /api/authentication/{apiKey} returns a plain-text GUID token that is then passed as a URL path segment on the reporting, brands, licences, partners, pvrplugin and trial operations. Credentials in the path are logged by intermediaries — recorded as an observed design weakness, not a recommendation.
  parameter: token
  sources:
  - openapi/hometrack-api-public-openapi.yml
  type: apiKey
slug: hometrack-authentication
source_filename: hometrack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\ndocs: https://developer.hometrack.com/api-authentication\nsource: >-\n  https://developer.hometrack.com/api-authentication (OAuth 2.0 client\n  credentials via Auth0) + the Auth0 tenant discovery documents in well-known/ +\n  the security schemes declared across all six OpenAPI documents in openapi/ +\n  live anonymous probes of api.hometrack.com.\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header, query, path]\n  oauth2_flows: [clientCredentials]\n  gate: >-\n    Three distinct credential mechanisms sit in front of Hometrack's APIs and\n    they are not alternatives — they are layers from different eras of the\n    platform. (1) OAuth 2.0 client credentials against Hometrack's Auth0 tenant\n    is the documented, current way to authenticate; the bearer token is\n    presented to api.hometrack.com. (2) Every harvested OpenAPI additionally\n    declares Azure API Management subscription-key schemes\n    (Ocp-Apim-Subscription-Key\
  \ header / subscription-key query), which is the\n    gateway product key. (3) Two older APIs carry their own bespoke token\n    exchange in the contract itself: the Valuation API exchanges an API key for\n    a five-minute token used as `Authorization: Token token=\"<guid>\"`, and the\n    Hometrack API Public exchanges an API key for a plain-text GUID passed as a\n    {token} path segment on nearly every operation. No credential of any kind is\n    self-service — the portal directs you to a sales contact form.\noauth2:\n  documented: true\n  docs: https://developer.hometrack.com/api-authentication\n  provider: Auth0\n  tenant: https://hometrack-prod.eu.auth0.com/\n  issuer: https://hometrack-prod.eu.auth0.com/\n  token_endpoint: https://hometrack-prod.eu.auth0.com/oauth/token\n  jwks_uri: https://hometrack-prod.eu.auth0.com/.well-known/jwks.json\n  grant_type: client_credentials\n  audience: https://api.hometrack.com\n  request_body_fields: [client_id, client_secret, audience, grant_type]\n\
  \  token_type: Bearer\n  expires_in: 86400\n  token_lifetime_note: '\"The access token is valid for 24 hours.\"'\n  example_scope: read:valuations write:valuations\n  usage: 'Authorization: Bearer <access_token>'\n  discovery:\n    openid_configuration: well-known/hometrack-auth0-openid-configuration.json\n    oauth_authorization_server: well-known/hometrack-auth0-oauth-authorization-server.json\n    jwks: well-known/hometrack-auth0-jwks.json\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  dpop_signing_alg_values_supported: [ES256]\n  note: >-\n    grant_types_supported on the tenant lists many Auth0 grants; only\n    client_credentials is documented for API access, because the audience\n    https://api.hometrack.com is a machine-to-machine API, not an end-user login.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl:\
  \ https://hometrack-prod.eu.auth0.com/oauth/token\n  audience: https://api.hometrack.com\n  scopes: [read:valuations, write:valuations]\n  sources: [https://developer.hometrack.com/api-authentication]\n  note: >-\n    Documented on the portal but NOT declared in any harvested OpenAPI — the\n    APIM export emits only the gateway subscription-key schemes. This is a\n    genuine spec/doc divergence worth reporting to Hometrack.\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  layer: azure-api-management\n  sources:\n  - openapi/hometrack-api-public-openapi.yml\n  - openapi/hometrack-broker-avm-api-openapi.yml\n  - openapi/hometrack-climate-api-v2-openapi.yml\n  - openapi/hometrack-climate-graphql-api-openapi.yml\n  - openapi/hometrack-prh-core-external-client-api-v2-openapi.yml\n  - openapi/hometrack-valuation-api-v1-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  layer: azure-api-management\n \
  \ sources:\n  - openapi/hometrack-api-public-openapi.yml\n  - openapi/hometrack-broker-avm-api-openapi.yml\n  - openapi/hometrack-climate-api-v2-openapi.yml\n  - openapi/hometrack-climate-graphql-api-openapi.yml\n  - openapi/hometrack-prh-core-external-client-api-v2-openapi.yml\n  - openapi/hometrack-valuation-api-v1-openapi.yml\n- name: ValuationApiToken\n  type: http\n  scheme: Token\n  in: header\n  parameter: Authorization\n  format: 'Token token=\"<guid>\"'\n  ttl_seconds: 300\n  exchange_operation: openapi/hometrack-valuation-api-v1-openapi.yml#authentication\n  sources: [openapi/hometrack-valuation-api-v1-openapi.yml]\n  note: >-\n    POST /authentication/{apiKey} returns a temporary token \"valid for 5\n    minutes\". The spec documents that the header is also accepted without the\n    quotes and without the `token=` prefix.\n- name: PublicApiPathToken\n  type: apiKey\n  in: path\n  parameter: token\n  exchange_operation: openapi/hometrack-api-public-openapi.yml#AuthenticationApi_Post\n\
  \  sources: [openapi/hometrack-api-public-openapi.yml]\n  note: >-\n    POST /api/authentication/{apiKey} returns a plain-text GUID token that is\n    then passed as a URL path segment on the reporting, brands, licences,\n    partners, pvrplugin and trial operations. Credentials in the path are\n    logged by intermediaries — recorded as an observed design weakness, not a\n    recommendation.\nprobes:\n- {url: 'https://api.hometrack.com/valuation/v2/broker/order/1', anonymous: true, status: 401, body: '{\"statusCode\": 401, \"message\": \"Unauthorized. Access token is missing or invalid.\"}'}\n- {url: 'https://api.hometrack.com/climate/graphql', anonymous: true, method: POST, status: 401, body: '{\"statusCode\": 401, \"message\": \"Unauthorized. Access token is missing or invalid.\"}'}\n- {url: 'https://api.hometrack.com/valuation-api/v1/status', anonymous: true, status: 200, body: '(zero bytes)'}\nonboarding:\n  self_service: false\n  path: https://www.hometrack.com/uk/#contactus\n  verbatim:\
  \ >-\n    \"To interact with any of our APIs you will need to have a valid API Key for\n    that respective product. If you do not yet have an API Key, please contact\n    us.\"\ncross_links:\n  scopes: scopes/hometrack-scopes.yml\n  well_known: well-known/hometrack-well-known.yml\n  conventions: conventions/hometrack-conventions.yml\n  conformance: conformance/hometrack-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hometrack/refs/heads/main/authentication/hometrack-authentication.yml
summary_line: oauth2/apiKey/http · 5 schemes
tags:
- Real Estate
- United Kingdom
- PropTech
- Valuation
- AVM
- Mortgage
- Property Data
- Climate Risk
- Lending
- Surveying
---
