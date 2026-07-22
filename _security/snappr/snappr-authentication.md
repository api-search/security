---
api_key_in:
- header
api_specs:
- filename: snappr-openapi.yml
  format: yaml
  label: Snappr API
  slug: snappr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Snappr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snappr secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snappr
provider_slug: snappr
scheme_count: 1
schemes:
- description: API key as a bearer token. The API is available only to Snappr for Enterprise customers.
  format: 'Authorization: Bearer <api_key>'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snappr-openapi.yml
  - https://docs.snappr.com/
  type: http
slug: snappr-authentication
source_filename: snappr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.snappr.com/\ndocs: https://docs.snappr.com/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  notes: >-\n    Snappr uses API keys presented as a bearer token in the Authorization\n    header. Each user has a single unique active API key, managed and\n    regenerated from the Photography Portal GUI. Regenerating deactivates the\n    previous key; deleting a user deactivates their key.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <api_key>'\n    description: >-\n      API key as a bearer token. The API is available only to Snappr for\n      Enterprise customers.\n    sources: [openapi/snappr-openapi.yml, https://docs.snappr.com/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/authentication/snappr-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Marketplace
- Photography
- Videography
- Visual Content
- Photo Editing
- On-Demand
- Enterprise
---
