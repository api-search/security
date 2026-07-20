---
api_key_in: []
api_specs:
- filename: aghanim-openapi-original.json
  format: json
  label: Aghanim Server-to-Server API
  slug: aghanim-server-to-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aghanim/refs/heads/main/openapi/aghanim-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Aghanim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aghanim secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Aghanim
provider_slug: aghanim
scheme_count: 1
schemes:
- description: Refer to the [Authentication](https://docs.aghanim.com/api-reference/) section for instructions on obtaining an API key and use it as the `Bearer` token.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/aghanim-openapi-original.json
  type: http
slug: aghanim-authentication
source_filename: aghanim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/aghanim-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  description: Refer to the [Authentication](https://docs.aghanim.com/api-reference/) section\n    for instructions on obtaining an API key and use it as the `Bearer` token.\n  sources:\n  - openapi/aghanim-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aghanim/refs/heads/main/authentication/aghanim-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Mobile Games
- Game Publishing
- Direct-to-Consumer
- Payments
- Merchant of Record
- Web Shop
- LiveOps
- Fintech
- Gaming
---
