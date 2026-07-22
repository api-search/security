---
api_key_in: []
api_specs:
- filename: qa-wolf-rest-openapi.yml
  format: yaml
  label: QA Wolf REST API
  slug: qa-wolf-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qa-wolf/refs/heads/main/openapi/qa-wolf-rest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qa Wolf Authentication
name_suffix: Authentication
oauth_flows: []
overview: QA Wolf secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: QA Wolf
provider_slug: qa-wolf
scheme_count: 1
schemes:
- description: Bearer token using the workspace API key (QAWOLF_API_KEY). Find the key in the platform under Workspace Settings -> Integrations -> API Access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/qa-wolf-rest-openapi.yml
  type: http
slug: qa-wolf-authentication
source_filename: qa-wolf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/qa-wolf-rest-openapi.yml\ndocs: https://docs.qawolf.com/qawolf/local-execution/authenticate\nnotes: >-\n  API access uses a workspace API key (QAWOLF_API_KEY) passed as a bearer token\n  in the Authorization header. Platform sign-in additionally supports SSO via an\n  identity provider (Okta, OneLogin, Entra ID) and MFA. Inbound bug-tracker\n  webhooks from QA Wolf can carry optional HTTP basic auth.\nsso:\n  supported: true\n  providers: [Okta, OneLogin, Entra ID]\n  docs: https://docs.qawolf.com/qawolf/sso\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token using the workspace API key (QAWOLF_API_KEY). Find the key in the\n    platform under Workspace Settings -> Integrations -> API Access.\n  sources:\n  - openapi/qa-wolf-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qa-wolf/refs/heads/main/authentication/qa-wolf-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Devtools
- Testing
- Test Automation
- QA
- CI/CD
- Playwright
- Developer Tools
---
