---
api_key_in:
- header
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Testsigma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Testsigma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Testsigma
provider_slug: testsigma
scheme_count: 1
schemes:
- bearerFormat: api-key
  description: 'Send the user''s API Key as a Bearer token. The docs show the header as `Authorization: Bearer <API_Key>`. The API Key is generated per-user in the Testsigma app settings.'
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  sources:
  - https://testsigma.com/docs/api/overview/
  type: http
slug: testsigma-authentication
source_filename: testsigma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://testsigma.com/docs/api/overview/\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  notes: >-\n    All Testsigma REST API endpoints require a Bearer token which is the user's\n    personal API Key, generated from the Testsigma app configuration/settings.\n    There is no OAuth2 authorization-code flow and no documented scope surface\n    for the public REST API; the API key carries the user's own permissions.\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: api-key\n    in: header\n    header: Authorization\n    description: >-\n      Send the user's API Key as a Bearer token. The docs show the header as\n      `Authorization: Bearer <API_Key>`. The API Key is generated per-user in\n      the Testsigma app settings.\n    sources: [https://testsigma.com/docs/api/overview/]\ndocs: https://testsigma.com/docs/api/overview/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testsigma/refs/heads/main/authentication/testsigma-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- Testing
- Test Automation
- QA
- DevOps
- Continuous Integration
- Software Quality
- Agentic AI
---
