---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: snaplab-dev-account-api-openapi.yml
  format: yaml
  label: snaplab-dev Account API
  slug: snaplab-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-account-api-openapi.yml
- filename: snaplab-dev-billing-api-openapi.yml
  format: yaml
  label: snaplab-dev Billing API
  slug: snaplab-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-billing-api-openapi.yml
- filename: snaplab-dev-captures-api-openapi.yml
  format: yaml
  label: snaplab-dev Captures API
  slug: snaplab-dev-captures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-captures-api-openapi.yml
- filename: snaplab-dev-free-tools-api-openapi.yml
  format: yaml
  label: snaplab-dev Free tools API
  slug: snaplab-dev-free-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-free-tools-api-openapi.yml
- filename: snaplab-dev-rendering-api-openapi.yml
  format: yaml
  label: snaplab-dev Rendering API
  slug: snaplab-dev-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-rendering-api-openapi.yml
- filename: snaplab-dev-system-api-openapi.yml
  format: yaml
  label: snaplab-dev System API
  slug: snaplab-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snaplab-dev/openapi/snaplab-dev-system-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Snaplab Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: snaplab-dev secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: snaplab-dev
provider_slug: snaplab-dev
scheme_count: 3
schemes:
- bearerFormat: sk_<40 chars>
  description: 'Send the key as `Authorization: Bearer sk_…`. This is also how the MCP server at `/mcp` authenticates.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/snaplab-dev-openapi.json
  type: http
- description: 'Signed-URL auth (GET renders only): the API key''s **id**, not its secret. Pair with `sig`.'
  in: query
  name: signedKeyId
  parameter: keyId
  sources:
  - openapi/snaplab-dev-openapi.json
  type: apiKey
- description: '`hex(HMAC_SHA256(signingSecret, canonical))`, where canonical is every query pair except `sig`, sorted by name then value and joined with `&`. Add `expires` (Unix seconds) to time-limit the URL.'
  in: query
  name: signedSignature
  parameter: sig
  sources:
  - openapi/snaplab-dev-openapi.json
  type: apiKey
slug: snaplab-dev-authentication
source_filename: snaplab-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/snaplab-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_<40 chars>\n  description: 'Send the key as `Authorization: Bearer sk_…`. This is also how the MCP server\n    at `/mcp` authenticates.'\n  sources:\n  - openapi/snaplab-dev-openapi.json\n- name: signedKeyId\n  type: apiKey\n  in: query\n  parameter: keyId\n  description: 'Signed-URL auth (GET renders only): the API key''s **id**, not its secret. Pair\n    with `sig`.'\n  sources:\n  - openapi/snaplab-dev-openapi.json\n- name: signedSignature\n  type: apiKey\n  in: query\n  parameter: sig\n  description: '`hex(HMAC_SHA256(signingSecret, canonical))`, where canonical is every query\n    pair except `sig`, sorted by name then value and joined with `&`. Add `expires` (Unix seconds)\n    to time-limit the URL.'\n  sources:\n  - openapi/snaplab-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/snaplab-dev/authentication/snaplab-dev-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Screenshot
- PDF
- OpenGraph
- API
---
