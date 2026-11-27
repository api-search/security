---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cherishedbook-com-auth-api-openapi.yml
  format: yaml
  label: Cherished Book Auth API
  slug: cherishedbook-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-auth-api-openapi.yml
- filename: cherishedbook-com-contributions-api-openapi.yml
  format: yaml
  label: Cherished Book Contributions API
  slug: cherishedbook-com-contributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-contributions-api-openapi.yml
- filename: cherishedbook-com-me-api-openapi.yml
  format: yaml
  label: Cherished Book Me API
  slug: cherishedbook-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-me-api-openapi.yml
- filename: cherishedbook-com-memorials-api-openapi.yml
  format: yaml
  label: Cherished Book Memorials API
  slug: cherishedbook-com-memorials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-memorials-api-openapi.yml
- filename: cherishedbook-com-organization-api-openapi.yml
  format: yaml
  label: Cherished Book Organization API
  slug: cherishedbook-com-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-organization-api-openapi.yml
- filename: cherishedbook-com-owners-api-openapi.yml
  format: yaml
  label: Cherished Book Owners API
  slug: cherishedbook-com-owners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-owners-api-openapi.yml
- filename: cherishedbook-com-ping-api-openapi.yml
  format: yaml
  label: Cherished Book Ping API
  slug: cherishedbook-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherishedbook-com/openapi/cherishedbook-com-ping-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cherished Book Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cherished Book secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cherished Book
provider_slug: cherishedbook-com
scheme_count: 1
schemes:
- description: 'API token, sent as `Authorization: Bearer <token>`.

    A personal token is obtained through the device flow (`POST /auth/device`), or by hand from Connected apps in account settings. Rate limited to 20 requests/minute.

    A business token is created by a Business Admin in Business settings → API tokens, is shown once, and scopes to that organization. Rate limited to 50 requests/minute.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cherishedbook-com-openapi.yml
  - https://www.cherishedbook.com/developers
  type: http
slug: cherishedbook-com-authentication
source_filename: cherishedbook-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://www.cherishedbook.com/developers\ndocs: https://www.cherishedbook.com/developers\nagent_docs: https://www.cherishedbook.com/developers/ai.md\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API token, sent as `Authorization: Bearer <token>`.\n    A personal token is obtained through the device flow (`POST /auth/device`), or by hand from Connected apps in account settings. Rate limited to 20 requests/minute.\n    A business token is created by a Business Admin in Business settings → API tokens, is shown once, and scopes to that organization. Rate limited to 50 requests/minute.\n  sources:\n  - openapi/cherishedbook-com-openapi.yml\n  - https://www.cherishedbook.com/developers\ntoken_kinds:\n- name: personal token\n  acquisition: device authorization flow (POST /auth/device, then poll POST /auth/token; 400 authorization_pending while waiting), or by hand\
  \ from Connected apps in account settings\n  scope: \"acts for one person, on memorials they look after\"\n  source: https://www.cherishedbook.com/developers/ai.md\n- name: business token\n  acquisition: \"A Business Admin creates a token in Business settings, under API tokens. It is shown once\"\n  scope: \"bound to one organisation (funeral homes, celebrants) and only ever sees that organisation's data\"\n  revocation: \"You can revoke a token at any time from the same screen.\"\n  source: https://www.cherishedbook.com/developers\nmcp:\n  endpoint: https://app.cherishedbook.com/api/mcp\n  auth: \"Authenticate it with a personal token.\"\n  source: https://www.cherishedbook.com/developers/ai.md\n"
source_yaml_url: https://artifacts.apis.io/cherishedbook-com/authentication/cherishedbook-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Memorials
- Online Memorials
- Funeral Services
- Grief Support
- Consumer
- MCP
- AI Agents
---
