---
api_key_in:
- header
api_specs:
- filename: snappr-availability-api-openapi.yml
  format: yaml
  label: Snappr Availability API
  slug: snappr-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-availability-api-openapi.yml
- filename: snappr-bookings-api-openapi.yml
  format: yaml
  label: Snappr Bookings API
  slug: snappr-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-bookings-api-openapi.yml
- filename: snappr-coverage-api-openapi.yml
  format: yaml
  label: Snappr Coverage API
  slug: snappr-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-coverage-api-openapi.yml
- filename: snappr-editing-job-types-api-openapi.yml
  format: yaml
  label: Snappr Editing Job Types API
  slug: snappr-editing-job-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-editing-job-types-api-openapi.yml
- filename: snappr-editing-jobs-api-openapi.yml
  format: yaml
  label: Snappr Editing Jobs API
  slug: snappr-editing-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-editing-jobs-api-openapi.yml
- filename: snappr-images-api-openapi.yml
  format: yaml
  label: Snappr Images API
  slug: snappr-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-images-api-openapi.yml
- filename: snappr-presets-api-openapi.yml
  format: yaml
  label: Snappr Presets API
  slug: snappr-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-presets-api-openapi.yml
- filename: snappr-shoot-types-api-openapi.yml
  format: yaml
  label: Snappr Shoot Types API
  slug: snappr-shoot-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-shoot-types-api-openapi.yml
- filename: snappr-videos-api-openapi.yml
  format: yaml
  label: Snappr Videos API
  slug: snappr-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snappr/refs/heads/main/openapi/snappr-videos-api-openapi.yml
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
