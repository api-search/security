---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trendsfast-next-move-api-openapi.yml
  format: yaml
  label: TrendsFast Next Move API
  slug: trendsfast-next-move-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trendsfast/openapi/trendsfast-next-move-api-openapi.yml
- filename: trendsfast-next-moves-api-openapi.yml
  format: yaml
  label: TrendsFast Next Moves API
  slug: trendsfast-next-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trendsfast/openapi/trendsfast-next-moves-api-openapi.yml
- filename: trendsfast-projects-api-openapi.yml
  format: yaml
  label: TrendsFast Projects API
  slug: trendsfast-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trendsfast/openapi/trendsfast-projects-api-openapi.yml
- filename: trendsfast-public-api-openapi.yml
  format: yaml
  label: TrendsFast Public API
  slug: trendsfast-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trendsfast/openapi/trendsfast-public-api-openapi.yml
- filename: trendsfast-trends-api-openapi.yml
  format: yaml
  label: TrendsFast Trends API
  slug: trendsfast-trends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trendsfast/openapi/trendsfast-trends-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Trendsfast Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrendsFast declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TrendsFast
provider_slug: trendsfast
scheme_count: 1
schemes:
- bearerFormat: TrendsFast API key
  description: API key passed as Bearer token in Authorization header.
  docs: https://trendsfast.com/docs#auth
  expiration_days: 90
  name: bearerApiKey
  scheme: bearer
  scopes:
  - trends:query
  - trends:read
  - credits:read
  type: http
slug: trendsfast-authentication
source_filename: trendsfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/trendsfast-v1-openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: TrendsFast API key\n    description: API key passed as Bearer token in Authorization header.\n    name: bearerApiKey\n    scopes:\n      - trends:query\n      - trends:read\n      - credits:read\n    expiration_days: 90\n    docs: https://trendsfast.com/docs#auth\n"
source_yaml_url: https://artifacts.apis.io/trendsfast/authentication/trendsfast-authentication.yml
summary_line: 1 scheme
tags:
- API
- Trends
- SocialMedia
- Search
- AI
---
