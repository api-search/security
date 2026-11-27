---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entire-vc-check-store-api-openapi.yml
  format: yaml
  label: Entire VC Check Store API
  slug: entire-vc-check-store-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entire-vc/openapi/entire-vc-check-store-api-openapi.yml
- filename: entire-vc-d-api-openapi.yml
  format: yaml
  label: Entire VC D API
  slug: entire-vc-d-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entire-vc/openapi/entire-vc-d-api-openapi.yml
- filename: entire-vc-doc-api-openapi.yml
  format: yaml
  label: Entire VC Doc API
  slug: entire-vc-doc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entire-vc/openapi/entire-vc-doc-api-openapi.yml
- filename: entire-vc-ready-api-openapi.yml
  format: yaml
  label: Entire VC Ready API
  slug: entire-vc-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entire-vc/openapi/entire-vc-ready-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Entire VC Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entire VC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Entire VC
provider_slug: entire-vc
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/entire-vc-openapi.yml
  type: http
slug: entire-vc-authentication
source_filename: entire-vc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/entire-vc-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/entire-vc-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/entire-vc/authentication/entire-vc-authentication.yml
summary_line: http · 1 scheme
tags:
- AI toolbox
- Task Management
- Collaboration
- Open Source
- Community
- Workflow catalog
---
