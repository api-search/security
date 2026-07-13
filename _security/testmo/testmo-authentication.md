---
api_key_in: []
api_specs:
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Test Runs API
  slug: testmo-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Automation Runs API
  slug: testmo-automation-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Automation Sources API
  slug: testmo-automation-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Sessions API
  slug: testmo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Projects API
  slug: testmo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Milestones API
  slug: testmo-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
- filename: testmo-openapi.yml
  format: yaml
  label: Testmo Test Case Management API
  slug: testmo-test-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/openapi/testmo-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Testmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testmo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Testmo
provider_slug: testmo
scheme_count: 1
schemes:
- description: 'Personal API token generated from your Testmo profile page, passed as `Authorization: Bearer <token>`. The API is per-instance at https://{instance}.testmo.net/api/v1 and access is scoped to the token user''s permissions; some endpoints (users, groups, roles) are admin-only.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/testmo-openapi.yml
  type: http
slug: testmo-authentication
source_filename: testmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/testmo-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal API token generated from your Testmo profile page, passed as `Authorization:\n    Bearer <token>`. The API is per-instance at https://{instance}.testmo.net/api/v1 and access\n    is scoped to the token user''s permissions; some endpoints (users, groups, roles) are admin-only.'\n  sources:\n  - openapi/testmo-openapi.yml\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testmo/refs/heads/main/authentication/testmo-authentication.yml
summary_line: http · 1 scheme
tags:
- Test Runs
- Test Management
- Test Automation
- QA
- Exploratory Testing
- CI/CD
- Quality Assurance
---
