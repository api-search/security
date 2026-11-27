---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-fonts-webfonts-api-openapi.yml
  format: yaml
  label: Google Fonts Developer Fonts Webfonts API
  slug: google-fonts-webfonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-fonts/openapi/google-fonts-webfonts-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Google Fonts Developer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Google Fonts Developer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Google Fonts Developer
provider_slug: google-fonts
scheme_count: 1
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-fonts-webfonts-api-openapi.yml
  type: apiKey
slug: google-fonts-authentication
source_filename: google-fonts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-fonts-webfonts-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-fonts-webfonts-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-fonts/authentication/google-fonts-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CSS
- Design
- Fonts
- Google Fonts
- Typography
- Web Fonts
---
