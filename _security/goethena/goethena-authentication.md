---
api_key_in: []
api_specs:
- filename: goethena-openapi-original.yml
  format: yaml
  label: Ethena API
  slug: ethena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/openapi/goethena-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Goethena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goethena secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Goethena
provider_slug: goethena
scheme_count: 1
schemes:
- description: Send requests with the Authorization header that contains the word `Basic` followed by a space and a base64-encoded string of the username and api key, `username:apiKey`.
  name: basic_auth
  scheme: basic
  sources:
  - openapi/goethena-openapi-original.yml
  type: http
slug: goethena-authentication
source_filename: goethena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/goethena-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Send requests with the Authorization header that contains the word `Basic` followed\n    by a space and a base64-encoded string of the username and api key, `username:apiKey`.\n  sources:\n  - openapi/goethena-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goethena/refs/heads/main/authentication/goethena-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Compliance
- Training
- Human Resources
- Ethics
- Learning Management
- AI Agents
- Governance
- Workforce
---
