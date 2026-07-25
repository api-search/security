---
api_key_in: []
api_specs:
- filename: neon-auth-webhooks-asyncapi.yml
  format: yaml
  label: Neon Auth
  slug: auth
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/asyncapi/neon-auth-webhooks-asyncapi.yml
- filename: neon-api-keys-api-openapi.yml
  format: yaml
  label: Neon API Keys API
  slug: neon-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-api-keys-api-openapi.yml
- filename: neon-auth-api-openapi.yml
  format: yaml
  label: Neon Auth API
  slug: neon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-auth-api-openapi.yml
- filename: neon-branches-api-openapi.yml
  format: yaml
  label: Neon Branches API
  slug: neon-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-branches-api-openapi.yml
- filename: neon-consumption-api-openapi.yml
  format: yaml
  label: Neon Consumption API
  slug: neon-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-consumption-api-openapi.yml
- filename: neon-data-api-api-openapi.yml
  format: yaml
  label: Neon Data API API
  slug: neon-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-data-api-api-openapi.yml
- filename: neon-databases-api-openapi.yml
  format: yaml
  label: Neon Databases API
  slug: neon-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-databases-api-openapi.yml
- filename: neon-endpoints-api-openapi.yml
  format: yaml
  label: Neon Endpoints API
  slug: neon-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-endpoints-api-openapi.yml
- filename: neon-operations-api-openapi.yml
  format: yaml
  label: Neon Operations API
  slug: neon-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-operations-api-openapi.yml
- filename: neon-projects-api-openapi.yml
  format: yaml
  label: Neon Projects API
  slug: neon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-projects-api-openapi.yml
- filename: neon-roles-api-openapi.yml
  format: yaml
  label: Neon Roles API
  slug: neon-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-roles-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Neon
provider_slug: neon
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Neon API keys are used to authenticate requests. Include the API key in the Authorization header as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/neon-management-api-openapi.yml
  type: http
slug: neon-authentication
source_filename: neon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neon-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Neon API keys are used to authenticate requests. Include the API key in the Authorization\n    header as a Bearer token.\n  sources:\n  - openapi/neon-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/authentication/neon-authentication.yml
summary_line: http · 1 scheme
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
---
