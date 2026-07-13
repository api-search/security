---
api_key_in:
- cookie
api_specs:
- filename: backstage-catalog-openapi.yml
  format: yaml
  label: Backstage Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-catalog-openapi.yml
- filename: backstage-scaffolder-openapi.yml
  format: yaml
  label: Backstage Scaffolder API
  slug: scaffolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-scaffolder-openapi.yml
- filename: backstage-auth-openapi.yml
  format: yaml
  label: Backstage Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-auth-openapi.yml
- filename: backstage-techdocs-openapi.yml
  format: yaml
  label: Backstage TechDocs API
  slug: techdocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-techdocs-openapi.yml
- filename: backstage-search-openapi.yml
  format: yaml
  label: Backstage Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-openapi.yml
- filename: backstage-permissions-openapi.yml
  format: yaml
  label: Backstage Permissions API
  slug: permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-permissions-openapi.yml
- filename: backstage-events-asyncapi.yml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/asyncapi/backstage-events-asyncapi.yml
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
