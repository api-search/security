---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: hackforddata-com-complaints-api-openapi.yml
  format: yaml
  label: Hackford Complaints API
  slug: hackforddata-com-complaints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-complaints-api-openapi.yml
- filename: hackforddata-com-enforcement-api-openapi.yml
  format: yaml
  label: Hackford Enforcement API
  slug: hackforddata-com-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-enforcement-api-openapi.yml
- filename: hackforddata-com-exports-api-openapi.yml
  format: yaml
  label: Hackford Exports API
  slug: hackforddata-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-exports-api-openapi.yml
- filename: hackforddata-com-firm-types-api-openapi.yml
  format: yaml
  label: Hackford Firm types API
  slug: hackforddata-com-firm-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-firm-types-api-openapi.yml
- filename: hackforddata-com-firms-api-openapi.yml
  format: yaml
  label: Hackford Firms API
  slug: hackforddata-com-firms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-firms-api-openapi.yml
- filename: hackforddata-com-people-api-openapi.yml
  format: yaml
  label: Hackford People API
  slug: hackforddata-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-people-api-openapi.yml
- filename: hackforddata-com-public-api-api-openapi.yml
  format: yaml
  label: Hackford Public API
  slug: hackforddata-com-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-public-api-api-openapi.yml
- filename: hackforddata-com-relationships-api-openapi.yml
  format: yaml
  label: Hackford Relationships API
  slug: hackforddata-com-relationships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-relationships-api-openapi.yml
- filename: hackforddata-com-saved-searches-api-openapi.yml
  format: yaml
  label: Hackford Saved searches API
  slug: hackforddata-com-saved-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-saved-searches-api-openapi.yml
- filename: hackforddata-com-watchlists-api-openapi.yml
  format: yaml
  label: Hackford Watchlists API
  slug: hackforddata-com-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackforddata-com/openapi/hackforddata-com-watchlists-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Hackford Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hackford secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hackford
provider_slug: hackforddata-com
scheme_count: 3
schemes:
- bearerFormat: OAuth 2.1 access token
  name: OAuthAccessTokenAuth
  scheme: bearer
  sources:
  - openapi/hackforddata-com-openapi.yml
  type: http
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/hackforddata-com-openapi.yml
  type: apiKey
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/hackforddata-com-openapi.yml
  type: apiKey
slug: hackforddata-com-authentication
source_filename: hackforddata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hackforddata-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: OAuthAccessTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth 2.1 access token\n  sources:\n  - openapi/hackforddata-com-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/hackforddata-com-openapi.yml\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/hackforddata-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/hackforddata-com/authentication/hackforddata-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Data
- Intelligence
- Financial Services
- Regulatory
- B2B
- Compliance
---
