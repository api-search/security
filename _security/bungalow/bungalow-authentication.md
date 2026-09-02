---
api_key_in: []
api_specs:
- filename: bungalow-applications-api-openapi.yml
  format: yaml
  label: Bungalow Applications API
  slug: bungalow-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-applications-api-openapi.yml
- filename: bungalow-listings-api-openapi.yml
  format: yaml
  label: Bungalow Listings API
  slug: bungalow-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-listings-api-openapi.yml
- filename: bungalow-markets-api-openapi.yml
  format: yaml
  label: Bungalow Markets API
  slug: bungalow-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-markets-api-openapi.yml
- filename: bungalow-showings-api-openapi.yml
  format: yaml
  label: Bungalow Showings API
  slug: bungalow-showings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-showings-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Bungalow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bungalow secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bungalow
provider_slug: bungalow
scheme_count: 0
schemes: []
slug: bungalow-authentication
source_filename: bungalow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://fieldstone.bungalow.com/api/v1/docs/\ndocs: https://fieldstone.bungalow.com/api/v1/docs/#section/Getting-Started\nnote: >-\n  The Bungalow OpenAPI declares no components.securitySchemes, so the mechanical derive produced\n  nothing. This profile is SEARCHED from the published API documentation and confirmed by live\n  anonymous calls: the public JSON API is unauthenticated. The docs' error reference does describe\n  bearer access/refresh tokens (AuthenticationFailed, NotAuthenticated, InvalidToken), which apply to\n  Bungalow's non-public/authenticated surfaces (the partner XML feeds and the resident/homeowner\n  product), not to the seven published listings operations.\nsummary:\n  types: [none]\n  public_api_authentication: none\n  api_key_in: []\n  oauth2_flows: []\n  partner_surfaces_authenticated: true\nschemes: []\nsurfaces:\n- name: Public JSON API\n  base_url: https://fieldstone.bungalow.com/api/v1/\n  authentication:\
  \ none\n  evidence:\n    verified: '2026-08-01'\n    request: GET https://fieldstone.bungalow.com/api/v1/markets/?limit=3\n    http_status: 200\n    content_type: application/json\n    note: 200 returned with no Authorization header and no cookie.\n  operations:\n  - /markets/\n  - /markets/{id}\n  - /listings/properties/\n  - /listings/properties/{id_or_slug}\n  - /listings/showings/availability/{id}/\n  - /listings/showings/\n  - /applications/source/\n- name: Partner XML feeds (Hotpads / Facebook Catalog)\n  authentication: partner-provisioned\n  onboarding: email integrations@bungalow.com with intended use and desired format\n  note: >-\n    \"Since they are authenticated, we can provide a broader range of fields than the public JSON API\n    does.\" Credential type is not published. MITS format is listed as possible future support.\n  formats: [hotpads, facebook-catalog]\n  source: https://fieldstone.bungalow.com/api/v1/docs/#section/Getting-Started\n- name: Lead-capture webhook (partner\
  \ -> Bungalow)\n  authentication: partner-provisioned\n  onboarding: email integrations@bungalow.com to have a webhook configured for your platform\n  source: https://fieldstone.bungalow.com/api/v1/docs/#section/Getting-Started\ndocumented_auth_errors:\n- type: AuthenticationFailed\n  status: 401\n  message: Incorrect authentication credentials.\n- type: NotAuthenticated\n  status: 401\n  message: Authentication credentials were not provided.\n  note: A WWW-Authenticate header is returned indicating how to authenticate.\n- type: InvalidToken\n  status: 401\n  message: The refresh or access token provided has expired or is malformed.\n  note: Refresh-token rotation is documented — use the refresh token to mint a new access token.\n- type: PermissionDenied\n  status: 403\n  message: You do not have permission to perform this action.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/authentication/bungalow-authentication.yml
summary_line: none · 0 schemes
tags:
- Company
- Real-Estate
- Residential Real Estate
- Rental Listings
- Property Management
- Co-Living
- Single-Family Rental
- Listings Syndication
- Housing
- PropTech
- Marketplace
---
