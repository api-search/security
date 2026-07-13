---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Smithsonian Open Access API
  slug: smithsonian-open-access-api
  spec_type: OpenAPI
  url: https://edan.si.edu/openaccess/apidocs/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smithsonian Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smithsonian Institution secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Smithsonian Institution
provider_slug: smithsonian
scheme_count: 1
schemes:
- description: API key from https://api.data.gov/signup/
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/smithsonian-open-access-api-openapi.yml
  type: apiKey
slug: smithsonian-authentication
source_filename: smithsonian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smithsonian-open-access-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key from https://api.data.gov/signup/\n  sources:\n  - openapi/smithsonian-open-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithsonian/refs/heads/main/authentication/smithsonian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Museums
- Open Access
- Cultural Heritage
- Collections
- Images
- 3D Models
- Public Domain
- CC0
---
