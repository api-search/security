---
api_key_in: []
api_specs:
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Objects API
  slug: warrant-dev-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Relationships (Warrants) API
  slug: warrant-dev-warrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Check (Authorization) API
  slug: warrant-dev-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Object Types API
  slug: warrant-dev-object-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Roles & Permissions API
  slug: warrant-dev-roles-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Warrant Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Warrant secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Warrant
provider_slug: warrant-dev
scheme_count: 1
schemes:
- description: 'Warrant authenticated API requests with an API key passed in the Authorization header as `Authorization: ApiKey YOUR_API_KEY`. Hosted keys were issued from the Warrant dashboard; self-hosted deployments set the key via the `ApiKey` value in the server configuration. Frontend/self-service flows used short-lived session tokens minted from the API key server-side. RETIRED - the hosted service was sunset 2025-11-15; the same header scheme applies to the open-source self-hosted server.'
  headerName: Authorization
  in: header
  name: apiKeyAuth
  sources:
  - openapi/warrant-dev-openapi.yml
  - https://github.com/warrant-dev/warrant
  type: apiKey
slug: warrant-dev-authentication
source_filename: warrant-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warrant-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  headerName: Authorization\n  description: >-\n    Warrant authenticated API requests with an API key passed in the\n    Authorization header as `Authorization: ApiKey YOUR_API_KEY`. Hosted keys\n    were issued from the Warrant dashboard; self-hosted deployments set the key\n    via the `ApiKey` value in the server configuration. Frontend/self-service\n    flows used short-lived session tokens minted from the API key server-side.\n    RETIRED - the hosted service was sunset 2025-11-15; the same header scheme\n    applies to the open-source self-hosted server.\n  sources:\n  - openapi/warrant-dev-openapi.yml\n  - https://github.com/warrant-dev/warrant\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/authentication/warrant-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Access Control
- Authorization
- Fine-Grained Authorization
- FGA
- RBAC
- ReBAC
- ABAC
- Zanzibar
- Permissions
- Open Source
- Retired
---
