---
api_key_in: []
api_specs:
- filename: torii-apps-api-openapi.yml
  format: yaml
  label: Torii Apps API
  slug: torii-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-apps-api-openapi.yml
- filename: torii-audit-api-openapi.yml
  format: yaml
  label: Torii Audit API
  slug: torii-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-audit-api-openapi.yml
- filename: torii-contracts-api-openapi.yml
  format: yaml
  label: Torii Contracts API
  slug: torii-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-contracts-api-openapi.yml
- filename: torii-files-api-openapi.yml
  format: yaml
  label: Torii Files API
  slug: torii-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-files-api-openapi.yml
- filename: torii-metadata-api-openapi.yml
  format: yaml
  label: Torii Metadata API
  slug: torii-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-metadata-api-openapi.yml
- filename: torii-parsings-api-openapi.yml
  format: yaml
  label: Torii Parsings API
  slug: torii-parsings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-parsings-api-openapi.yml
- filename: torii-scim-api-openapi.yml
  format: yaml
  label: Torii SCIM API
  slug: torii-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-scim-api-openapi.yml
- filename: torii-services-api-openapi.yml
  format: yaml
  label: Torii Services API
  slug: torii-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-services-api-openapi.yml
- filename: torii-users-api-openapi.yml
  format: yaml
  label: Torii Users API
  slug: torii-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-users-api-openapi.yml
- filename: torii-workflows-api-openapi.yml
  format: yaml
  label: Torii Workflows API
  slug: torii-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Torii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Torii secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Torii
provider_slug: torii
scheme_count: 1
schemes:
- description: 'API key authentication. Generate an API key from Settings > API Access in Torii. Use the Authorization header: Bearer {API_KEY}.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/torii-torii-openapi.yml
  type: http
slug: torii-authentication
source_filename: torii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/torii-torii-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key authentication. Generate an API key from Settings > API Access in Torii.\n    Use the Authorization header: Bearer {API_KEY}.'\n  sources:\n  - openapi/torii-torii-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/authentication/torii-authentication.yml
summary_line: http · 1 scheme
tags:
- Application
- Compliance
- Cost Optimization
- Governance
- IT Management
- SaaS Management
---
