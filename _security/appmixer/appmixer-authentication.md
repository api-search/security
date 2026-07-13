---
api_key_in: []
api_specs:
- filename: appmixer-api-openapi.yml
  format: yaml
  label: Appmixer API
  slug: appmixer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/openapi/appmixer-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appmixer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appmixer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appmixer
provider_slug: appmixer
scheme_count: 1
schemes:
- description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer {token} header.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appmixer-api-openapi.yml
  type: http
slug: appmixer-authentication
source_filename: appmixer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/appmixer-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Access token obtained from the /user/auth endpoint. Pass as Authorization: Bearer\n    {token} header.'\n  sources:\n  - openapi/appmixer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appmixer/refs/heads/main/authentication/appmixer-authentication.yml
summary_line: http · 1 scheme
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
---
