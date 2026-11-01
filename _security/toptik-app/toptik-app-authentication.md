---
anonymous_access: false
api_key_in: []
api_specs:
- filename: toptik-app-openapi-generated.yml
  format: yaml
  label: toptik-app API
  slug: toptik-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/toptik-app/openapi/_ae-authored/toptik-app-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Toptik App Authentication
name_suffix: Authentication
oauth_flows: []
overview: toptik-app declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: toptik-app
provider_slug: toptik-app
scheme_count: 2
schemes:
- description: RapidAPI subscription key
  in: header
  name: X-RapidAPI-Key
  type: apiKey
- description: Private API key for direct access
  in: header
  name: x-api-key
  type: apiKey
slug: toptik-app-authentication
source_filename: toptik-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://toptik.app/docs/\nschemes:\n  - type: apiKey\n    name: X-RapidAPI-Key\n    in: header\n    description: RapidAPI subscription key\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Private API key for direct access\n"
source_yaml_url: https://artifacts.apis.io/toptik-app/authentication/toptik-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- TikTok
- Data
- Public
---
