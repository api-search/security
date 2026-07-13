---
api_key_in: []
api_specs:
- filename: drone-api-openapi.yml
  format: yaml
  label: Drone REST API
  slug: drone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/openapi/drone-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Drone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Drone secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Drone
provider_slug: drone
scheme_count: 1
schemes:
- description: Bearer token retrieved from the Drone user interface profile page.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/drone-api-openapi.yml
  type: http
slug: drone-authentication
source_filename: drone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/drone-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token retrieved from the Drone user interface profile page.\n  sources:\n  - openapi/drone-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drone/refs/heads/main/authentication/drone-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Containers
- Docker
- Build Automation
- Open Source
- Self-Hosted
---
