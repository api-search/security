---
api_key_in:
- header
api_specs:
- filename: golden-entity-api-api-openapi.yml
  format: yaml
  label: Golden Entity API API
  slug: golden-entity-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-entity-api-api-openapi.yml
- filename: golden-query-api-api-openapi.yml
  format: yaml
  label: Golden Query API API
  slug: golden-query-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-query-api-api-openapi.yml
- filename: golden-schema-api-api-openapi.yml
  format: yaml
  label: Golden Schema API API
  slug: golden-schema-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/openapi/golden-schema-api-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Golden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Golden secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Golden
provider_slug: golden
scheme_count: 1
schemes:
- description: All requests to the Golden Public API v2 authenticate with an API key passed in the `apikey` request header. Keys are issued from the Golden account/API settings. There is no OAuth or user-delegated flow; the key is a static service credential.
  in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/golden-openapi-original.json
  - https://docs.golden.com/openapi.json
  type: apiKey
slug: golden-authentication
source_filename: golden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  openapi/golden-openapi-original.json, re-confirmed against the live spec at\n  https://docs.golden.com/openapi.json and a live unauthenticated call\ndocs: https://docs.golden.com\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: >-\n    All requests to the Golden Public API v2 authenticate with an API key\n    passed in the `apikey` request header. Keys are issued from the Golden\n    account/API settings. There is no OAuth or user-delegated flow; the key\n    is a static service credential.\n  sources:\n  - openapi/golden-openapi-original.json\n  - https://docs.golden.com/openapi.json\noauth: false\noauth_note: >-\n  No OAuth or OpenID Connect surface exists. golden.com returns HTTP 404 for\n  /.well-known/openid-configuration, /.well-known/oauth-authorization-server and\n  /.well-known/oauth-protected-resource.\
  \ No scopes/ artifact is emitted: an\n  api-key-only provider has no scope surface.\nx-evidence:\n  checked: '2026-08-14'\n  probes:\n  - url: https://docs.golden.com/openapi.json\n    status: 200\n    finding: 'components.securitySchemes: {\"ApiKeyAuth\": {\"type\": \"apiKey\", \"in\": \"header\", \"name\": \"apikey\"}}'\n  - url: https://golden.com/api/v2/public/entities/?pageSize=1\n    status: 403\n    finding: >-\n      The live API names the header itself in the failure message —\n      {\"type\":\"client_error\",\"errors\":[{\"code\":\"permission_denied\",\"detail\":\"You\n      didn't pass a valid API Key in the 'apikey' header.\",\"attr\":null}]} —\n      confirming the scheme is enforced in production and not just declared in\n      the spec.\n  - url: https://golden.com/.well-known/openid-configuration\n    status: 404\n    finding: no OIDC discovery document\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden/refs/heads/main/authentication/golden-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Knowledge Graph
- Company Data
- Data
- Entities
- Artificial Intelligence
- Search
- Business Intelligence
---
