---
api_key_in:
- header
api_specs:
- filename: vitally-rest-openapi.yml
  format: yaml
  label: Vitally REST API
  slug: vitally-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitally/refs/heads/main/openapi/vitally-rest-openapi.yml
auth_types:
- http
description: Vitally's REST API authenticates with HTTP Basic authentication using a Vitally REST API key as the username and an empty password. Keys are created and managed in the Vitally UI under Settings -> Integrations -> Vitally REST API, where each key has an editable name, a copyable secret token, a copyable Basic Auth header, and per-key regenerate / revoke controls. Multiple keys can coexist for different integrations or environments. The Vitally MCP server authenticates separately with OAuth (see mcp/vitally-mcp.yml).
kind: authentication
layout: security
method: searched
name: Vitally Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vitally secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vitally
provider_slug: vitally
scheme_count: 1
schemes:
- description: 'Basic auth with the REST API key as the username and an empty password. The docs also show the pre-computed header form, e.g. ''Authorization: Basic c2VjcmV0X2tleTo=''.'
  format: 'Authorization: Basic base64(<api_key>:)'
  header: Authorization
  in: header
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vitally-rest-openapi.yml
  type: http
slug: vitally-authentication
source_filename: vitally-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vitally.io/en/articles/9880649-rest-api-overview\ndocs: https://docs.vitally.io/en/articles/9880649-rest-api-overview\ndescription: >-\n  Vitally's REST API authenticates with HTTP Basic authentication using a\n  Vitally REST API key as the username and an empty password. Keys are created\n  and managed in the Vitally UI under Settings -> Integrations -> Vitally REST\n  API, where each key has an editable name, a copyable secret token, a copyable\n  Basic Auth header, and per-key regenerate / revoke controls. Multiple keys can\n  coexist for different integrations or environments. The Vitally MCP server\n  authenticates separately with OAuth (see mcp/vitally-mcp.yml).\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    in: header\n    header: Authorization\n    format: 'Authorization: Basic base64(<api_key>:)'\n\
  \    description: >-\n      Basic auth with the REST API key as the username and an empty password.\n      The docs also show the pre-computed header form, e.g.\n      'Authorization: Basic c2VjcmV0X2tleTo='.\n    sources:\n      - openapi/vitally-rest-openapi.yml\nkey_management:\n  location: 'Settings -> Integrations -> Vitally REST API (Quick Jump: Cmd/Alt + j)'\n  multiple_keys: true\n  rotation: Keys can be rolled (regenerated) or revoked individually.\nrelated:\n  mcp_oauth: mcp/vitally-mcp.yml\n  data_centers:\n    us: https://{subdomain}.rest.vitally.io\n    eu: https://rest.vitally-eu.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitally/refs/heads/main/authentication/vitally-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Customer Success
- SaaS
- CRM
- NPS
- Surveys
- Analytics
- Artificial Intelligence
---
