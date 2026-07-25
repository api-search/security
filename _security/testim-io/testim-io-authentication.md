---
api_key_in: []
api_specs:
- filename: testim-io-branches-api-openapi.yml
  format: yaml
  label: Testim Io Branches API
  slug: testim-io-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-branches-api-openapi.yml
- filename: testim-io-executions-api-openapi.yml
  format: yaml
  label: Testim Io Executions API
  slug: testim-io-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-executions-api-openapi.yml
- filename: testim-io-labels-api-openapi.yml
  format: yaml
  label: Testim Io Labels API
  slug: testim-io-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-labels-api-openapi.yml
- filename: testim-io-mobile-applications-api-openapi.yml
  format: yaml
  label: Testim Io Mobile Applications API
  slug: testim-io-mobile-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-mobile-applications-api-openapi.yml
- filename: testim-io-suites-api-openapi.yml
  format: yaml
  label: Testim Io Suites API
  slug: testim-io-suites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-suites-api-openapi.yml
- filename: testim-io-test-plans-api-openapi.yml
  format: yaml
  label: Testim Io Test plans API
  slug: testim-io-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-test-plans-api-openapi.yml
- filename: testim-io-tests-api-openapi.yml
  format: yaml
  label: Testim Io Tests API
  slug: testim-io-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-tests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Testim Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testim Io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Testim Io
provider_slug: testim-io
scheme_count: 1
schemes:
- bearerFormat: PAK-[RANDOM_KEY]
  header: 'Authorization: Bearer PAK-<key>'
  key_management: Generate/revoke keys in the Testim app under Settings > API.
  name: apiKeyAuth
  plan_requirement: The public REST API requires a Professional (Pro) tier project.
  scheme: bearer
  sources:
  - openapi/testim-io-openapi.yml
  - https://docs.tricentis.com/testim/content/administration/api-access.htm
  type: http
slug: testim-io-authentication
source_filename: testim-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tricentis.com/testim/content/administration/api-access.htm\ndocs: https://docs.tricentis.com/testim/content/administration/api-access.htm\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAK-[RANDOM_KEY]\n  header: 'Authorization: Bearer PAK-<key>'\n  key_management: Generate/revoke keys in the Testim app under Settings > API.\n  plan_requirement: The public REST API requires a Professional (Pro) tier project.\n  sources:\n  - openapi/testim-io-openapi.yml\n  - https://docs.tricentis.com/testim/content/administration/api-access.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/authentication/testim-io-authentication.yml
summary_line: http · 1 scheme
tags:
- API Testing
- Test Automation
- Quality Assurance
- CI/CD
- Mobile Testing
- Software Testing
- DevOps
- Company
---
