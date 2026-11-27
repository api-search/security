---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coloringbookify-com-account-api-openapi.yml
  format: yaml
  label: ColoringBookify Account API
  slug: coloringbookify-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-account-api-openapi.yml
- filename: coloringbookify-com-books-api-openapi.yml
  format: yaml
  label: ColoringBookify Books API
  slug: coloringbookify-com-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-books-api-openapi.yml
- filename: coloringbookify-com-characters-api-openapi.yml
  format: yaml
  label: ColoringBookify Characters API
  slug: coloringbookify-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-characters-api-openapi.yml
- filename: coloringbookify-com-operations-api-openapi.yml
  format: yaml
  label: ColoringBookify Operations API
  slug: coloringbookify-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-operations-api-openapi.yml
- filename: coloringbookify-com-pages-api-openapi.yml
  format: yaml
  label: ColoringBookify Pages API
  slug: coloringbookify-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-pages-api-openapi.yml
- filename: coloringbookify-com-planning-api-openapi.yml
  format: yaml
  label: ColoringBookify Planning API
  slug: coloringbookify-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-planning-api-openapi.yml
- filename: coloringbookify-com-print-api-openapi.yml
  format: yaml
  label: ColoringBookify Print API
  slug: coloringbookify-com-print-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coloringbookify-com/openapi/coloringbookify-com-print-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ColoringBookify Authentication
name_suffix: Authentication
oauth_flows: []
overview: ColoringBookify secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ColoringBookify
provider_slug: coloringbookify-com
scheme_count: 2
schemes:
- bearerFormat: ColoringBookify API key
  description: Create one account-level key from the API section in your account, then send it in the Authorization header as a Bearer token. Browser session cookies do not authenticate API requests. The complete key is shown only after creation or rotation.
  key_management: https://coloringbookify.com/api
  key_prefix: cbf_
  location: Authorization header (Bearer)
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/coloringbookify-com-openapi.yml
  type: http
- applies_to: https://coloringbookify.com/mcp
  description: MCP uses OAuth instead of API keys and requires an active Business plan. Compatible clients discover ColoringBookify's OAuth metadata automatically; the browser opens ColoringBookify for sign-in and consent.
  name: mcp-oauth
  sources:
  - https://coloringbookify.com/api/docs
  type: oauth2
slug: coloringbookify-com-authentication
source_filename: coloringbookify-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coloringbookify.com/api/docs\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ColoringBookify API key\n  sources:\n  - openapi/coloringbookify-com-openapi.yml\n  key_prefix: cbf_\n  location: Authorization header (Bearer)\n  description: Create one account-level key from the API section in your account,\n    then send it in the Authorization header as a Bearer token. Browser session cookies\n    do not authenticate API requests. The complete key is shown only after creation\n    or rotation.\n  key_management: https://coloringbookify.com/api\n- name: mcp-oauth\n  type: oauth2\n  applies_to: https://coloringbookify.com/mcp\n  description: MCP uses OAuth instead of API keys and requires an active Business\n    plan. Compatible clients discover ColoringBookify's OAuth metadata automatically;\n    the browser opens ColoringBookify for sign-in and\
  \ consent.\n  sources:\n  - https://coloringbookify.com/api/docs\ndocs: https://coloringbookify.com/api/docs#authentication\n"
source_yaml_url: https://artifacts.apis.io/coloringbookify-com/authentication/coloringbookify-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Coloring Books
- Image Generation
- PDF Generation
- Printing
- Publishing
- MCP
---
