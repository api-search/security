---
api_key_in:
- header
api_specs:
- filename: swaggerhub-apis-api-openapi.yml
  format: yaml
  label: SwaggerHub APIs API
  slug: swaggerhub-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-apis-api-openapi.yml
- filename: swaggerhub-domains-api-openapi.yml
  format: yaml
  label: SwaggerHub Domains API
  slug: swaggerhub-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-domains-api-openapi.yml
- filename: swaggerhub-integrations-api-openapi.yml
  format: yaml
  label: SwaggerHub Integrations API
  slug: swaggerhub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-integrations-api-openapi.yml
- filename: swaggerhub-organizations-api-openapi.yml
  format: yaml
  label: SwaggerHub Organizations API
  slug: swaggerhub-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-organizations-api-openapi.yml
- filename: swaggerhub-projects-api-openapi.yml
  format: yaml
  label: SwaggerHub Projects API
  slug: swaggerhub-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-projects-api-openapi.yml
- filename: swaggerhub-search-api-openapi.yml
  format: yaml
  label: SwaggerHub Search API
  slug: swaggerhub-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-search-api-openapi.yml
- filename: swaggerhub-settings-api-openapi.yml
  format: yaml
  label: SwaggerHub Settings API
  slug: swaggerhub-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-settings-api-openapi.yml
- filename: swaggerhub-standardization-api-openapi.yml
  format: yaml
  label: SwaggerHub Standardization API
  slug: swaggerhub-standardization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-standardization-api-openapi.yml
- filename: swaggerhub-teams-api-openapi.yml
  format: yaml
  label: SwaggerHub Teams API
  slug: swaggerhub-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-teams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swaggerhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: SwaggerHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SwaggerHub
provider_slug: swaggerhub
scheme_count: 1
schemes:
- description: SwaggerHub API key. Obtain from My Account > API Key in SwaggerHub. Pass the key as the Authorization header value without any prefix.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/swaggerhub-registry-api-openapi.yml
  - openapi/swaggerhub-user-management-openapi.yml
  type: apiKey
slug: swaggerhub-authentication
source_filename: swaggerhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swaggerhub-registry-api-openapi.yml, openapi/swaggerhub-user-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: SwaggerHub API key. Obtain from My Account > API Key in SwaggerHub. Pass the\n    key as the Authorization header value without any prefix.\n  sources:\n  - openapi/swaggerhub-registry-api-openapi.yml\n  - openapi/swaggerhub-user-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/authentication/swaggerhub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Design
- API Management
- API Registry
- Documentation
- OpenAPI
- SmartBear
---
