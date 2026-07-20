---
api_key_in:
- query
api_specs:
- filename: testmail-app-json-api-openapi.yml
  format: yaml
  label: Testmail JSON API
  slug: testmail-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-json-api-openapi.yml
- filename: testmail-app-graphql-api-openapi.yml
  format: yaml
  label: Testmail GraphQL API
  slug: testmail-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/openapi/testmail-app-graphql-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Testmail App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testmail secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Testmail
provider_slug: testmail-app
scheme_count: 2
schemes:
- description: 'API key as Bearer token. Obtain from the Testmail developer console and pass as: Authorization: Bearer [example key]'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/testmail-app-graphql-api-openapi.yml
  type: http
- description: API key retrieved from the Testmail developer console.
  in: query
  name: ApiKeyQuery
  parameter: apikey
  sources:
  - openapi/testmail-app-json-api-openapi.yml
  type: apiKey
slug: testmail-app-authentication
source_filename: testmail-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/testmail-app-graphql-api-openapi.yml, openapi/testmail-app-json-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key as Bearer token. Obtain from the Testmail developer console and pass\n    as: Authorization: Bearer [example key]'\n  sources:\n  - openapi/testmail-app-graphql-api-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key retrieved from the Testmail developer console.\n  sources:\n  - openapi/testmail-app-json-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testmail-app/refs/heads/main/authentication/testmail-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email Testing
- Developer Tools
- API Testing
- GraphQL
- REST API
- CI/CD
- QA Automation
- Programmable Inboxes
---
