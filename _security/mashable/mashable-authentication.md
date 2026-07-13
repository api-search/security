---
api_key_in:
- header
api_specs:
- filename: mashable-openapi.yml
  format: yaml
  label: Mashable via News API
  slug: mashable-via-newsapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mashable/refs/heads/main/openapi/mashable-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mashable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mashable secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mashable
provider_slug: mashable
scheme_count: 1
schemes:
- description: News API key. May also be passed via apiKey query parameter.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/mashable-openapi.yml
  type: apiKey
slug: mashable-authentication
source_filename: mashable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mashable-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: News API key. May also be passed via apiKey query parameter.\n  sources:\n  - openapi/mashable-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mashable/refs/heads/main/authentication/mashable-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Articles
- Digital Culture
- Headlines
- Media
- News
- Technology News
---
