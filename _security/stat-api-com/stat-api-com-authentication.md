---
anonymous_access: false
api_key_in: []
api_specs:
- filename: stat-api-com-dfs-api-openapi.yml
  format: yaml
  label: stat-api-com DFS API
  slug: stat-api-com-dfs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-dfs-api-openapi.yml
- filename: stat-api-com-mlb-api-openapi.yml
  format: yaml
  label: stat-api-com MLB API
  slug: stat-api-com-mlb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-mlb-api-openapi.yml
- filename: stat-api-com-nba-api-openapi.yml
  format: yaml
  label: stat-api-com NBA API
  slug: stat-api-com-nba-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-nba-api-openapi.yml
- filename: stat-api-com-nfl-api-openapi.yml
  format: yaml
  label: stat-api-com NFL API
  slug: stat-api-com-nfl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-nfl-api-openapi.yml
- filename: stat-api-com-nhl-api-openapi.yml
  format: yaml
  label: stat-api-com NHL API
  slug: stat-api-com-nhl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-nhl-api-openapi.yml
- filename: stat-api-com-pga-api-openapi.yml
  format: yaml
  label: stat-api-com PGA API
  slug: stat-api-com-pga-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-pga-api-openapi.yml
- filename: stat-api-com-reference-api-openapi.yml
  format: yaml
  label: stat-api-com Reference API
  slug: stat-api-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stat-api-com/openapi/stat-api-com-reference-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Stat Api Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: stat-api-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: stat-api-com
provider_slug: stat-api-com
scheme_count: 1
schemes:
- bearerFormat: API key
  description: 'Pass your API key as an Authorization header: `Authorization: Bearer YOUR_API_KEY` (the `ApiKey` scheme is accepted as an alias). The docs UI exposes a global API key field that substitutes into every code sample and live request. Unauthenticated requests to /api/v1 are rejected with 401 — every call needs a key (the shared trial key works only against each endpoint''s documented default URL).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stat-api-com-openapi.json
  type: http
slug: stat-api-com-authentication
source_filename: stat-api-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource:\n  - openapi/stat-api-com-openapi.json\n  - https://stat-api.com/faq/\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  description: 'Pass your API key as an Authorization header: `Authorization: Bearer YOUR_API_KEY`\n    (the `ApiKey` scheme is accepted as an alias). The docs UI exposes a global API key field\n    that substitutes into every code sample and live request. Unauthenticated requests to /api/v1\n    are rejected with 401 — every call needs a key (the shared trial key works only against\n    each endpoint''s documented default URL).'\n  sources:\n  - openapi/stat-api-com-openapi.json\n\ndocs: https://stat-api.com/faq/\n"
source_yaml_url: https://artifacts.apis.io/stat-api-com/authentication/stat-api-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Sports
- Data
- API
- DFS
- Fantasy
---
