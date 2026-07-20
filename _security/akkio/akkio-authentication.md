---
api_key_in:
- query
- body
api_specs:
- filename: akkio-api-openapi.yml
  format: yaml
  label: Akkio API
  slug: akkio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/openapi/akkio-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Akkio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Akkio secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Akkio
provider_slug: akkio
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/akkio-api-openapi.yml
  type: apiKey
- in: body
  name: apiKeyBody
  parameter: api_key
  sources:
  - github.com/akkio-inc/akkio-python
  type: apiKey
slug: akkio-authentication
source_filename: akkio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://github.com/akkio-inc/akkio-python\ndocs: https://app.akk.io/team-settings\nsummary:\n  types: [apiKey]\n  api_key_in: [query, body]\n  oauth2_flows: []\n  notes: >-\n    Akkio authenticates every request with a single API key. On GET requests the\n    key is sent as the `api_key` query parameter; on POST/DELETE requests it is\n    sent as the `api_key` field inside the JSON request body. Keys are issued\n    and rotated from the account Team Settings page. There is no OAuth surface,\n    so no scopes/ artifact is produced.\nschemes:\n  - name: apiKeyQuery\n    type: apiKey\n    in: query\n    parameter: api_key\n    sources: [openapi/akkio-api-openapi.yml]\n  - name: apiKeyBody\n    type: apiKey\n    in: body\n    parameter: api_key\n    sources: [github.com/akkio-inc/akkio-python]\nkey_management:\n  issue_url: https://app.akk.io/team-settings\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akkio/refs/heads/main/authentication/akkio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Apps
- Machine Learning
- Predictive Analytics
- No Code
- Data Science
- Marketing
- Media
- Audience Modeling
- Predictions
---
