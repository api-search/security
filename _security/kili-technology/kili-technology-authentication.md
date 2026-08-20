---
api_key_in:
- header
api_specs:
- filename: kili-technology-graphql-api-openapi.yml
  format: yaml
  label: Kili Technology GraphQL API
  slug: kili-technology-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/openapi/kili-technology-graphql-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kili Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kili Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kili Technology
provider_slug: kili-technology
scheme_count: 1
schemes:
- description: 'Kili API key passed in the Authorization header using Kili''s documented format, where the X-API-Key token is embedded in the value: "Authorization: X-API-Key: <YOUR_API_KEY>".'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/kili-technology-openapi.yml
  type: apiKey
slug: kili-technology-authentication
source_filename: kili-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kili-technology-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Kili API key passed in the Authorization header using Kili''s documented format,\n    where the X-API-Key token is embedded in the value: \"Authorization: X-API-Key: <YOUR_API_KEY>\".'\n  sources:\n  - openapi/kili-technology-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kili-technology/refs/heads/main/authentication/kili-technology-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Data Labeling
- Training Data
- Annotation
- GraphQL
---
