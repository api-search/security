---
anonymous_access: false
api_key_in: []
api_specs:
- filename: channelseal-platform-api-openapi.yml
  format: yaml
  label: ChannelSeal Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-platform-api-openapi.yml
- filename: channelseal-api-discovery-service-api-openapi.yml
  format: yaml
  label: ChannelSeal API Discovery Service API
  slug: api-discovery-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-api-discovery-service-api-openapi.yml
- filename: channelseal-api-catalog-api-openapi.yml
  format: yaml
  label: ChannelSeal API Catalog API
  slug: api-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-api-catalog-api-openapi.yml
- filename: channelseal-data-classification-api-openapi.yml
  format: yaml
  label: ChannelSeal Data Classification API
  slug: data-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/openapi/channelseal-data-classification-api-openapi.yml
auth_types:
- oauth2
description: 'Every ChannelSeal API request is authenticated with an OAuth 2.0 client-credentials access token (RFC 6749 §4.4) presented as a Bearer token. Clients are created in the ChannelSeal Portal under Settings → API Credentials; tokens are minted by the provider''s Auth0 tenant (https://dev-channelseal.us.auth0.com/oauth/token) with audience https://api.channelseal.com and expire after 3600 seconds. Note the spec-level defect: four of the five OpenAPI documents declare the scheme under components.schemas.securitySchemes (a schema named "securitySchemes") rather than components.securitySchemes, and none applies a security[] requirement to any operation, so a generic OpenAPI client would treat every operation as anonymous. Only the shared-components document declares it correctly. The docs, not the contract, are the authority for auth here.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Channelseal Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ChannelSeal secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ChannelSeal
provider_slug: channelseal
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 5
    scopes_detail: scopes/channelseal-scopes.yml
    tokenUrl: https://dev-channelseal.us.auth0.com/oauth/token
  name: security_auth
  sources:
  - openapi/channelseal-api-schemas-openapi.yml
  - https://docs.channelseal.com/api-reference#authentication
  type: oauth2
slug: channelseal-authentication
source_filename: channelseal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: openapi/channelseal-api-schemas-openapi.yml\ndocs: https://docs.channelseal.com/api-reference#authentication\ndescription: >-\n  Every ChannelSeal API request is authenticated with an OAuth 2.0 client-credentials access token\n  (RFC 6749 §4.4) presented as a Bearer token. Clients are created in the ChannelSeal Portal under\n  Settings → API Credentials; tokens are minted by the provider's Auth0 tenant\n  (https://dev-channelseal.us.auth0.com/oauth/token) with audience https://api.channelseal.com and\n  expire after 3600 seconds. Note the spec-level defect: four of the five OpenAPI documents declare the\n  scheme under components.schemas.securitySchemes (a schema named \"securitySchemes\") rather than\n  components.securitySchemes, and none applies a security[] requirement to any operation, so a generic\n  OpenAPI client would treat every operation as anonymous. Only the shared-components document declares\n  it correctly.\
  \ The docs, not the contract, are the authority for auth here.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_location: Authorization header, Bearer scheme\n  token_lifetime_seconds: 3600\n  issuer: https://dev-channelseal.us.auth0.com/\n  audience: https://api.channelseal.com\n  https_required: true\nschemes:\n- name: security_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://dev-channelseal.us.auth0.com/oauth/token\n    scopes: 5\n    scopes_detail: scopes/channelseal-scopes.yml\n  sources:\n  - openapi/channelseal-api-schemas-openapi.yml\n  - https://docs.channelseal.com/api-reference#authentication\nissuer_metadata:\n  openid_configuration: well-known/channelseal-auth0-openid-configuration.json\n  oauth_authorization_server: well-known/channelseal-auth0-oauth-authorization-server.json\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  grant_types_supported_relevant:\
  \ [client_credentials, authorization_code, refresh_token, device_code, token-exchange, jwt-bearer]\n  registration_endpoint: https://dev-channelseal.us.auth0.com/oidc/register\n  code_challenge_methods_supported: [S256, plain]\ncredential_issuance:\n  where: ChannelSeal Portal → Settings → API Credentials → Create OAuth Client\n  self_service: true\n  note: The platform is invite-only (founding-customer program) so a portal account precedes any credential.\nerror_semantics:\n  '401': The access token is invalid or has expired (application/problem+json, type https://api.channelseal.com/problems/unauthorized)\n  '403': Insufficient permissions; the problem detail names the required scope\nnotes:\n- The issuer is a tenant literally named dev-channelseal on Auth0's shared us.auth0.com domain, yet the docs present it as the production token endpoint.\n- The production API host (api.channelseal.com) named as audience and server did not resolve in DNS on 2026-09-20; staging.channelseal.com enforces\
  \ the bearer requirement live (401 on /platform/api/v1/apis without a token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelseal/refs/heads/main/authentication/channelseal-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- API Security
- AI Agents
- MCP
- Data Classification
- API Discovery
- Non-Human Identity
- Sensitive Data
- Observability
- OpenTelemetry
- Governance
---
