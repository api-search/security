---
api_key_in:
- header
api_specs:
- filename: apigit-apis-api-openapi.yml
  format: yaml
  label: APIGit APIs API
  slug: apigit-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/openapi/apigit-apis-api-openapi.yml
- filename: apigit-mocks-api-openapi.yml
  format: yaml
  label: APIGit Mocks API
  slug: apigit-mocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/openapi/apigit-mocks-api-openapi.yml
- filename: apigit-repositories-api-openapi.yml
  format: yaml
  label: APIGit Repositories API
  slug: apigit-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/openapi/apigit-repositories-api-openapi.yml
- filename: apigit-tests-api-openapi.yml
  format: yaml
  label: APIGit Tests API
  slug: apigit-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/openapi/apigit-tests-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apigit Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIGit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIGit
provider_slug: apigit
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/apigit-api.yaml
  type: apiKey
slug: apigit-authentication
source_filename: apigit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apigit-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/apigit-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigit/refs/heads/main/authentication/apigit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Design
- API Lifecycle
- Documentation
- Git
- Governance
- Mocking
- Platform
- Testing
---
