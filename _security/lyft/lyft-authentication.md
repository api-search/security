---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lyft-concierge-rides-api-openapi.yml
  format: yaml
  label: lyft Concierge Rides API
  slug: lyft-concierge-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-concierge-rides-api-openapi.yml
- filename: lyft-cost-estimates-api-openapi.yml
  format: yaml
  label: lyft Cost Estimates API
  slug: lyft-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-cost-estimates-api-openapi.yml
- filename: lyft-drivers-api-openapi.yml
  format: yaml
  label: lyft Drivers API
  slug: lyft-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-drivers-api-openapi.yml
- filename: lyft-eta-api-openapi.yml
  format: yaml
  label: lyft ETA API
  slug: lyft-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-eta-api-openapi.yml
- filename: lyft-profile-api-openapi.yml
  format: yaml
  label: lyft Profile API
  slug: lyft-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-profile-api-openapi.yml
- filename: lyft-ride-types-api-openapi.yml
  format: yaml
  label: lyft Ride Types API
  slug: lyft-ride-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-ride-types-api-openapi.yml
- filename: lyft-rides-api-openapi.yml
  format: yaml
  label: lyft Rides API
  slug: lyft-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-rides-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Lyft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lyft secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lyft
provider_slug: lyft
scheme_count: 2
schemes:
- description: OAuth 2.0 access token obtained through the client credentials flow for the organization's concierge API client.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lyft-concierge-rides-api-openapi.yml
  - openapi/lyft-cost-estimates-api-openapi.yml
  - openapi/lyft-drivers-api-openapi.yml
  - openapi/lyft-eta-api-openapi.yml
  - openapi/lyft-profile-api-openapi.yml
  - openapi/lyft-ride-types-api-openapi.yml
  - openapi/lyft-rides-api-openapi.yml
  type: http
- description: Client token for accessing public endpoints without user authorization. Passed as a Bearer token in the Authorization header.
  in: header
  name: clientToken
  parameter: Authorization
  sources:
  - openapi/lyft-cost-estimates-api-openapi.yml
  - openapi/lyft-drivers-api-openapi.yml
  - openapi/lyft-eta-api-openapi.yml
  - openapi/lyft-profile-api-openapi.yml
  - openapi/lyft-ride-types-api-openapi.yml
  - openapi/lyft-rides-api-openapi.yml
  type: apiKey
slug: lyft-authentication
source_filename: lyft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://api.lyft.com/.well-known/oauth-authorization-server (live RFC 8414 metadata) + openapi/lyft-concierge-rides-api-openapi.yml,\n  openapi/lyft-cost-estimates-api-openapi.yml, openapi/lyft-drivers-api-openapi.yml, openapi/lyft-eta-api-openapi.yml,\n  openapi/lyft-profile-api-openapi.yml, openapi/lyft-ride-types-api-openapi.yml, openapi/lyft-rides-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained through the client credentials flow for the organization's concierge\n    API client.\n  sources:\n  - openapi/lyft-concierge-rides-api-openapi.yml\n  - openapi/lyft-cost-estimates-api-openapi.yml\n  - openapi/lyft-drivers-api-openapi.yml\n  - openapi/lyft-eta-api-openapi.yml\n  - openapi/lyft-profile-api-openapi.yml\n  - openapi/lyft-ride-types-api-openapi.yml\n  - openapi/lyft-rides-api-openapi.yml\n\
  - name: clientToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Client token for accessing public endpoints without user authorization. Passed as a Bearer token\n    in the Authorization header.\n  sources:\n  - openapi/lyft-cost-estimates-api-openapi.yml\n  - openapi/lyft-drivers-api-openapi.yml\n  - openapi/lyft-eta-api-openapi.yml\n  - openapi/lyft-profile-api-openapi.yml\n  - openapi/lyft-ride-types-api-openapi.yml\n  - openapi/lyft-rides-api-openapi.yml\noauth:\n  issuer: https://api.lyft.com\n  authorization_endpoint: https://api.lyft.com/oauth/authorize\n  token_endpoint: https://api.lyft.com/oauth/token\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - none\n  code_challenge_methods_supported:\n  - S256\n  pkce: 'S256 required for public clients (code_challenge_methods_supported: [S256]); token_endpoint_auth_methods_supported\n\
  \    includes \"none\", which is the public-client case PKCE protects'\n  scope_count: 47\n  scopes: scopes/lyft-scopes.yml\n  discovery_document: well-known/lyft-oauth-authorization-server.json\n  metadata_spec: RFC 8414\n  source: https://api.lyft.com/.well-known/oauth-authorization-server\nflows:\n- name: client_credentials\n  use: Two-legged, for public endpoints that need no user context (cost, eta, ridetypes, drivers). Matches the clientToken\n    scheme in the specs.\n  evidence: https://api.lyft.com/.well-known/oauth-authorization-server\n- name: authorization_code\n  use: Three-legged, for user-context endpoints (profile, rides) and the concierge surface.\n  evidence: https://api.lyft.com/.well-known/oauth-authorization-server\n- name: refresh_token\n  use: Token renewal; the published vocabulary includes an \"offline\" scope.\n  evidence: https://api.lyft.com/.well-known/oauth-authorization-server\nopenid_connect:\n  scopes_advertised:\n  - openid\n  - profile\n  - profile.email\n\
  \  - profile.phone\n  discovery_document_served: false\n  evidence: GET https://api.lyft.com/.well-known/openid-configuration -> 404 on 2026-09-17, while the OAuth 2.0\n    metadata document at the sibling path returns 200.\n  note: OIDC scopes are advertised without an OIDC discovery document, so a client cannot resolve jwks_uri or userinfo_endpoint\n    anonymously.\ndocs: null\ndocs_note: Lyft publishes no anonymously readable authentication reference. https://www.lyft.com/developers 302s\n  to https://account.lyft.com/auth/email; developer.lyft.com (cited by every Lyft SDK README) is NXDOMAIN.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/authentication/lyft-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Transportation
- Mobility
- Ride Hailing
- Micromobility
- Bike Share
- Scooters
- GBFS
- Logistics
- Travel
---
