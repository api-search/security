---
api_key_in: []
api_specs:
- filename: navigate-access-codes-api-openapi.yml
  format: yaml
  label: Navigate Access codes API
  slug: navigate-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-access-codes-api-openapi.yml
- filename: navigate-assets-api-openapi.yml
  format: yaml
  label: Navigate Assets API
  slug: navigate-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-assets-api-openapi.yml
- filename: navigate-lennar-api-openapi.yml
  format: yaml
  label: Navigate Lennar API
  slug: navigate-lennar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-lennar-api-openapi.yml
- filename: navigate-line-items-api-openapi.yml
  format: yaml
  label: Navigate Line items API
  slug: navigate-line-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-line-items-api-openapi.yml
- filename: navigate-locations-api-openapi.yml
  format: yaml
  label: Navigate Locations API
  slug: navigate-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-locations-api-openapi.yml
- filename: navigate-markets-api-openapi.yml
  format: yaml
  label: Navigate Markets API
  slug: navigate-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-markets-api-openapi.yml
- filename: navigate-rejection-reason-options-api-openapi.yml
  format: yaml
  label: Navigate Rejection reason options API
  slug: navigate-rejection-reason-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-rejection-reason-options-api-openapi.yml
- filename: navigate-room-types-api-openapi.yml
  format: yaml
  label: Navigate Room types API
  slug: navigate-room-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-room-types-api-openapi.yml
- filename: navigate-rooms-api-openapi.yml
  format: yaml
  label: Navigate Rooms API
  slug: navigate-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-rooms-api-openapi.yml
- filename: navigate-scopes-api-openapi.yml
  format: yaml
  label: Navigate Scopes API
  slug: navigate-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-scopes-api-openapi.yml
- filename: navigate-scoping-api-openapi.yml
  format: yaml
  label: Navigate Scoping API
  slug: navigate-scoping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-scoping-api-openapi.yml
- filename: navigate-vendors-api-openapi.yml
  format: yaml
  label: Navigate Vendors API
  slug: navigate-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-vendors-api-openapi.yml
- filename: navigate-video-upload-requests-api-openapi.yml
  format: yaml
  label: Navigate Video Upload Requests API
  slug: navigate-video-upload-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-video-upload-requests-api-openapi.yml
- filename: navigate-visit-types-api-openapi.yml
  format: yaml
  label: Navigate Visit types API
  slug: navigate-visit-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-visit-types-api-openapi.yml
- filename: navigate-visits-api-openapi.yml
  format: yaml
  label: Navigate Visits API
  slug: navigate-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-visits-api-openapi.yml
- filename: navigate-work-orders-api-openapi.yml
  format: yaml
  label: Navigate Work orders API
  slug: navigate-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/openapi/navigate-work-orders-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Navigate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Navigate declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Navigate
provider_slug: navigate
scheme_count: 1
schemes:
- description: HTTP bearer authentication. Present a NavigateAI API key as the bearer token. Applied globally as the security requirement on every documented operation.
  format: 'Authorization: Bearer <api_key>'
  header: Authorization
  in: header
  name: ApiKeyAuth
  scheme: bearer
  type: http
slug: navigate-authentication
source_filename: navigate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: derived from openapi/navigate-openapi.json components.securitySchemes\napi: NavigateAI API\nsummary: >-\n  The NavigateAI external API authenticates every operation with a bearer token\n  (API key) supplied in the Authorization header. All 51 operations declare the\n  ApiKeyAuth requirement; there are no unauthenticated endpoints and no OAuth2,\n  OpenID Connect, or mutual-TLS schemes in the published specification.\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <api_key>'\n  description: >-\n    HTTP bearer authentication. Present a NavigateAI API key as the bearer token.\n    Applied globally as the security requirement on every documented operation.\ncoverage:\n  total_operations: 51\n  secured_operations: 51\n  unsecured_operations: 0\nnotes:\n- The specification does not document a scopes/permissions model on the bearer scheme,\n  so\
  \ no OAuthScopes artifact is derived (single API-key credential).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navigate/refs/heads/main/authentication/navigate-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Proptech
- Construction
- Real Estate
- Artificial Intelligence
- Field Service
- Construction Technology
- API
---
