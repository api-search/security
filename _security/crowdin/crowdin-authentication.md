---
api_key_in: []
api_specs:
- filename: crowdin-openapi.yml
  format: yaml
  label: Crowdin REST API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdin/refs/heads/main/openapi/crowdin-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Crowdin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crowdin secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crowdin
provider_slug: crowdin
scheme_count: 1
schemes:
- bearerFormat: PAT
  description: Personal Access Token or OAuth 2 bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crowdin-openapi.yml
  type: http
slug: crowdin-authentication
source_filename: crowdin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crowdin-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  description: Personal Access Token or OAuth 2 bearer token\n  sources:\n  - openapi/crowdin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdin/refs/heads/main/authentication/crowdin-authentication.yml
summary_line: http · 1 scheme
tags:
- Localization
- Translation
- TMS
- REST
- GraphQL
- Developer Tools
- Enterprise
---
