---
api_key_in:
- header
api_specs:
- filename: rentcheck-openapi-original.yml
  format: yaml
  label: RentCheck REST API
  slug: rentcheck-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentcheck/refs/heads/main/openapi/rentcheck-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rentcheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: RentCheck secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RentCheck
provider_slug: rentcheck
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Authorization key needed to use the API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rentcheck-openapi-original.yml
  type: http
- description: Represents the identification of you application
  in: header
  name: x-app-id
  parameter: x-app-id
  sources:
  - openapi/rentcheck-openapi-original.yml
  type: apiKey
- description: Represents the secret for your application
  in: header
  name: x-app-secret
  parameter: x-app-secret
  sources:
  - openapi/rentcheck-openapi-original.yml
  type: apiKey
slug: rentcheck-authentication
source_filename: rentcheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/rentcheck-openapi-original.yml\ndocs: https://developers.getrentcheck.com/\nnotes: >-\n  Requests require three headers: a Bearer JWT access token (Authorization),\n  plus x-app-id and x-app-secret application credentials issued by RentCheck.\n  Access tokens are obtained via the /v1/oAuth2 token endpoints\n  (emailPasswordAuth -> access/token, refreshToken). App id/secret are provisioned\n  from the RentCheck API integration page (app.getrentcheck.com/account/integrations/rentcheck-api).\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Authorization key needed to use the API\n  sources:\n  - openapi/rentcheck-openapi-original.yml\n- name: x-app-id\n  type: apiKey\n  in: header\n  parameter: x-app-id\n  description: Represents the identification of you application\n  sources:\n  - openapi/rentcheck-openapi-original.yml\n\
  - name: x-app-secret\n  type: apiKey\n  in: header\n  parameter: x-app-secret\n  description: Represents the secret for your application\n  sources:\n  - openapi/rentcheck-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentcheck/refs/heads/main/authentication/rentcheck-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Property Management
- Property Inspection
- Real Estate
- PropTech
- Inspections
- Maintenance
- Rental
---
