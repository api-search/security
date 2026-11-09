---
anonymous_access: false
api_key_in: []
api_specs:
- filename: call4-me-balance-api-openapi.yml
  format: yaml
  label: call4me Balance API
  slug: call4-me-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-balance-api-openapi.yml
- filename: call4-me-call4me-api-api-openapi.yml
  format: yaml
  label: call4me Call4me API
  slug: call4-me-call4me-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-call4me-api-api-openapi.yml
- filename: call4-me-calls-api-openapi.yml
  format: yaml
  label: call4me Calls API
  slug: call4-me-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-calls-api-openapi.yml
- filename: call4-me-numbers-api-openapi.yml
  format: yaml
  label: call4me Numbers API
  slug: call4-me-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-numbers-api-openapi.yml
- filename: call4-me-profile-api-openapi.yml
  format: yaml
  label: call4me Profile API
  slug: call4-me-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-profile-api-openapi.yml
- filename: call4-me-requirements-api-openapi.yml
  format: yaml
  label: call4me Requirements API
  slug: call4-me-requirements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-requirements-api-openapi.yml
- filename: call4-me-scheduled-calls-api-openapi.yml
  format: yaml
  label: call4me Scheduled Calls API
  slug: call4-me-scheduled-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-scheduled-calls-api-openapi.yml
- filename: call4-me-x402-api-openapi.yml
  format: yaml
  label: call4me X402 API
  slug: call4-me-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/call4-me/openapi/call4-me-x402-api-openapi.yml
auth_types: []
description: Authentication methods for call4me as documented on the provider pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Call4 Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: call4me declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: call4me
provider_slug: call4-me
scheme_count: 1
schemes:
- evidence: 'It works as `Authorization: Bearer <key>` on https://call4.me/mcp and https://call4.me/api, or in the URL as https://call4.me/mcp/<key> for clients that cannot sign in or set headers.'
  how_to_obtain: User creates an API key in their account at https://call4.me/account; the key is then used as a Bearer token.
  name: API Key
  type: http-bearer
slug: call4-me-authentication
source_filename: call4-me-authentication.yml
source_heading: Authentication Profile
source_url: https://call4.me/auth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://call4.me/auth.md\nsources:\n- https://call4.me/auth.md\n- https://call4.me/blog/paradox-hotel-vancouver\n- https://call4.me/blog/grok-bot-template-troubleshooting\n- https://call4.me/blog/phone-calling-mcp-comparison\ndescription: Authentication methods for call4me as documented on the provider pages.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'It works as `Authorization: Bearer <key>` on https://call4.me/mcp and https://call4.me/api, or in the URL as https://call4.me/mcp/<key>\n    for clients that cannot sign in or set headers.'\n  how_to_obtain: User creates an API key in their account at https://call4.me/account; the key is then used as a Bearer token.\ndocs: https://call4.me/auth.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/call4-me/authentication/call4-me-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Telephony
- Automation
- Software-as-a-Service
- Call4me
---
