---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: codequiry-com-auth-api-openapi.yml
  format: yaml
  label: Codequiry Auth API
  slug: codequiry-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-auth-api-openapi.yml
- filename: codequiry-com-checks-api-openapi.yml
  format: yaml
  label: Codequiry Checks API
  slug: codequiry-com-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-checks-api-openapi.yml
- filename: codequiry-com-reference-api-openapi.yml
  format: yaml
  label: Codequiry Reference API
  slug: codequiry-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-reference-api-openapi.yml
- filename: codequiry-com-results-api-openapi.yml
  format: yaml
  label: Codequiry Results API
  slug: codequiry-com-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-results-api-openapi.yml
- filename: codequiry-com-run-api-openapi.yml
  format: yaml
  label: Codequiry Run API
  slug: codequiry-com-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-run-api-openapi.yml
- filename: codequiry-com-submissions-api-openapi.yml
  format: yaml
  label: Codequiry Submissions API
  slug: codequiry-com-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codequiry-com/openapi/codequiry-com-submissions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Codequiry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codequiry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Codequiry
provider_slug: codequiry-com
scheme_count: 1
schemes:
- description: Your 64-character API key from the Codequiry dashboard.
  docs_text: 'Every request requires the header `apikey: <YOUR_API_KEY>` (a 64-character key from your Codequiry dashboard). There is no OAuth or Bearer token, and the key is **not** accepted as a query-string parameter or a body field — header only. A missing or malformed key returns HTTP 401.'
  in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/codequiry-com-openapi.yml
  - https://codequiry.com/llms-full.txt
  type: apiKey
  validate_operation: GET /auth/validate
slug: codequiry-com-authentication
source_filename: codequiry-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codequiry.com/llms-full.txt\ndocs: https://codequiry.com/usage/api/auth\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Your 64-character API key from the Codequiry dashboard.\n  docs_text: \"Every request requires the header `apikey: <YOUR_API_KEY>` (a 64-character key from your Codequiry dashboard). There is no OAuth or Bearer token, and the key is **not** accepted as a query-string parameter or a body field — header only. A missing or malformed key returns HTTP 401.\"\n  validate_operation: GET /auth/validate\n  sources:\n  - openapi/codequiry-com-openapi.yml\n  - https://codequiry.com/llms-full.txt\noauth: none documented (\"There is no OAuth or Bearer token\")\nwebhook_signing:\n  header: X-Codequiry-Signature\n  scheme: \"sha256=<hex>, an HMAC-SHA256 of the raw request body keyed with your API key\"\n"
source_yaml_url: https://artifacts.apis.io/codequiry-com/authentication/codequiry-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Code Plagiarism
- AI Code Detection
- Education
- Source Code Analysis
- Academic Integrity
- MCP
---
