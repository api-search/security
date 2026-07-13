---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acceptance Criteria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acceptance Criteria secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/acceptance-criteria-management.yaml
  type: http
slug: acceptance-criteria-authentication
source_filename: acceptance-criteria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acceptance-criteria-management.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/acceptance-criteria-management.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/authentication/acceptance-criteria-authentication.yml
summary_line: http · 1 scheme
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
---
