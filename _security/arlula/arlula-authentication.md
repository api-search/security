---
api_key_in: []
api_specs:
- filename: arlula-openapi.yaml
  format: yaml
  label: Arlula API
  slug: arlula-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/openapi/arlula-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Arlula Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arlula secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arlula
provider_slug: arlula
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using API Key as username and API Secret as password. Credentials are obtained from the Arlula dashboard at https://dashboard.arlula.com/apis.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/arlula-openapi.yaml
  type: http
slug: arlula-authentication
source_filename: arlula-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arlula-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using API Key as username and API Secret as password.\n    Credentials are obtained from the Arlula dashboard at https://dashboard.arlula.com/apis.\n  sources:\n  - openapi/arlula-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/authentication/arlula-authentication.yml
summary_line: http · 1 scheme
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
---
