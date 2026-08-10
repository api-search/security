---
api_key_in: []
api_specs:
- filename: umbra-client-credentials-api-openapi.yml
  format: yaml
  label: Umbra Client Credentials API
  slug: umbra-client-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-client-credentials-api-openapi.yml
- filename: umbra-collections-api-openapi.yml
  format: yaml
  label: Umbra Collections API
  slug: umbra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collections-api-openapi.yml
- filename: umbra-collectmetadata-api-openapi.yml
  format: yaml
  label: Umbra Collect Metadata API
  slug: umbra-collectmetadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collectmetadata-api-openapi.yml
- filename: umbra-collects-api-openapi.yml
  format: yaml
  label: Umbra Collects API
  slug: umbra-collects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collects-api-openapi.yml
- filename: umbra-deliveryconfig-api-openapi.yml
  format: yaml
  label: Umbra Delivery Config API
  slug: umbra-deliveryconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-deliveryconfig-api-openapi.yml
- filename: umbra-feasibility-api-openapi.yml
  format: yaml
  label: Umbra Feasibility API
  slug: umbra-feasibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-feasibility-api-openapi.yml
- filename: umbra-organizations-api-openapi.yml
  format: yaml
  label: Umbra Organizations API
  slug: umbra-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-organizations-api-openapi.yml
- filename: umbra-preview-api-openapi.yml
  format: yaml
  label: Umbra Preview API
  slug: umbra-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-api-openapi.yml
- filename: umbra-preview-image-api-openapi.yml
  format: yaml
  label: Umbra Preview Image API
  slug: umbra-preview-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-image-api-openapi.yml
- filename: umbra-product-constraints-api-openapi.yml
  format: yaml
  label: Umbra Product Constraints API
  slug: umbra-product-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-product-constraints-api-openapi.yml
- filename: umbra-restricted-access-areas-api-openapi.yml
  format: yaml
  label: Umbra Restricted Access Areas API
  slug: umbra-restricted-access-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-restricted-access-areas-api-openapi.yml
- filename: umbra-search-api-openapi.yml
  format: yaml
  label: Umbra Search API
  slug: umbra-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-search-api-openapi.yml
- filename: umbra-tasks-api-openapi.yml
  format: yaml
  label: Umbra Tasks API
  slug: umbra-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-tasks-api-openapi.yml
- filename: umbra-thumbnail-api-openapi.yml
  format: yaml
  label: Umbra Thumbnail API
  slug: umbra-thumbnail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-thumbnail-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Umbra Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Umbra secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Umbra
provider_slug: umbra
scheme_count: 2
schemes:
- applied_to: every operation across all six Canopy OpenAPI documents
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/umbra-admin-openapi.yml
  - openapi/umbra-delivery-openapi.yml
  - openapi/umbra-stac-api-v2-openapi.yml
  - openapi/umbra-stac-archive-openapi.yml
  - openapi/umbra-tasking-openapi.yml
  - openapi/umbra-tiles-openapi.yml
  type: http
- audience_required: true
  audiences:
  - environment: live
    value: https://api.canopy.umbra.space
  - environment: sandbox
    value: https://api.canopy.prod.umbra-sandbox.space
  expires_in: 86400
  flow: clientCredentials
  identity_provider: Auth0
  issuer: https://auth.canopy.umbra.space/
  jwks_uri: https://auth.canopy.umbra.space/.well-known/jwks.json
  name: Canopy OAuth2 client credentials
  request_content_type: application/json
  sources:
  - https://docs.canopy.umbra.space/docs/authentication-via-client-credentials
  - well-known/umbra-oauth-authorization-server.json
  - well-known/umbra-openid-configuration.json
  token_type: Bearer
  token_url: https://auth.canopy.umbra.space/oauth/token
  type: oauth2
slug: umbra-authentication
source_filename: umbra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/ (all six documents) + the Canopy authentication docs + Auth0 discovery documents\ndocs: https://docs.canopy.umbra.space/docs/authenticate\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_flows: [clientCredentials]\n  note: >-\n    The OpenAPI documents declare only the resulting bearer token (securityScheme `bearerAuth`,\n    http/bearer/JWT, applied to every operation in all six specs). The OAuth2 client-credentials\n    exchange that mints that token is documented in prose and confirmed by the RFC 8414 / OIDC\n    discovery documents on auth.canopy.umbra.space, but is not modelled in any spec — so a\n    spec-only read understates Canopy's auth posture.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied_to: every operation across all six Canopy OpenAPI documents\n  sources:\n  - openapi/umbra-admin-openapi.yml\n  - openapi/umbra-delivery-openapi.yml\n\
  \  - openapi/umbra-stac-api-v2-openapi.yml\n  - openapi/umbra-stac-archive-openapi.yml\n  - openapi/umbra-tasking-openapi.yml\n  - openapi/umbra-tiles-openapi.yml\n- name: Canopy OAuth2 client credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.canopy.umbra.space/oauth/token\n  issuer: https://auth.canopy.umbra.space/\n  jwks_uri: https://auth.canopy.umbra.space/.well-known/jwks.json\n  identity_provider: Auth0\n  request_content_type: application/json\n  audience_required: true\n  audiences:\n  - value: https://api.canopy.umbra.space\n    environment: live\n  - value: https://api.canopy.prod.umbra-sandbox.space\n    environment: sandbox\n  token_type: Bearer\n  expires_in: 86400\n  sources:\n  - https://docs.canopy.umbra.space/docs/authentication-via-client-credentials\n  - well-known/umbra-oauth-authorization-server.json\n  - well-known/umbra-openid-configuration.json\ntoken_acquisition:\n- method: ui-generated temporary access token\n  docs: https://docs.canopy.umbra.space/docs/authentication\n\
  \  where: https://canopy.umbra.space/account\n  lifetime: 24 hours\n  note: >-\n    Copied by hand from the Canopy account page. Valid for multiple requests. Toggling \"Test Mode\"\n    in the app header yields the sandbox-scoped equivalent.\n- method: oauth2 client credentials\n  docs: https://docs.canopy.umbra.space/docs/authentication-via-client-credentials\n  where: Canopy Organization page, Authentication tab\n  lifetime: 86400 seconds\n  intended_for: scripts and applications that cannot do interactive login\n  credential_scope: organization\n  note: >-\n    Each organization has ONE shared client_id/client_secret pair that any user in the org can\n    rotate or delete, and rotating it affects every user and application in that organization.\n    Credentials are also managed through the Admin API (create_token, get_token, rotate_token,\n    delete_token).\nusage:\n  header: 'Authorization: Bearer <access_token>'\n  expiry_behavior: >-\n    Expired tokens produce HTTP 401. Umbra directs\
  \ clients to catch the 401, request a new token\n    and retry, or to refresh proactively just before expiry.\ntoken_exchange_rate_limit:\n  limit: 50\n  window: rolling 24 hours\n  scope: per client\n  rationale: to force token caching and reuse rather than a token exchange per API call\n  claims:\n  - name: https://umbra.space/rate_limit\n    type: int\n    description: the configured token-exchange rate limit per 24-hour period for the client\n  - name: https://umbra.space/rate_limit_remaining\n    type: int\n    description: auth requests remaining in the current interval\n  gotcha: >-\n    When the token-exchange rate limit is hit, the authentication provider returns HTTP 400, not\n    429. Clients must inspect response.error_description.code for the value 429 to detect it.\n    error_description also carries rate_limit and rate_limit_refresh (an ISO timestamp for the\n    next allowed exchange).\nauthorization_model:\n  granularity: per organization\n  scopes: >-\n    Canopy publishes\
  \ no API-specific OAuth scope vocabulary. Access is determined by the\n    organization the credential belongs to and by that organization's contract and product\n    constraints, not by scopes carried on the token. See scopes/umbra-scopes.yml.\n  environment_isolation: >-\n    Live and sandbox are entirely isolated. A token minted for one audience cannot query the other.\n  restricted_access_areas: >-\n    Tasking is additionally constrained by an organization-specific geofence, retrievable as GeoJSON\n    via the get_restricted_access_areas operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/authentication/umbra-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Satellite Imagery
- Synthetic Aperture Radar
- Earth Observation
- Geospatial
- Space
- STAC
- Remote Sensing
- Tasking
- Defense and Intelligence
- Company
---
