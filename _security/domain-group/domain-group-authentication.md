---
api_key_in:
- header
api_specs:
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Address Suggestions API
  slug: domain-address-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Agents & Listings API
  slug: domain-agents-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API
  slug: domain-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API - Preview
  slug: domain-campaign-api-preview
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Listings Management API
  slug: domain-listings-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Price Estimation API
  slug: domain-price-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Properties & Locations API
  slug: domain-properties-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Enrichment API
  slug: domain-property-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Package API
  slug: domain-property-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain PropertyRadar API
  slug: domain-propertyradar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Rental AVM API
  slug: domain-rental-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Schools Data API
  slug: domain-schools-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Webhooks API
  slug: domain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Domain Group Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Domain Group secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Domain Group
provider_slug: domain-group
scheme_count: 2
schemes:
- description: API Key in Header
  in: header
  name: apikey
  parameter: x-api-key
  sources:
  - openapi/domain-group-openapi-latest.json
  - openapi/domain-group-openapi-v1.json
  - openapi/domain-group-openapi-v2.json
  type: apiKey
- description: OAuth 2
  flows:
  - flow: clientCredentials
    scopes: 25
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  - authorizationUrl: https://auth.domain.com.au/v1/connect/authorize
    flow: authorizationCode
    scopes: 25
    tokenUrl: https://auth.domain.com.au/v1/connect/token
  name: oauth2
  sources:
  - openapi/domain-group-openapi-latest.json
  - openapi/domain-group-openapi-v1.json
  - openapi/domain-group-openapi-v2.json
  type: oauth2
slug: domain-group-authentication
source_filename: domain-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/domain-group-openapi-latest.json, openapi/domain-group-openapi-v1.json, openapi/domain-group-openapi-v2.json,\n  https://developer.domain.com.au/docs/latest/authentication, well-known/domain-group-openid-configuration.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API Key in Header\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n    scopes: 25\n  - flow: authorizationCode\n    authorizationUrl: https://auth.domain.com.au/v1/connect/authorize\n    tokenUrl: https://auth.domain.com.au/v1/connect/token\n    scopes:\
  \ 25\n  description: OAuth 2\n  sources:\n  - openapi/domain-group-openapi-latest.json\n  - openapi/domain-group-openapi-v1.json\n  - openapi/domain-group-openapi-v2.json\ndocs: https://developer.domain.com.au/docs/latest/authentication\nguidance: 'Domain documents exactly two authentication methods: API Key and OAuth 2.0. Domain recommends\n  OAuth 2.0 wherever the application can securely store a secret server-side. API Keys cannot reach user-specific\n  data at all - any call requiring user context (agency-scoped webhook subscriptions, GET /v1/me and its\n  sub-resources) must use an Authorization Code or Implicit token. No endpoint is reachable until the\n  required API package has been added to the project in the developer portal.'\nidentity_provider:\n  issuer: https://auth.domain.com.au/v1\n  discovery: https://auth.domain.com.au/v1/.well-known/openid-configuration\n  jwks: https://auth.domain.com.au/v1/.well-known/jwks\n  local_discovery: well-known/domain-group-openid-configuration.json\n\
  \  id_token_signing:\n  - RS256\n  pkce:\n  - plain\n  - S256\n  dpop: true\n  par: true\n  ciba: true\n  device_code: true\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  introspection_endpoint: https://auth.domain.com.au/v1/connect/introspect\n  revocation_endpoint: https://auth.domain.com.au/v1/connect/revocation\ntoken_handling:\n  cache: Access tokens must be cached and reused until expiry.\n  authorisation_rate_limit: up to 3000 token requests per hour\n  sla_condition: The 99% uptime / 900ms p95 SLA is conditional on following these authentication best\n    practices.\n  source: https://developer.domain.com.au/docs/latest/conventions/rate-limiting\nflow_selection:\n- flow: clientCredentials\n  use: 'Machine-to-machine reads: properties, listings, market statistics, schools, sales results. No\n    user context.'\n- flow: authorizationCode\n  use: Any call needing user context - agency-scoped webhook subscriptions, GET /v1/me, GET /v1/me/agencies,\n\
  \    GET /v1/me/providers.\n- flow: implicit\n  use: Documented by Domain as an alternative user-context grant; the OpenAPI documents declare clientCredentials\n    and authorizationCode only.\nfailure_diagnostics:\n  header: X-Domain-Security-Reason\n  note: Returned on 401/403 and usually names the cause. See errors/domain-group-problem-types.yml.\n  source: https://developer.domain.com.au/docs/latest/troubleshooting\nenvironments:\n- name: Primary\n  api: https://api.domain.com.au/\n  auth: https://auth.domain.com.au/\n- name: Sandbox\n  api: https://api.domain.com.au/sandbox/\n  auth: https://auth.domain.com.au/\n  note: Auth host is shared; only the API base URL differs.\nscopes_artifact: scopes/domain-group-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/authentication/domain-group-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Real-Estate
- Australia
- Property Listings
- Property Data
- Valuation
- AVM
- Rentals
- Listing Management
- PropTech
- Portal Marketplace
---
