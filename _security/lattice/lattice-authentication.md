---
api_key_in: []
api_specs:
- filename: lattice-competencies-api-openapi.yml
  format: yaml
  label: Lattice Competencies API
  slug: lattice-competencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-competencies-api-openapi.yml
- filename: lattice-departments-api-openapi.yml
  format: yaml
  label: Lattice Departments API
  slug: lattice-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-departments-api-openapi.yml
- filename: lattice-feedbacks-api-openapi.yml
  format: yaml
  label: Lattice Feedbacks API
  slug: lattice-feedbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-feedbacks-api-openapi.yml
- filename: lattice-goal-updates-api-openapi.yml
  format: yaml
  label: Lattice Goal Updates API
  slug: lattice-goal-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-goal-updates-api-openapi.yml
- filename: lattice-goals-api-openapi.yml
  format: yaml
  label: Lattice Goals API
  slug: lattice-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-goals-api-openapi.yml
- filename: lattice-me-api-openapi.yml
  format: yaml
  label: Lattice Me API
  slug: lattice-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-me-api-openapi.yml
- filename: lattice-review-cycles-api-openapi.yml
  format: yaml
  label: Lattice Review Cycles API
  slug: lattice-review-cycles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-review-cycles-api-openapi.yml
- filename: lattice-reviewees-api-openapi.yml
  format: yaml
  label: Lattice Reviewees API
  slug: lattice-reviewees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-reviewees-api-openapi.yml
- filename: lattice-reviews-api-openapi.yml
  format: yaml
  label: Lattice Reviews API
  slug: lattice-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-reviews-api-openapi.yml
- filename: lattice-tags-api-openapi.yml
  format: yaml
  label: Lattice Tags API
  slug: lattice-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-tags-api-openapi.yml
- filename: lattice-users-api-openapi.yml
  format: yaml
  label: Lattice Users API
  slug: lattice-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lattice/refs/heads/main/openapi/lattice-users-api-openapi.yml
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
