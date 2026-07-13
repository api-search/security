---
api_key_in: []
api_specs:
- filename: grist.yml
  format: yaml
  label: Grist REST API
  slug: grist-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/gristlabs/grist-help/master/api/grist.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Grist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grist
provider_slug: grist
scheme_count: 1
schemes:
- bearerFormat: 'Authorization: Bearer XXXXXXXXXXX'
  description: Access to the Grist API is controlled by an Authorization header, which should contain the word 'Bearer', followed by a space, followed by your API key.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/grist-rest-api-openapi.yml
  type: http
slug: grist-authentication
source_filename: grist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grist-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: 'Authorization: Bearer XXXXXXXXXXX'\n  description: Access to the Grist API is controlled by an Authorization header, which should\n    contain the word 'Bearer', followed by a space, followed by your API key.\n  sources:\n  - openapi/grist-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/authentication/grist-authentication.yml
summary_line: http · 1 scheme
tags:
- Spreadsheet
- Database
- Collaboration
- No-Code
- Data Management
- Webhooks
- Open Source
---
