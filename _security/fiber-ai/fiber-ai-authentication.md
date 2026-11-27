---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fiber-ai-api-openapi.json
  format: json
  label: Fiber AI API API
  slug: fiber-ai-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fiber-ai/openapi/_original/fiber-ai-api-openapi.json
auth_types: []
description: Authentication for Fiber AI public API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Fiber AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiber AI declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Fiber AI
provider_slug: fiber-ai
scheme_count: 4
schemes:
- evidence: 'Send that key on every call — body/query apiKey , or x-api-key / Authorization: Bearer .'
  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.
  location: query
  name: apiKey
  type: apiKey
- evidence: 'Send that key on every call — body/query apiKey , or x-api-key / Authorization: Bearer .'
  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.
  location: body
  name: apiKey
  type: apiKey
- evidence: 'Send that key on every call — body/query apiKey , or x-api-key / Authorization: Bearer .'
  header: Authorization
  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'Prefer a header over putting the secret in the URL: curl -H "x-api-key: $FIBER_API_KEY " https://api.fiber.ai/v1/get-org-credits'
  header: x-api-key
  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.
  location: header
  name: x-api-key
  type: http
slug: fiber-ai-authentication
source_filename: fiber-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fiber.ai/account/api-keys
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fiber.ai/account/api-keys\nsources:\n- https://docs.fiber.ai/account/api-keys\n- https://docs.fiber.ai/account/quickstart\ndescription: Authentication for Fiber AI public API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: 'Send that key on every call — body/query apiKey , or x-api-key / Authorization: Bearer .'\n  location: query\n  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.\n- type: apiKey\n  name: apiKey\n  evidence: 'Send that key on every call — body/query apiKey , or x-api-key / Authorization: Bearer .'\n  location: body\n  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send that key on every call — body/query\
  \ apiKey , or x-api-key / Authorization: Bearer .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.\n- type: http\n  name: x-api-key\n  evidence: 'Prefer a header over putting the secret in the URL: curl -H \"x-api-key: $FIBER_API_KEY \" https://api.fiber.ai/v1/get-org-credits'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a Fiber API key in the dashboard (fiber.ai/app/api) or via the quickstart script, then store the secret as FIBER_API_KEY.\nnote: The API key can be supplied via query parameter 'apiKey', request body field 'apiKey', header 'x-api-key', or as a Bearer token in the Authorization\n  header.\ndocs: https://docs.fiber.ai/account/api-keys\n"
source_yaml_url: https://artifacts.apis.io/fiber-ai/authentication/fiber-ai-authentication.yml
summary_line: 4 schemes
tags:
- B2B
- Data Platform
- Sales
- Recruiting
- Artificial Intelligence
---
