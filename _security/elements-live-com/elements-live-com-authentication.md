---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elements-live-com-elements-api-openapi.yml
  format: yaml
  label: Elements Live Elements API
  slug: elements-live-com-elements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elements-live-com/openapi/elements-live-com-elements-api-openapi.yml
- filename: elements-live-com-lab-api-openapi.yml
  format: yaml
  label: Elements Live Lab API
  slug: elements-live-com-lab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elements-live-com/openapi/elements-live-com-lab-api-openapi.yml
- filename: elements-live-com-research-api-openapi.yml
  format: yaml
  label: Elements Live Research API
  slug: elements-live-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elements-live-com/openapi/elements-live-com-research-api-openapi.yml
- filename: elements-live-com-subjects-api-openapi.yml
  format: yaml
  label: Elements Live Subjects API
  slug: elements-live-com-subjects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elements-live-com/openapi/elements-live-com-subjects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Elements Live Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elements Live secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Elements Live
provider_slug: elements-live-com
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/elements-live-com-openapi.json
  type: http
slug: elements-live-com-authentication
source_filename: elements-live-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/elements-live-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/elements-live-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/elements-live-com/authentication/elements-live-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Research
- Science
- Metrics
- Dashboards
- Data
---
