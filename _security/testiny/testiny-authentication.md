---
api_key_in: []
api_specs:
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Runs API
  slug: testiny-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Cases API
  slug: testiny-test-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Test Plans API
  slug: testiny-test-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Projects API
  slug: testiny-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
- filename: testiny-openapi.yml
  format: yaml
  label: Testiny Automation API
  slug: testiny-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/openapi/testiny-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Testiny Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testiny secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Testiny
provider_slug: testiny
scheme_count: 1
schemes:
- description: 'API key created in Testiny with fine-grained permissions scoped to your organization. Passed as the `X-Api-Key` request header. The MCP server additionally supports an `Authorization: Bearer <key>` header or browser-based OAuth. Treat the API key like a password.'
  in: header
  name: ApiKeyAuth
  parameterName: X-Api-Key
  sources:
  - openapi/testiny-openapi.yml
  - https://www.testiny.io/docs/api-quickstart/
  - https://www.testiny.io/docs/mcp-server/
  type: apiKey
slug: testiny-authentication
source_filename: testiny-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/testiny-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameterName: X-Api-Key\n  description: 'API key created in Testiny with fine-grained permissions scoped to your\n    organization. Passed as the `X-Api-Key` request header. The MCP server additionally\n    supports an `Authorization: Bearer <key>` header or browser-based OAuth. Treat the\n    API key like a password.'\n  sources:\n  - openapi/testiny-openapi.yml\n  - https://www.testiny.io/docs/api-quickstart/\n  - https://www.testiny.io/docs/mcp-server/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testiny/refs/heads/main/authentication/testiny-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Test Runs
- Test Management
- QA
- Test Cases
- Test Automation
- Quality Assurance
- Testing
---
