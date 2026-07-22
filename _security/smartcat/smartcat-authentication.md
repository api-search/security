---
api_key_in:
- header
api_specs:
- filename: smartcat-openapi.json
  format: json
  label: Smartcat API v1
  slug: smartcat-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcat/refs/heads/main/openapi/smartcat-openapi.json
auth_types:
- http-basic
description: ''
kind: authentication
layout: security
method: searched
name: Smartcat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smartcat secures its APIs with http-basic across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smartcat
provider_slug: smartcat
scheme_count: 1
schemes:
- credential_source: Settings > API (admin account)
  description: Every Smartcat API method uses HTTP Basic authentication. The Authorization header carries a Base64-encoded "AccountId":"ApiKey" pair. The username is the Account ID (Settings > API), the password is an API key generated with CREATE NEW KEY in the API Keys pane.
  name: basicAuth
  scheme: basic
  sources:
  - https://developers.smartcat.com/api-guides/
  type: http
slug: smartcat-authentication
source_filename: smartcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.smartcat.com/api-guides/\ndocs: https://developers.smartcat.com/api-guides/\nsummary:\n  types: [http-basic]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Every Smartcat API method uses HTTP Basic authentication. The Authorization\n      header carries a Base64-encoded \"AccountId\":\"ApiKey\" pair. The username is the\n      Account ID (Settings > API), the password is an API key generated with\n      CREATE NEW KEY in the API Keys pane.\n    credential_source: Settings > API (admin account)\n    sources: [https://developers.smartcat.com/api-guides/]\nnotes: >-\n  Basic auth is documented in the developer guides but is NOT declared as a\n  securityScheme in the published OpenAPI (components.securitySchemes is empty);\n  captured here from the docs (method: searched). Requests are rate limited to\n  4 req/s. Regional\
  \ hosts: smartcat.com (EU), us.smartcat.com (US), ea.smartcat.com (Asia).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartcat/refs/heads/main/authentication/smartcat-authentication.yml
summary_line: http-basic · 1 scheme
tags:
- Company
- Ai
- Translation
- Localization
- Language
- Machine Translation
- Content
- Translation Management
---
