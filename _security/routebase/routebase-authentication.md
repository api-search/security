---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Routebase API
  slug: routebase-api
  spec_type: OpenAPI
  url: https://docs.routebase.dev/api/routebase-public-api/openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Routebase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routebase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Routebase
provider_slug: routebase
scheme_count: 2
schemes:
- description: 'An organization API key, created under Settings then API Keys. Keys start with

    `rb_live_` and carry their own permission scopes, so a key only reaches what it

    was granted.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/routebase-public-api-openapi.json
  type: apiKey
- description: 'The SCIM token of the organization, issued when SCIM provisioning is enabled.

    It is separate from an API key and only unlocks the SCIM endpoints.'
  name: ScimBearerAuth
  scheme: bearer
  sources:
  - openapi/routebase-public-api-openapi.json
  type: http
slug: routebase-authentication
source_filename: routebase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: derived\nsource: openapi/routebase-public-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    An organization API key, created under Settings then API Keys. Keys start with\n    `rb_live_` and carry their own permission scopes, so a key only reaches what it\n    was granted.\n  sources:\n  - openapi/routebase-public-api-openapi.json\n- name: ScimBearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    The SCIM token of the organization, issued when SCIM provisioning is enabled.\n    It is separate from an API key and only unlocks the SCIM endpoints.\n  sources:\n  - openapi/routebase-public-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/authentication/routebase-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- API lifecycle management
- API design
- OpenAPI
- API documentation
- API testing
- API mocking
- API monitoring
- API security
- MCP
- AI agents
- developer tools
- CI/CD
- REST
- OAuth 2.1
- SCIM
- Streamable HTTP
---
