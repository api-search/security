---
anonymous_access: false
api_key_in: []
api_specs:
- filename: poof-bg-account-api-openapi.yml
  format: yaml
  label: poof-bg Account API
  slug: poof-bg-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/poof-bg/openapi/poof-bg-account-api-openapi.yml
- filename: poof-bg-background-removal-api-openapi.yml
  format: yaml
  label: poof-bg Background Removal API
  slug: poof-bg-background-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/poof-bg/openapi/poof-bg-background-removal-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Poof Bg Authentication
name_suffix: Authentication
oauth_flows: []
overview: poof-bg declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: poof-bg
provider_slug: poof-bg
scheme_count: 1
schemes:
- description: Your API key. Get one at https://dash.poof.bg
  in: header
  name: x-api-key
  type: apiKey
slug: poof-bg-authentication
source_filename: poof-bg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/poof-bg-openapi.json\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Your API key. Get one at https://dash.poof.bg\n"
source_yaml_url: https://artifacts.apis.io/poof-bg/authentication/poof-bg-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- BackgroundRemoval
- ImageProcessing
- VideoProcessing
---
