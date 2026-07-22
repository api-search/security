---
api_key_in: []
api_specs:
- filename: revyze-openapi.json
  format: json
  label: Revyze API
  slug: revyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/openapi/revyze-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Revyze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revyze declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Revyze
provider_slug: revyze
scheme_count: 0
schemes: []
slug: revyze-authentication
source_filename: revyze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/revyze-openapi.json\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The published OpenAPI (FastAPI, title \"FastAPI\", version 0.1.0) declares NO\n    components.securitySchemes and applies no security requirements to any\n    operation. This is the mobile app's own backend rather than a documented\n    developer API, so no public authentication model is published. Observed\n    endpoints imply app-internal auth that is not described in the spec: an\n    /admin/api/token endpoint and /admin/graphql suggest an admin token flow, and\n    the primary /graphql3 endpoint is consumed by the first-party mobile client.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revyze/refs/heads/main/authentication/revyze-authentication.yml
summary_line: 0 schemes
tags:
- Company
- EdTech
- Education
- Mobile
- Video
- Learning
- Quiz
- France
- GraphQL
---
