---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: famxplor-family-travel-api-openapi.yml
  format: yaml
  label: Famxplor Family Travel API
  slug: famxplor-family-travel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/famxplor-family-travel-api/refs/heads/main/openapi/famxplor-family-travel-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Famxplor Family Travel Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Famxplor Family Travel API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Famxplor Family Travel API
provider_slug: famxplor-family-travel-api
scheme_count: 1
schemes:
- applies_to_operations:
  - nearest_posts_v1_nearest_posts_post
  - nearest_activities_v1_nearest_activities_post
  - travel_time_v1_travel_time_post
  - activity_details_v1_activities_details__activity_id__get
  in: header
  name: APIKeyHeader
  parameter: api-key
  sources:
  - openapi/famxplor-family-travel-api-openapi.yml
  type: apiKey
slug: famxplor-family-travel-api-authentication
source_filename: famxplor-family-travel-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://api.famxplor.com/openapi.json\ndocs: https://api.famxplor.com/redoc\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows: []\n  model: >-\n    Single static API key passed in the `api-key` request header. Every one of the\n    four published operations declares `security: [{APIKeyHeader: []}]`, so the whole\n    surface is key-protected; there is no anonymous tier, no OAuth, and no per-scope\n    authorization. Keys are self-service after signup and are bound to a paid plan.\nschemes:\n  - name: APIKeyHeader\n    type: apiKey\n    in: header\n    parameter: api-key\n    sources:\n      - openapi/famxplor-family-travel-api-openapi.yml\n    applies_to_operations:\n      - nearest_posts_v1_nearest_posts_post\n      - nearest_activities_v1_nearest_activities_post\n      - travel_time_v1_travel_time_post\n      - activity_details_v1_activities_details__activity_id__get\nkey_acquisition:\n  url:\
  \ https://famxplor.com/api\n  note: >-\n    \"Get your API key today\" — the key is issued on signup at https://famxplor.com/login\n    and requires an active plan (14-day free trial, no card).\nexample_request: |\n  curl -X POST \"https://api.famxplor.com/v1/nearest-activities\" \\\n    -H 'Content-Type: application/json' \\\n    -H \"api-key: $API_KEY\" \\\n    -d '{\"lat\":48.85341,\"lon\":2.3488,\"max_distance\":100000}'\nobserved_failure:\n  probed: '2026-09-07'\n  request: POST https://api.famxplor.com/v1/nearest-activities (no api-key header)\n  status: 403\n  body: '{\"detail\":\"An API key must be passed as header\"}'\n  note: >-\n    403 rather than 401, and no WWW-Authenticate challenge header is returned — an\n    agent has to read the body to learn what is missing.\nrotation: not documented\nscopes: none — the key carries no scope or permission model\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/famxplor-family-travel-api/refs/heads/main/authentication/famxplor-family-travel-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Activities
- Family
- Travel
- Artificial Intelligence
- MCP
---
