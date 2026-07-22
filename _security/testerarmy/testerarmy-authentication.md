---
api_key_in:
- header
api_specs:
- filename: testerarmy-openapi-original.json
  format: json
  label: TesterArmy API
  slug: testerarmy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/testerarmy/refs/heads/main/openapi/testerarmy-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Testerarmy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testerarmy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Testerarmy
provider_slug: testerarmy
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: API key authentication using Bearer token format
  location: header (Authorization)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/testerarmy-openapi-original.json
  type: http
slug: testerarmy-authentication
source_filename: testerarmy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tester.army/api/v1/openapi.json\ndocs: https://docs.tester.army/api-reference\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    TesterArmy uses API-key authentication passed as an HTTP Bearer token\n    (Authorization: Bearer <API_KEY>). API keys are created in the dashboard.\n    No OAuth2/OIDC surface is exposed by the public API.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: API Key\n    description: API key authentication using Bearer token format\n    location: header (Authorization)\n    sources: [openapi/testerarmy-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testerarmy/refs/heads/main/authentication/testerarmy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- QA
- Software Testing
- Browser Automation
- AI Agents
- Developer Tools
- CI/CD
- End-to-End Testing
- Mobile Testing
---
