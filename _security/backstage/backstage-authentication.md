---
api_key_in:
- cookie
api_specs:
- filename: backstage-events-asyncapi.yml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/asyncapi/backstage-events-asyncapi.yml
- filename: backstage-actions-api-openapi.yml
  format: yaml
  label: Backstage Actions API
  slug: backstage-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-actions-api-openapi.yml
- filename: backstage-authentication-api-openapi.yml
  format: yaml
  label: Backstage Authentication API
  slug: backstage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authentication-api-openapi.yml
- filename: backstage-authorization-api-openapi.yml
  format: yaml
  label: Backstage Authorization API
  slug: backstage-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authorization-api-openapi.yml
- filename: backstage-documentation-api-openapi.yml
  format: yaml
  label: Backstage Documentation API
  slug: backstage-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-documentation-api-openapi.yml
- filename: backstage-entities-api-openapi.yml
  format: yaml
  label: Backstage Entities API
  slug: backstage-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-entities-api-openapi.yml
- filename: backstage-locations-api-openapi.yml
  format: yaml
  label: Backstage Locations API
  slug: backstage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-locations-api-openapi.yml
- filename: backstage-metadata-api-openapi.yml
  format: yaml
  label: Backstage Metadata API
  slug: backstage-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-metadata-api-openapi.yml
- filename: backstage-search-api-openapi.yml
  format: yaml
  label: Backstage Search API
  slug: backstage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-api-openapi.yml
- filename: backstage-sync-api-openapi.yml
  format: yaml
  label: Backstage Sync API
  slug: backstage-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-sync-api-openapi.yml
- filename: backstage-tasks-api-openapi.yml
  format: yaml
  label: Backstage Tasks API
  slug: backstage-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-tasks-api-openapi.yml
- filename: backstage-templates-api-openapi.yml
  format: yaml
  label: Backstage Templates API
  slug: backstage-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-templates-api-openapi.yml
- filename: backstage-token-verification-api-openapi.yml
  format: yaml
  label: Backstage Token Verification API
  slug: backstage-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-token-verification-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Backstage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backstage secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Backstage
provider_slug: backstage
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: backstage-auth
  sources:
  - openapi/backstage-auth-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/backstage-auth-openapi.yml
  - openapi/backstage-catalog-openapi.yml
  - openapi/backstage-permissions-openapi.yml
  - openapi/backstage-scaffolder-openapi.yml
  - openapi/backstage-search-openapi.yml
  - openapi/backstage-techdocs-openapi.yml
  type: http
slug: backstage-authentication
source_filename: backstage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/backstage-auth-openapi.yml, openapi/backstage-catalog-openapi.yml, openapi/backstage-permissions-openapi.yml,\n  openapi/backstage-scaffolder-openapi.yml, openapi/backstage-search-openapi.yml, openapi/backstage-techdocs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: backstage-auth\n  sources:\n  - openapi/backstage-auth-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/backstage-auth-openapi.yml\n  - openapi/backstage-catalog-openapi.yml\n  - openapi/backstage-permissions-openapi.yml\n  - openapi/backstage-scaffolder-openapi.yml\n  - openapi/backstage-search-openapi.yml\n  - openapi/backstage-techdocs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/authentication/backstage-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
---
