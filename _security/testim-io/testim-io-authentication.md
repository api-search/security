---
api_key_in: []
api_specs:
- filename: testim-io-openapi.yml
  format: yaml
  label: Testim.io Public API
  slug: testimio-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testim-io/refs/heads/main/openapi/testim-io-openapi.yml
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
