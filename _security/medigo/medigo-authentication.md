---
api_key_in:
- header
api_specs:
- filename: medigo-openapi-original.yml
  format: yaml
  label: MEDIGO API
  slug: medigo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medigo/refs/heads/main/openapi/medigo-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Medigo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medigo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Medigo
provider_slug: medigo
scheme_count: 1
schemes:
- description: "Authentication done is via an *API token* provided by MEDIGO. The token should be provided as a bearer in the *Authorization* header of every request\nNote that the string *Bearer* followed by a whitespace should be prepended to the token.\nExample:\n\n    GET /v2/ HTTP/1.1\n    Host: https://api.medigo.com\n    Authorization: Bearer <your-api-token>"
  in: header
  name: partner_token
  parameter: Authorization
  sources:
  - openapi/medigo-openapi-original.yml
  type: apiKey
slug: medigo-authentication
source_filename: medigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/medigo-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: partner_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Authentication done is via an *API token* provided by MEDIGO. The token should be provided as a bearer in the *Authorization* header of every request\n    Note that the string *Bearer* followed by a whitespace should be prepended to the token.\n    Example:\n\n        GET /v2/ HTTP/1.1\n        Host: https://api.medigo.com\n        Authorization: Bearer <your-api-token>\n  sources:\n  - openapi/medigo-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medigo/refs/heads/main/authentication/medigo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Consumer
- Healthcare
- Insurance
- Third Party Administrator
- Claims
- Cost Containment
- Second Medical Opinion
- Medical Travel
- Health Insurance
---
