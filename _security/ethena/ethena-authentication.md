---
api_key_in: []
api_specs:
- filename: ethena-openapi-original.yml
  format: yaml
  label: Ethena API
  slug: ethena-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ethena/refs/heads/main/openapi/ethena-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ethena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethena secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ethena
provider_slug: ethena
scheme_count: 1
schemes:
- description: Send requests with the Authorization header that contains the word `Basic` followed by a space and a base64-encoded string of the username and api key, `username:apiKey`.
  name: basic_auth
  scheme: basic
  sources:
  - openapi/ethena-openapi-original.yml
  type: http
slug: ethena-authentication
source_filename: ethena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/ethena-openapi-original.yml\ndocs: https://help.goethena.com/hc/en-us/articles/28796851013773-Ethena-s-API\nsummary:\n  types:\n  - http\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  description: Send requests with the Authorization header that contains the word `Basic` followed\n    by a space and a base64-encoded string of the username and api key, `username:apiKey`.\n  sources:\n  - openapi/ethena-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethena/refs/heads/main/authentication/ethena-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Compliance
- Training
- Governance, Risk and Compliance
- Human Resources
- Learning Management
- Workflow
- Webhooks
---
