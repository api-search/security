---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Canto REST API
  slug: canto-rest-api
  spec_type: OpenAPI
  url: https://canto1.portal.swaggerhub.com/
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Canto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Canto
provider_slug: canto
scheme_count: 1
schemes:
- bearerFormat: AccessToken
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/canto-pim-openapi.json
  type: http
slug: canto-authentication
source_filename: canto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canto-pim-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: AccessToken\n  sources:\n  - openapi/canto-pim-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canto/refs/heads/main/authentication/canto-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Asset Management
- DAM
- Brand Assets
- Images
- Videos
- Documents
- Media Library
- Asset Distribution
---
