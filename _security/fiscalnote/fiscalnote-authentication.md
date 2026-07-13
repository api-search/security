---
api_key_in:
- header
api_specs:
- filename: fiscalnote-policynote-openapi.yml
  format: yaml
  label: FiscalNote PolicyNote API
  slug: policynote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-policynote-openapi.yml
- filename: fiscalnote-appdata-openapi.yml
  format: yaml
  label: FiscalNote AppData API
  slug: appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-appdata-openapi.yml
- filename: fiscalnote-people-openapi.yml
  format: yaml
  label: FiscalNote People API
  slug: people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-people-openapi.yml
- filename: fiscalnote-organization-openapi.yml
  format: yaml
  label: FiscalNote Organization API
  slug: organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-organization-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fiscalnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: FiscalNote secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FiscalNote
provider_slug: fiscalnote
scheme_count: 1
schemes:
- description: API key provided by FiscalNote. Include in the Authorization header of each request.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/fiscalnote-appdata-openapi.yml
  - openapi/fiscalnote-organization-openapi.yml
  - openapi/fiscalnote-people-openapi.yml
  - openapi/fiscalnote-policynote-openapi.yml
  type: apiKey
slug: fiscalnote-authentication
source_filename: fiscalnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fiscalnote-appdata-openapi.yml, openapi/fiscalnote-organization-openapi.yml,\n  openapi/fiscalnote-people-openapi.yml, openapi/fiscalnote-policynote-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key provided by FiscalNote. Include in the Authorization header of each request.\n  sources:\n  - openapi/fiscalnote-appdata-openapi.yml\n  - openapi/fiscalnote-organization-openapi.yml\n  - openapi/fiscalnote-people-openapi.yml\n  - openapi/fiscalnote-policynote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/authentication/fiscalnote-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
---
