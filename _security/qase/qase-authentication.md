---
api_key_in: []
api_specs:
- filename: qase-cases-api-openapi.yml
  format: yaml
  label: Qase cases API
  slug: qase-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-cases-api-openapi.yml
- filename: qase-defects-api-openapi.yml
  format: yaml
  label: Qase defects API
  slug: qase-defects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-defects-api-openapi.yml
- filename: qase-plans-api-openapi.yml
  format: yaml
  label: Qase plans API
  slug: qase-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-plans-api-openapi.yml
- filename: qase-projects-api-openapi.yml
  format: yaml
  label: Qase projects API
  slug: qase-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-projects-api-openapi.yml
- filename: qase-results-api-openapi.yml
  format: yaml
  label: Qase results API
  slug: qase-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-results-api-openapi.yml
- filename: qase-runs-api-openapi.yml
  format: yaml
  label: Qase runs API
  slug: qase-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-runs-api-openapi.yml
- filename: qase-suites-api-openapi.yml
  format: yaml
  label: Qase suites API
  slug: qase-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/openapi/qase-suites-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qase
provider_slug: qase
scheme_count: 1
schemes:
- description: 'A personal or application API token created in the Qase app under Settings. Passed on every request in the `Token` header (for example, `Token: YOUR_API_TOKEN`). All requests must use HTTPS. Access is further constrained by the user''s role-based permissions.'
  in: header
  name: TokenAuth
  scheme: token
  sources:
  - openapi/qase-openapi.yml
  - https://developers.qase.io/reference/introduction-to-the-qase-api
  type: apiKey
slug: qase-authentication
source_filename: qase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qase-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  scheme: token\n  description: >-\n    A personal or application API token created in the Qase app under Settings.\n    Passed on every request in the `Token` header (for example,\n    `Token: YOUR_API_TOKEN`). All requests must use HTTPS. Access is further\n    constrained by the user's role-based permissions.\n  sources:\n  - openapi/qase-openapi.yml\n  - https://developers.qase.io/reference/introduction-to-the-qase-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qase/refs/heads/main/authentication/qase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Test Runs
- Test Management
- Test Cases
- QA
- Testing
- TestOps
- Test Results
- Defects
- Quality Assurance
- Test Automation
---
