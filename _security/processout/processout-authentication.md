---
api_key_in: []
api_specs:
- filename: processout-openapi.json
  format: json
  label: ProcessOut API
  slug: processout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-openapi.json
auth_types:
- http
description: 'ProcessOut authenticates every API request with HTTP Basic auth using two project keys: the project ID as the username and a secret API key as the password. Sandbox and production keys are fully separate — the sandbox project ID carries a `test-` prefix and the secret is `key_sandbox_`/`key_test_`; production uses the un-prefixed project ID and a `key_live_` secret. API keys carry per-project permissions set at creation and cannot be edited afterward. The audit-logs endpoint authenticates with the organization ID as username and the API secret as password. Dashboard sign-in additionally supports SAML and OIDC SSO (enterprise).'
kind: authentication
layout: security
method: searched
name: Processout Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProcessOut secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProcessOut
provider_slug: processout
scheme_count: 1
schemes:
- detail: project ID (username) + secret API key (password)
  name: sec0
  scheme: basic
  sources:
  - openapi/processout-openapi.json
  type: http
slug: processout-authentication
source_filename: processout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/processout-openapi.json\ndocs: https://docs.processout.com/reference/getting-started-with-your-api\ndescription: >-\n  ProcessOut authenticates every API request with HTTP Basic auth using two project\n  keys: the project ID as the username and a secret API key as the password. Sandbox\n  and production keys are fully separate — the sandbox project ID carries a `test-`\n  prefix and the secret is `key_sandbox_`/`key_test_`; production uses the un-prefixed\n  project ID and a `key_live_` secret. API keys carry per-project permissions set at\n  creation and cannot be edited afterward. The audit-logs endpoint authenticates with\n  the organization ID as username and the API secret as password. Dashboard sign-in\n  additionally supports SAML and OIDC SSO (enterprise).\nsummary:\n  types:\n    - http\n  http_schemes:\n    - basic\nschemes:\n  - name: sec0\n    type: http\n    scheme: basic\n    detail: project ID (username)\
  \ + secret API key (password)\n    sources:\n      - openapi/processout-openapi.json\nkey_management:\n  docs: https://docs.processout.com/docs/api-keys\n  permissions_required: Developers > Manage API keys\n  immutable: true\n  environments_separate: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/authentication/processout-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Payment Orchestration
- Smart Routing
- Tokenization
- Checkout
- Reconciliation
- Fraud
- 3-D Secure
- Company
---
