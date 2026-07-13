---
api_key_in: []
api_specs:
- filename: lattice-talent-openapi.yml
  format: yaml
  label: Lattice Talent API
  slug: lattice-talent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-talent-openapi.yml
- filename: lattice-hris-openapi.yml
  format: yaml
  label: Lattice HRIS API
  slug: lattice-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-hris-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lattice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lattice secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lattice
provider_slug: lattice
scheme_count: 1
schemes:
- description: 'Service account API key passed as a Bearer token in the Authorization header. Example: Authorization: Bearer <your-api-key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lattice-hris-openapi.yml
  - openapi/lattice-talent-openapi.yml
  type: http
slug: lattice-authentication
source_filename: lattice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lattice-hris-openapi.yml, openapi/lattice-talent-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Service account API key passed as a Bearer token in the Authorization header.\n    Example: Authorization: Bearer <your-api-key>'\n  sources:\n  - openapi/lattice-hris-openapi.yml\n  - openapi/lattice-talent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/authentication/lattice-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- People Management
- Performance Management
- OKRs
- Goals
- Employee Engagement
- HRIS
- Compensation
- Feedback
- Surveys
---
