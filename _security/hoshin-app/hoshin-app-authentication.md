---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hoshin-app-analysis-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Analysis API
  slug: hoshin-app-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-analysis-api-openapi.yml
- filename: hoshin-app-cadences-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Cadences API
  slug: hoshin-app-cadences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-cadences-api-openapi.yml
- filename: hoshin-app-elements-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Elements API
  slug: hoshin-app-elements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-elements-api-openapi.yml
- filename: hoshin-app-exports-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Exports API
  slug: hoshin-app-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-exports-api-openapi.yml
- filename: hoshin-app-ideas-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Ideas API
  slug: hoshin-app-ideas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-ideas-api-openapi.yml
- filename: hoshin-app-identity-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Identity API
  slug: hoshin-app-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-identity-api-openapi.yml
- filename: hoshin-app-matrices-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Matrices API
  slug: hoshin-app-matrices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-matrices-api-openapi.yml
- filename: hoshin-app-sharing-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Sharing API
  slug: hoshin-app-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-sharing-api-openapi.yml
- filename: hoshin-app-themes-api-openapi.yml
  format: yaml
  label: Hoshin Kanri Themes API
  slug: hoshin-app-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoshin-app/openapi/hoshin-app-themes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hoshin Kanri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hoshin Kanri secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hoshin Kanri
provider_slug: hoshin-app
scheme_count: 1
schemes:
- description: 'An API token, hk_..., or an OAuth 2.1 access token. OAuth needs PKCE S256 and a registered client: https://hoshin.app/.well-known/oauth-authorization-server'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hoshin-app-openapi.json
  type: http
slug: hoshin-app-authentication
source_filename: hoshin-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hoshin-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API token, hk_..., or an OAuth 2.1 access token. OAuth needs PKCE S256 and\n    a registered client: https://hoshin.app/.well-known/oauth-authorization-server'\n  sources:\n  - openapi/hoshin-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hoshin-app/authentication/hoshin-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Software
- Manufacturing
- Artificial Intelligence
- Strategy
- HoshinKanri
---
