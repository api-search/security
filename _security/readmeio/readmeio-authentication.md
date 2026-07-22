---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Readmeio Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReadMe.io secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReadMe.io
provider_slug: readmeio
scheme_count: 2
schemes:
- applies_to: ReadMe API (v2), Developer Metrics API
  base_url: https://api.readme.com/v2
  example: 'curl https://api.readme.com/v2/projects/me -X GET --header "Authorization: Bearer README_API_KEY"'
  header: 'Authorization: Bearer README_API_KEY'
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.readme.com/main/reference/authentication
  type: http
- applies_to: ReadMe API (v1, Legacy)
  base_url: https://dash.readme.com/api/v1
  name: BasicAuth
  note: API key supplied via HTTP Basic auth. Not available to projects using ReadMe Refactored; superseded by the v2 Bearer scheme.
  scheme: basic
  sources:
  - https://docs.readme.com/main/reference/legacy-api
  type: http
slug: readmeio-authentication
source_filename: readmeio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.readme.com/main/reference/authentication\ndocs: https://docs.readme.com/main/reference/authentication\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    ReadMe uses project API keys. v2 passes the key as an HTTP Bearer token; the\n    legacy v1 API uses HTTP Basic auth with the API key as the username.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applies_to: ReadMe API (v2), Developer Metrics API\n  base_url: https://api.readme.com/v2\n  header: 'Authorization: Bearer README_API_KEY'\n  example: >-\n    curl https://api.readme.com/v2/projects/me -X GET\n    --header \"Authorization: Bearer README_API_KEY\"\n  sources:\n  - https://docs.readme.com/main/reference/authentication\n- name: BasicAuth\n  type: http\n  scheme: basic\n  applies_to: ReadMe API (v1, Legacy)\n  base_url: https://dash.readme.com/api/v1\n  note: >-\n    API key supplied via HTTP\
  \ Basic auth. Not available to projects using ReadMe\n    Refactored; superseded by the v2 Bearer scheme.\n  sources:\n  - https://docs.readme.com/main/reference/legacy-api\nkey_management:\n  where: ReadMe dashboard — Configuration > API Keys\n  programmatic:\n  - createApiKey\n  - getApiKeys\n  - getApiKey\n  - updateApiKey\n  - deleteApiKey\n  rotation: API keys can be rotated from the dashboard.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readmeio/refs/heads/main/authentication/readmeio-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Apis
- Documentation
- API Documentation
- Developer Experience
- Developer Portal
- OpenAPI
- Developer Hub
- API Metrics
---
