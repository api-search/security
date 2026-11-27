---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usetrackly-app-companies-api-openapi.yml
  format: yaml
  label: Trackly Companies API
  slug: usetrackly-app-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-companies-api-openapi.yml
- filename: usetrackly-app-jobs-api-openapi.yml
  format: yaml
  label: Trackly Jobs API
  slug: usetrackly-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-jobs-api-openapi.yml
- filename: usetrackly-app-user-api-openapi.yml
  format: yaml
  label: Trackly User API
  slug: usetrackly-app-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetrackly-app/openapi/usetrackly-app-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Trackly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trackly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trackly
provider_slug: usetrackly-app
scheme_count: 1
schemes:
- bearerFormat: trk_
  description: 'Trackly API key, issued at [usetrackly.app/developers](https://usetrackly.app/developers). Keys start with the `trk_` prefix. Pass as `Authorization: Bearer trk_...`.'
  name: TracklyAPIKey
  scheme: bearer
  sources:
  - openapi/usetrackly-app-openapi.json
  type: http
slug: usetrackly-app-authentication
source_filename: usetrackly-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: derived\nsource: openapi/usetrackly-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: TracklyAPIKey\n  type: http\n  scheme: bearer\n  bearerFormat: trk_\n  description: 'Trackly API key, issued at [usetrackly.app/developers](https://usetrackly.app/developers).\n    Keys start with the `trk_` prefix. Pass as `Authorization: Bearer trk_...`.'\n  sources:\n  - openapi/usetrackly-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/usetrackly-app/authentication/usetrackly-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Job Search
- Student Recruiting
- AI Agent
- Career Page Monitoring
---
