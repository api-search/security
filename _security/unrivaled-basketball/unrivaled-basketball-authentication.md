---
api_key_in:
- header
api_specs:
- filename: unrivaled-basketball-openapi.yml
  format: yaml
  label: Unrivaled API
  slug: unrivaled-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/openapi/unrivaled-basketball-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Unrivaled Basketball Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unrivaled Basketball secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unrivaled Basketball
provider_slug: unrivaled-basketball
scheme_count: 1
schemes:
- access_levels:
  - trial
  - production
  in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/unrivaled-basketball-openapi.yml
  type: apiKey
slug: unrivaled-basketball-authentication
source_filename: unrivaled-basketball-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/unrivaled-basketball-openapi.yml\ndocs: https://developer.sportradar.com/basketball/docs/unrivaled-ig-api-basics\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Authentication is required for all Unrivaled API calls. The API is operated\n  by Sportradar as the league's Official Data Provider; HTTP requests are\n  made using the API authentication access established in a Sportradar\n  account. The key is sent in the `x-api-key` header, and the key's access\n  level (`trial` or `production`) is also encoded as the first path segment\n  of every request. Applications must support TLS 1.2 or above.\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  access_levels:\n  - trial\n  - production\n  sources:\n  - openapi/unrivaled-basketball-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unrivaled-basketball/refs/heads/main/authentication/unrivaled-basketball-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Basketball
- Sports
- Womens Sports
- Sports Data
- Media
- League
---
