---
api_key_in: []
api_specs:
- filename: predicthq-events-api-openapi.yml
  format: yaml
  label: PredictHQ Events API
  slug: predicthq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/openapi/predicthq-events-api-openapi.yml
- filename: predicthq-features-api-openapi.yml
  format: yaml
  label: PredictHQ Features API
  slug: predicthq-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/openapi/predicthq-features-api-openapi.yml
- filename: predicthq-places-api-openapi.yml
  format: yaml
  label: PredictHQ Places API
  slug: predicthq-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/openapi/predicthq-places-api-openapi.yml
- filename: predicthq-suggested-radius-api-openapi.yml
  format: yaml
  label: PredictHQ Suggested Radius API
  slug: predicthq-suggested-radius-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/openapi/predicthq-suggested-radius-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Predicthq Authentication
name_suffix: Authentication
oauth_flows: []
overview: PredictHQ secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PredictHQ
provider_slug: predicthq
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/predicthq-openapi.yml
  type: http
slug: predicthq-authentication
source_filename: predicthq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/predicthq-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/predicthq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predicthq/refs/heads/main/authentication/predicthq-authentication.yml
summary_line: http · 1 scheme
tags:
- Demand Intelligence
- Event
- Forecasting
- Machine-Learning
- Real-World Events
---
