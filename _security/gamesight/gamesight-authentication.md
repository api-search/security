---
api_key_in:
- header
api_specs:
- filename: gamesight-measurement-openapi.json
  format: json
  label: Gamesight Measurement API
  slug: gamesight-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-measurement-openapi.json
- filename: gamesight-reporting-openapi.json
  format: json
  label: Gamesight Reporting API
  slug: gamesight-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/openapi/gamesight-reporting-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gamesight Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gamesight secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gamesight
provider_slug: gamesight
scheme_count: 1
schemes:
- description: A valid Gamesight API key passed in the Authorization header. Reporting API keys carry Reporting, Aggregate Reporting, or GDPR scope.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/gamesight-measurement-openapi.json
  - openapi/gamesight-reporting-openapi.json
  type: apiKey
slug: gamesight-authentication
source_filename: gamesight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gamesight-measurement-openapi.json, openapi/gamesight-reporting-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: A valid Gamesight API key passed in the Authorization header. Reporting API keys\n    carry Reporting, Aggregate Reporting, or GDPR scope.\n  sources:\n  - openapi/gamesight-measurement-openapi.json\n  - openapi/gamesight-reporting-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamesight/refs/heads/main/authentication/gamesight-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Gaming
- Marketing
- Analytics
- Attribution
- Measurement
- Advertising
- Creators
- Game Development
---
